# Outlaw 2FA

[![Wear OS](https://img.shields.io/badge/Made%20for-Wear%20OS%203.0+-4285f4.svg?style=flat-square&logo=wear%20os)](https://wearos.google.com)
[![License](https://img.shields.io/badge/License-MIT-purple?style=flat-square&logo=libreoffice)](LICENSE)
[![Version](https://img.shields.io/badge/Release-1.0--Outlaw-orange?style=flat-square&logo=semver)](https://github.com/YOUR-GITHUB-USERNAME/Outlaw-2FA)

**Outlaw 2FA** is a high-performance, refined 2FA client for Wear OS. Designed for power users and IT professionals who need reliable, secure, and perfectly aligned access to their codes directly from their wrist.

This project is a specialized fork of the excellent [Wristkey](https://github.com/0x4f53/Wristkey) project, optimized with custom UI layouts, corrected vertical alignment, and a completely rebranded standalone identity.

---

## 🛠 THE OUTLAW ADVANTAGE (Modifications)
*This version introduces several key improvements over the original engine:*

* **Fixed Vertical Alignment:** Resolved the "Empty Top Space" bug where layouts would push content down after returning from settings.
* **Optimized Container Padding:** Replaced hard-coded margins with container-level padding for better stability on round watch faces.
* **Complete Rebrand:** Migrated to the `com.outlaw.authenticator` namespace for side-by-side installation with other clients.
* **Modern Build Stack:** Updated to Target SDK 33/34 for better compatibility with the latest Pixel Watch and Galaxy Watch hardware.

---

## FEATURES
- **Standalone Operation:** Use it without ever pairing your watch to a phone.
- **Universal Import:** Supports Aegis, andOTP, and Bitwarden via ADB, WiFi, or file imports.
- **Biometric & PIN Security:** Screen locking via PIN, pattern, or password.
- **Military-Grade Encryption:** Local storage encrypted using **256-bit AES-GCM**.
- **Encrypted Transfers:** WiFi transfers secured using **XSalsa20-Poly1305** and **X25519**.
- **Wide Protocol Support:** TOTP and HOTP (up to SHA512 and 4-8 digits).

---

## ACKNOWLEDGEMENTS
Outlaw 2FA is built upon the hard work of the open-source community:
- **[0x4f53 (Wristkey)](https://github.com/0x4f53/Wristkey)** - The original base project.
- [Marcel Kliemannel](https://github.com/marcelkliemannel/kotlin-onetimepassword) - Kotlin Onetimepassword.
- [Androidmads](https://github.com/androidmads/QRGenerator) - QR Generator.
- [Yuriy Budiyev](https://github.com/yuriy-budiyev/code-scanner) - Code scanner.

*Aegis, andOTP, Google Authenticator, and Bitwarden are trademarks of their respective owners.*

---

## LICENSE
This project is licensed under the **MIT License**. You are free to use, modify, and distribute this software, provided the original copyright notice and permission notice are included.

**[Copyright © 2026 Outlaw 2FA](https://github.com/YOUR-GITHUB-USERNAME-HERE/Outlaw-2FA)** [Original Copyright © 2022 Owais Shaikh](https://github.com/0x4f53/Wristkey)

---

## SUPPORT THE ORIGINAL CREATOR
If you find this app useful, consider supporting the original developer of the engine, [0x4f53](https://github.com/0x4f53), whose core work made this fork possible.
