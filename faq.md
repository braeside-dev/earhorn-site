---
layout: page
title: FAQ
description: "Frequently asked questions about EarHorn, the privacy-first iPhone baby monitor app."
permalink: /faq/
---

<div class="faq-category">
<h3>Setup & Requirements</h3>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details>
<summary>What do I need to use EarHorn?</summary>
<p>Two iPhones running iOS 16.7 or later, both connected to the same WiFi network. That's it — no extra hardware, no account, no subscription.</p>
</details>
</div>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details>
<summary>Does EarHorn work without WiFi?</summary>
<p>EarHorn requires both devices to be on the same WiFi network for audio streaming. Push notifications (for when the app is backgrounded) require an internet connection, but the core monitoring works entirely over your local network.</p>
</details>
</div>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details>
<summary>Can I use an old iPhone as the baby unit?</summary>
<p>Yes. Any iPhone running iOS 16.7 or later works great. That old iPhone 8 in your drawer is a great baby monitor — just plug it in and set it up as the baby device.</p>
</details>
</div>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details>
<summary>Does EarHorn work on iPad?</summary>
<p>EarHorn is currently iPhone-only. iPad support may be added in a future update.</p>
</details>
</div>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details>
<summary>How should I position the baby device?</summary>
<p>Place the phone close enough to pick up sound but out of the baby's reach, with the microphone (bottom of the phone) facing toward the baby. Keep it plugged in. A <strong>gooseneck phone mount</strong> (the flexible clamp-arm holders that attach to a nightstand or furniture) works well for positioning. <strong>Important:</strong> Keep the phone and all cables out of the baby's reach. Never place cords within reach of the crib. Ensure any mount is securely attached and cannot fall. Follow CPSC and AAP safe sleep guidelines.</p>
</details>
</div>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details>
<summary>How do I pair the baby and parent devices?</summary>
<p>Choose "Baby" on one device and "Parent" on the other. The baby device generates a 6-character pairing code. Enter that code on the parent device. Once paired, your devices will automatically reconnect in the future without needing the code again.</p>
</details>
</div>

</div>

<div class="faq-category">
<h3>Privacy & Security</h3>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details>
<summary>Does EarHorn send data to the cloud?</summary>
<p>Audio streams directly between your devices over your home WiFi using peer-to-peer technology. No audio data is sent to the internet. The only thing that goes online is push notification metadata through Apple's CloudKit (which contains no audio content — just that sound was detected).</p>
</details>
</div>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details>
<summary>How secure is EarHorn's connection?</summary>
<p>EarHorn uses P-256 elliptic curve cryptography, a widely-used industry standard recommended by NIST. Devices authenticate each other with a 3-step cryptographic handshake. Encryption keys are stored only on your device (in the iOS Keychain) and never leave your phone.</p>
</details>
</div>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details>
<summary>Can anyone else listen to my baby monitor?</summary>
<p>Audio only streams between devices you've explicitly paired using the 6-character code. The connection is encrypted, and the peer-to-peer architecture means there's no server for anyone to intercept. The baby device always displays how many parent devices are currently connected — so you can verify at a glance that only the devices you expect are listening.</p>
</details>
</div>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details>
<summary>Does EarHorn require an account?</summary>
<p>No. There is no account to create, no email to enter, no password to remember. EarHorn works entirely on-device. The only Apple service it optionally uses is iCloud for push notifications, using your existing Apple ID transparently.</p>
</details>
</div>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details>
<summary>Does EarHorn include analytics or tracking?</summary>
<p>No. EarHorn does not include any analytics frameworks, advertising SDKs, or third-party tracking. We don't collect usage data, and we have no way to see how you use the app.</p>
</details>
</div>

</div>

<div class="faq-category">
<h3>Usage & Features</h3>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details>
<summary>How does the sound threshold work?</summary>
<p>EarHorn continuously listens but only streams audio when the nursery sound level crosses your configured threshold. Smart filtering (hysteresis) requires sustained sound above the threshold to trigger, which means a brief sound like a door slam is less likely to trigger an alert than sustained sound like crying. Results depend on threshold settings, device placement, and environmental conditions. You can adjust the threshold from either the baby or parent device.</p>
</details>
</div>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details>
<summary>What is pre-roll audio?</summary>
<p>When EarHorn detects sound above your threshold, it sends the audio that triggered the alert — not just what came after. A 1-second buffer captures the triggering sound, so you hear exactly what woke your baby, not just the crying that followed.</p>
</details>
</div>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details>
<summary>Can multiple parents listen at the same time?</summary>
<p>This feature is currently in beta testing. EarHorn is designed to support multiple parent devices connecting to the same baby device simultaneously — perfect for when one parent is upstairs and the other is in the garage. We're still testing this in real-world conditions and will update when it's fully validated.</p>
</details>
</div>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details>
<summary>Can I adjust the sensitivity from the parent device?</summary>
<p>Yes. The parent device has a threshold slider that sends adjustments to the baby device in real-time. You'll see a visual confirmation when the baby device acknowledges the change — no need to tiptoe back to the nursery.</p>
</details>
</div>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details>
<summary>Does EarHorn have video monitoring?</summary>
<p>No, by design. EarHorn is deliberately audio-only. No camera means no video to hack, no cloud storage of nursery footage, and dramatically better battery life. Audio is what matters at 3 AM — you need to know if your baby is crying, not watch them sleep.</p>
</details>
</div>

</div>

<div class="faq-category">
<h3>Battery & Performance</h3>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details>
<summary>Will EarHorn drain my phone battery?</summary>
<p>The baby device uses the microphone continuously, so it will use more battery than idle — similar to a voice recording app. For extended monitoring, we recommend keeping it plugged in. The parent device uses minimal battery when waiting for audio. EarHorn alerts you when the baby device reaches 20% and 10% battery.</p>
</details>
</div>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details>
<summary>Does EarHorn work in the background?</summary>
<p>The baby device continues monitoring in the background using iOS background audio. The parent device receives push notifications when sound is detected, even if you've switched to another app. For the best experience, keep EarHorn in the foreground on the parent device.</p>
</details>
</div>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details>
<summary>What happens if the baby device's battery dies?</summary>
<p>EarHorn sends battery alerts at 20% and 10% so you have time to plug in. If the baby device dies or the connection drops, the parent device will show a disconnected status and send a disconnection alert so you know monitoring has stopped. For extended monitoring, we recommend keeping the baby device plugged in.</p>
</details>
</div>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details>
<summary>What happens if WiFi drops briefly?</summary>
<p>EarHorn has built-in reconnection logic with a grace period. Brief WiFi hiccups are handled automatically — the connection typically recovers on its own within seconds without alerting you unnecessarily.</p>
</details>
</div>

</div>

<div class="faq-category">
<h3>Comparison</h3>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details>
<summary>How is EarHorn different from a hardware baby monitor?</summary>
<p>EarHorn is portable — it works anywhere you have WiFi and two phones. It's great for travel, visiting family, hotel stays, Airbnbs, or as a backup when your main monitor isn't available. There's no extra hardware to buy and no subscription. Hardware monitors are excellent for a dedicated nursery setup; EarHorn is the monitor you can always have with you.</p>
</details>
</div>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details>
<summary>How is EarHorn different from other baby monitor apps?</summary>
<p>Most baby monitor apps route audio through cloud servers. EarHorn is strictly peer-to-peer — audio data streams only over your local network and is not sent to any external server. EarHorn also has features most apps lack: pre-roll audio capture, hysteresis-based smart detection, P-256 cryptographic authentication, and a live 5-minute audio visualization graph.</p>
</details>
</div>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details>
<summary>Why doesn't EarHorn have video?</summary>
<p>Privacy and security. No camera means no video to hack, no nursery footage stored on cloud servers, and no risk of visual surveillance being compromised. It also means dramatically better battery life and simpler setup. Audio monitoring catches the things that matter — crying, coughing, unusual sounds — without the risks that come with a camera.</p>
</details>
</div>

</div>

<div class="faq-category">
<h3>Permissions</h3>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details>
<summary>Why does EarHorn ask for microphone access?</summary>
<p>The baby device uses the microphone to listen for sound above your configured threshold. Without microphone access, EarHorn can't monitor audio. The microphone is only actively used when monitoring is running. No audio is recorded, stored, or sent to Braeside Dev — it streams directly to your paired parent device over your local network.</p>
</details>
</div>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details>
<summary>Why does EarHorn ask for local network access?</summary>
<p>EarHorn uses your local WiFi network to discover and connect to your other device. Apple requires apps to request local network permission before they can communicate with other devices on the same network. This is how the baby and parent devices find each other and stream audio — no internet or cloud server is involved.</p>
</details>
</div>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details>
<summary>Why does EarHorn ask for notification access?</summary>
<p>Notifications let EarHorn alert you when sound is detected while the app is in the background, when the baby device's battery is running low, and when the connection between devices drops. If you decline notifications, EarHorn will still work — but you'll need to keep the app open to see status changes on screen. You won't receive any alerts when the app is in the background.</p>
</details>
</div>

</div>

<script type="application/ld+json">
{
    "@context": "https://schema.org",
    "@type": "FAQPage",
    "mainEntity": [
        {
            "@type": "Question",
            "name": "What do I need to use EarHorn?",
            "acceptedAnswer": {
                "@type": "Answer",
                "text": "Two iPhones running iOS 16.7 or later, both connected to the same WiFi network. No extra hardware, no account, no subscription."
            }
        },
        {
            "@type": "Question",
            "name": "Does EarHorn work without WiFi?",
            "acceptedAnswer": {
                "@type": "Answer",
                "text": "EarHorn requires both devices to be on the same WiFi network for audio streaming. Push notifications require an internet connection, but the core monitoring works entirely over your local network."
            }
        },
        {
            "@type": "Question",
            "name": "Does EarHorn send data to the cloud?",
            "acceptedAnswer": {
                "@type": "Answer",
                "text": "No. Audio streams directly between your devices over your home WiFi using peer-to-peer technology. No audio ever touches the internet."
            }
        },
        {
            "@type": "Question",
            "name": "How secure is EarHorn's connection?",
            "acceptedAnswer": {
                "@type": "Answer",
                "text": "EarHorn uses P-256 elliptic curve cryptography with a 3-step mutual authentication handshake. Encryption keys are stored in the iOS Keychain and never leave your device."
            }
        },
        {
            "@type": "Question",
            "name": "Can I use an old iPhone as the baby unit?",
            "acceptedAnswer": {
                "@type": "Answer",
                "text": "Yes. Any iPhone running iOS 16.7 or later works. That old iPhone 8 in your drawer is a great baby monitor."
            }
        },
        {
            "@type": "Question",
            "name": "What is pre-roll audio?",
            "acceptedAnswer": {
                "@type": "Answer",
                "text": "When EarHorn detects sound above your threshold, it sends the audio that triggered the alert — not just what came after. A 1-second buffer captures the triggering sound."
            }
        },
        {
            "@type": "Question",
            "name": "Can multiple parents listen at the same time?",
            "acceptedAnswer": {
                "@type": "Answer",
                "text": "This feature is currently in beta testing. EarHorn is designed to support multiple parent devices connecting simultaneously, and we're testing in real-world conditions."
            }
        },
        {
            "@type": "Question",
            "name": "Does EarHorn have video monitoring?",
            "acceptedAnswer": {
                "@type": "Answer",
                "text": "No, by design. EarHorn is deliberately audio-only. No camera means no video to hack, no cloud storage of nursery footage, and dramatically better battery life."
            }
        },
        {
            "@type": "Question",
            "name": "How is EarHorn different from a hardware baby monitor?",
            "acceptedAnswer": {
                "@type": "Answer",
                "text": "EarHorn is portable — great for travel, visiting family, or as a backup. No extra hardware to buy and no subscription. Hardware monitors are excellent for a dedicated nursery; EarHorn is the monitor you can always have with you."
            }
        }
    ]
}
</script>
