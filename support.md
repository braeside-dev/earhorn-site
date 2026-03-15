---
layout: page
title: Support
description: "Get help with EarHorn. Troubleshooting tips, setup help, and contact information."
permalink: /support/
---

## Troubleshooting

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details open>
<summary>Devices can't find each other</summary>
<p>Both devices must be on the same WiFi network. Check that both are connected to the same network name (not one on 2.4GHz and the other on 5GHz with different SSIDs). Try toggling WiFi off and back on, then reopen EarHorn.</p>
</details>
</div>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details open>
<summary>Connection drops or won't reconnect</summary>
<p>Close EarHorn on both devices, wait 10 seconds, then reopen. EarHorn needs a moment to clean up the previous connection before reconnecting. If the issue persists, try restarting both devices.</p>
</details>
</div>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details open>
<summary>No audio is coming through</summary>
<p>Check that the baby device has granted microphone permission (Settings > Privacy & Security > Microphone > EarHorn). Also verify the sound threshold isn't set too high — try lowering it from the parent device's threshold slider.</p>
</details>
</div>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details open>
<summary>Push notifications aren't working</summary>
<p>Push notifications require both devices to have an internet connection and iCloud signed in. Check that notifications are enabled for EarHorn in Settings > Notifications. You can use the "Test Push" button in EarHorn's settings to verify your setup.</p>
</details>
</div>

<div class="card" style="padding: 16px 20px; margin-bottom: 12px;">
<details open>
<summary>Too many false alerts</summary>
<p>Raise the sound threshold from the parent device. EarHorn uses smart filtering to avoid false triggers from brief sounds, but if your environment is consistently noisy (fan, white noise machine), a higher threshold will help. Place the baby device closer to the crib and away from noise sources.</p>
</details>
</div>

## Known Limitations

- **Audio only** — EarHorn does not include video monitoring, by design
- **Same WiFi required** — audio streaming requires both devices on the same local network
- **Push notifications require iCloud** — background alerts use Apple's CloudKit service
- **Not a safety device** — EarHorn is a convenience tool and does not replace attentive supervision

## Contact

For issues not covered above, contact us at [info@braesidedev.com](mailto:info@braesidedev.com). We aim to respond within 48 hours.

You can also check the [FAQ]({{ '/faq' | relative_url }}) for answers to common questions.
