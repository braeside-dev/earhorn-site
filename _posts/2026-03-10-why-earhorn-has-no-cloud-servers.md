---
layout: post
title: "Why EarHorn Has No Cloud Servers"
description: "Most baby monitor apps route audio through cloud servers. EarHorn doesn't. Here's why we chose peer-to-peer architecture and what it means for your privacy."
date: 2026-03-10
---

When we started building EarHorn, we had to make a fundamental architectural decision: should audio go through our servers, or should it stream directly between devices?

We chose direct. Here's why.

## The problem with cloud baby monitors

Most baby monitor apps — and virtually all WiFi baby cameras — route audio and video through cloud servers. The typical flow looks like this:

1. Baby device captures audio/video
2. Audio/video uploads to company's cloud server
3. Server relays it to the parent device
4. Parent sees/hears the feed

This architecture exists because it's simpler to build. Cloud relay handles NAT traversal, works across different networks, and lets companies add features like recording and AI analysis.

But it comes with real costs:

**Privacy**: Your baby's audio (or video) is on someone else's server. Even with encryption in transit, the company's infrastructure handles the data. Server breaches happen. Insider threats exist. And privacy policies can change.

**Security**: Cloud-connected cameras are a target. Every year brings new stories of hacked baby monitors — strangers talking to children through the camera, footage leaked online, or cameras recruited into botnets. The attack surface is large: the camera itself, the cloud API, the company's infrastructure, and the user's account credentials.

**Reliability**: Your monitor now depends on the company's servers being up. Server outages, maintenance windows, or the company going out of business all mean your monitor stops working.

**Ongoing cost**: Servers cost money. That cost gets passed to you as a subscription — often $50-100/year, on top of the hardware cost.

## How EarHorn works instead

EarHorn uses Apple's Multipeer Connectivity framework to stream audio directly between your devices over your home WiFi network. The architecture is simple:

1. Baby device captures audio
2. Audio streams directly to parent device over local WiFi
3. That's it. No server in the middle.

The only thing that touches the internet is push notification metadata — and that contains no audio content. When the baby device detects sound, it creates a CloudKit record through Apple's servers that says, essentially, "sound was detected." The actual audio data stays on your local network.

## What this means in practice

**Your audio stays on your network by design.** We have no servers receiving audio. There is no cloud infrastructure to breach. A remote attacker cannot access your baby monitor through our servers because there are no servers to attack. Your audio only traverses your local network, which means protecting your home WiFi is what protects your monitor.

**No accounts, no credentials to steal.** EarHorn doesn't have user accounts. There's no email/password combination to phish, no database of user credentials to breach. Devices authenticate each other directly using P-256 elliptic curve cryptography.

**It works without internet.** If your internet goes down but your WiFi router is still running, EarHorn keeps monitoring. Your local network is all it needs for the core functionality.

**No subscription needed.** We don't have server costs to pass along. EarHorn is a one-time purchase.

## The tradeoff

The honest tradeoff is that EarHorn requires both devices to be on the same WiFi network. You can't monitor from across town or check in from work. For parents who need remote access, a cloud-connected camera makes sense.

But for the primary use case — monitoring a sleeping baby from another room in your house — a local connection is not just sufficient, it's better. Lower latency, no internet dependency, and a dramatically smaller attack surface.

## The security layer

Peer-to-peer doesn't mean unprotected. EarHorn implements serious security:

- **P-256 mutual authentication**: Both devices verify each other's identity using NIST P-256 elliptic curve cryptography with a 3-step handshake
- **Encrypted sessions**: All MPC sessions require encryption
- **Secure pairing**: The 6-character pairing code uses PBKDF2 key derivation with 600,000 iterations and HMAC-SHA256 verification
- **Rate limiting**: Failed pairing attempts trigger exponential backoff (up to 1-hour lockout)
- **Keychain storage**: All cryptographic keys stored with `kSecAttrAccessibleWhenUnlockedThisDeviceOnly` — not synced to iCloud, deleted on device wipe

P-256 is a widely-used industry standard recommended by NIST. With EarHorn, the encryption is between your own devices, with no third party in the middle.

## Building trust through architecture

We believe the strongest privacy approach isn't just a policy — it's architecture. A policy says "we won't look at your data." Architecture means we never have the opportunity to.

EarHorn is built so that audio data flows only between your paired devices over your local network. We have no servers receiving it, no infrastructure storing it, and no way to access it.

*EarHorn is a convenience tool for audio monitoring and is not a substitute for attentive supervision.*
