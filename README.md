# Outlaw 2FA

[![Wear OS](https://img.shields.io/badge/Made%20for-Wear%20OS%203.0-4285f4.svg?style=flat-square&logo=wear%20os)](https://wearos.google.com)
[![License](https://img.shields.io/badge/License-MIT-purple?style=flat-square&logo=libreoffice)](LICENSE)
[![Latest Version](https://img.shields.io/github/v/release/0x4f53/Wristkey?label=Engine%20Version&style=flat-square&logo=semver)](https://github.com/0x4f53/Wristkey)

**Outlaw 2FA** is a high-performance, refined 2FA client for Wear OS. Designed for power users and IT professionals who need reliable, secure, and perfectly aligned access to their codes directly from their wrist.

This project is a specialized fork of the excellent [Wristkey](https://github.com/0x4f53/Wristkey) project, optimized with custom UI layouts and expanded configuration options.

<img src="screenshots/featuregraphic.png" alt="Outlaw 2FA mockup" width="750dp">

---

## 🛠 THE OUTLAW ADVANTAGE (Modifications)
*This version introduces several key improvements over the original source:*

* **Optimized UI Alignment:** Fixed layout issues where OTP codes were rendered too low on circular watch faces.
* **Expanded Settings:** Additional granular controls for display behavior and timeout settings.
* **Refined UX:** Streamlined interface for faster access during login prompts.

---

## FEATURES
- **Standalone Operation:** Use it without ever pairing your watch to a phone.
- **Universal Import:** Supports Aegis, andOTP, and Bitwarden via ADB, WiFi, or file imports.
- **Biometric & PIN Security:** Screen locking via PIN, pattern, or password.
- **Military-Grade Encryption:** Local storage encrypted using **256-bit AES-GCM**.
- **Encrypted Transfers:** WiFi transfers secured using **XSalsa20-Poly1305** and **X25519**.
- **Wide Protocol Support:** TOTP and HOTP (up to SHA512 and 4-8 digits).
- **Universal Design:** Fully responsive for both round and square Wear OS devices.

---

## USAGE & DOCUMENTATION
For detailed setup instructions, including how to import your existing accounts via ADB, please refer to the [Wiki](https://github.com/0x4f53/Wristkey/wiki).

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
