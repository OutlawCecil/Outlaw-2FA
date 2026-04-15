# Outlaw 2FA

[![Wear OS](https://img.shields.io/badge/Made%20for-Wear%20OS%205.0+-4285f4.svg?style=flat-square&logo=android)](https://wearos.google.com)
[![License](https://img.shields.io/badge/License-MIT-purple?style=flat-square&logo=libreoffice)](LICENSE)
[![Version](https://img.shields.io/badge/Release-1.0-orange?style=flat-square&logo=semver)](https://github.com/OutlawCecil/Outlaw-2FA/releases)

**Lightning‑fast, modern, secure 2FA authenticator completely rebuilt.** TOTP/HOTP codes from your wrist. Smaller, safer, snappier than ever.

+ Custom secure encrypted exports/backups .O2fa
+ Import (and manage accounts) from Bitwarden, Aegis, OTPAuth, or .O2fa
+ App customization options
+ Full Translations support
+ Send to/from watch and phone freely
+ Multi-theme support

---

## ✨ Why Upgrade?

- Based off the baseline of Wristkey, but modernized, optimized, and build almost completely from scratch.
- Full WearOS (watch) AND Android (phone) support.
- Strong backwards compatibility for devices starting around 2017 (SDK 26) Android 8.0 Oreo.
- Modernized for newer devices. Optimized for around 2026 (SDK 34) Android 14 Upside Down Cake. Working toward SDK 36.

---

## 📱 Install
1. Sideload APK (Wear OS 3.0+).
2. Import vault (QR / .JSON / encrypted .O2fa).

---

## 🔒 Security
- EncryptedSharedPreferences with MasterKey for encrypted vault storage.
- Android KeyguardManager for device-credential lock support.
- Ghost migration from WristKey WFS.
- LazySodium for asymmetric crypto/key exchange.
- AES-GCM / AES-CBC + PBKDF2 custom encryption for backup/transfer payloads.
- Sensitive clipboard handling for OTP copying.
- Network/security checks for data transfers.
  
---

## 🛠️ Utilized tools
Kotlin One-Time Password for TOTP/HOTP generation
ZXing for QR code generation
Jetpack Compose including Compose UI, Material 3, and lifecycle-aware state collection.
Kotlin Coroutines
Android ViewModel + StateFlow

---

## Acknowledgements
Lovingly inspired by [Wristkey](https://github.com/0x4f53/Wristkey) core.  

---

## License
MIT © 2026 Outlaw 2FA. Free to fork/use/sell
