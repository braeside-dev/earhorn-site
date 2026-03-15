---
layout: page
title: Privacy Policy
description: "EarHorn Privacy Policy. Learn how EarHorn handles your information."
permalink: /privacy/
---

<div class="legal-content">

**Effective date:** February 20, 2026

Braeside Dev LLC ("Braeside Dev") built EarHorn as a baby monitor app. This page describes how the app handles your information. This Privacy Policy is governed by and subject to the [Terms of Service]({{ '/terms' | relative_url }}), including the governing law and dispute resolution provisions therein.

## Data Collection

EarHorn does not collect personal information. The app does not require an account and does not ask for personal details such as your name or email address.

## Device Identifiers

EarHorn generates a random device identifier (UUID) on first launch to facilitate device pairing and reconnection. This identifier is stored locally on your device in the iOS Keychain and is not transmitted to Braeside Dev or any third party. It persists until the app is deleted or devices are unpaired.

## Cryptographic Keys

EarHorn generates P-256 cryptographic keys for device authentication. These keys are stored in the iOS Keychain with protections that prevent them from being synced to iCloud or backed up. Keys are deleted when the app is removed.

## Audio and Device Communication

EarHorn streams audio between your paired devices over your local WiFi network using Apple's Multipeer Connectivity framework. Audio data is transient — it is processed locally on-device and streamed directly to paired devices. Audio is not retained after playback and is not transmitted to Braeside Dev, Apple, or any third party.

When in baby mode, the app accesses the device microphone continuously to detect sound above your configured threshold. Audio is only streamed to paired parent devices when the threshold is exceeded.

## iCloud and CloudKit

EarHorn uses Apple's CloudKit service to deliver push notifications when the app is in the background. When sound is detected, the app creates a notification record in your iCloud account containing metadata (timestamp and alert type). These records contain no audio content. Battery alert records are similarly stored when the baby device reaches low battery thresholds.

CloudKit data is stored in Apple's infrastructure under your iCloud account. Braeside Dev does not have access to your CloudKit data. Records are retained until the CloudKit share between devices is revoked.

## Data Retention

- **Audio data**: Not retained. Processed in real-time and discarded after playback.
- **Device identifiers**: Stored locally until the app is deleted or devices are unpaired.
- **Cryptographic keys**: Stored locally until the app is removed.
- **CloudKit records**: Retained in your iCloud account until the share is revoked.

## Analytics and Tracking

EarHorn does not include analytics, advertising, or third-party tracking.

## Children's Privacy

EarHorn is designed for use by adult caregivers aged 18 and older, not by children directly. While the app captures audio that may include children's voices, this audio streams exclusively between the user's own paired devices over their local network. Braeside Dev does not collect, receive, store, or have access to any audio data, including children's voices. Because no audio data is transmitted to or collected by Braeside Dev, the app does not trigger operator obligations under the Children's Online Privacy Protection Act (COPPA). Braeside Dev does not knowingly collect personal information from children under 13.

## California and State Privacy Rights

EarHorn does not sell or share personal information as defined under the California Consumer Privacy Act. Because EarHorn does not collect personal information beyond locally-stored device identifiers, the rights to know, delete, and opt out under state privacy laws are addressed by the app's design: there is no personal data held by Braeside Dev to disclose, delete, or stop selling.

## Changes to This Policy

If this policy is updated, the revised version will be posted on this page with a new effective date.

## Contact

If you have questions about this policy, contact Braeside Dev at [info@braesidedev.com](mailto:info@braesidedev.com) or via the contact information listed on the App Store.

</div>
