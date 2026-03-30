# AntiDarkSword ⚔️

**System-wide JS kill-switch with exceptions.**

AntiDarkSword is an advanced iOS security tweak designed to harden jailbroken devices against WebKit and iMessage-based exploits. It significantly reduces your device's attack surface by neutralizing common vectors used in one-click and zero-click attacks.

## ✨ Features

* **WebKit Hardening:** Forcibly disables JavaScript execution, inline media playback, Picture-in-Picture, WebGL, WebRTC (peer connections), and local file access within targeted web views.
* **iMessage Mitigation:** Defends against BlastPass/FORCEDENTRY-style attacks by disabling automatic attachment downloading and preview generation.
* **Tiered Protection:**
  * **Level 1:** Protects native Apple apps and services.
  * **Level 2:** Expands protection to major third-party browsers and social media apps.
  * **Level 3:** Locks down critical system daemons to prevent daemon-level zero-clicks.
* **Custom Targeting:** Manually specify bundle IDs or process names to restrict specific apps or background tasks.

## 📦 Compatibility

* **Architecture:** Rootful (iphoneos-arm64)
* **iOS Versions:** iOS 14.5 - 18.0
* **Dependencies:** mobilesubstrate, preferenceloader, com.opa334.altlist

## ⚠️ Warning

Even level one disables email / text previews of files, you have to hold the file down and save to files to view it. Enabling Level 3 restricts critical background daemons (like imagent and mediaserverd). Level 3 may break media playback. Only enable this level if you understand to disable if any issues.
