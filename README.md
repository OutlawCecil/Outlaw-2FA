# Outlaw 2FA

[![Wear OS](https://img.shields.io/badge/Made%20for-Wear%20OS%205.0+-4285f4.svg?style=flat-square&logo=android)](https://wearos.google.com)
[![License](https://img.shields.io/badge/License-Custom%20Source--Available-purple?style=flat-square&logo=libreoffice)](LICENSE)
[![Version](https://img.shields.io/badge/Release-1.0-orange?style=flat-square&logo=semver)](https://github.com/OutlawCecil/Outlaw-2FA/releases)

**Built from the ground up! Fast, modern, secure offline 2FA authenticator with no bloat. For Phone or Watch!** TOTP/HOTP codes from your wrist! Smaller, safer, snappier than ever. Full import / export support. You're in control!

+ Import, Manage, and Export from:
   - Bitwarden
   - Aegis
   - OTPAuth
   - O2fa (our own encryption)
+ App customization options
+ Full Translations support
+ Send to/from watch and phone freely
+ Many theme combinations to choose from

---

## ✨ Why Upgrade?

- Based off the baseline of Wristkey, but modernized, optimized, and eventually completely rebuilt from scratch.
- Full WearOS (watch) AND Android (phone) support.
- Strong backwards compatibility for devices starting around 2017 (SDK 26) Android 8.0 Oreo.
- Modernized for newer devices. Optimized for current and future devices (SDK 37).
- No "create an account" BS. Offline and yours forever.
- No ads, forever, guaranteed.

---

## 📱 Install
1. Sideload APK (Wear OS 3.0+).
2. Import vault (QR / .JSON / encrypted .O2fa).

---

## 🔒 Enterprise-Grade Security

Outlaw 2FA goes beyond typical authenticator apps with production-grade protections:

| Feature | Outlaw | Typical Apps |
|---------|--------|--------------|
| **Vault Storage** | EncryptedSharedPreferences + **MasterKey** | Plain SharedPreferences |
| **Device Lock** | Android KeyguardManager integration | Basic PIN/biometrics |
| **Backup Encryption** | **AES-GCM + 120K PBKDF2** + magic bytes | AES-CBC + weak PBKDF2 (10K) or no encryption |
| **Device Transfer** | **Curve25519 box-seal** (LazySodium) | Plain QR or weak symmetric |
| **Import Validation** | Normalized secret validation + deduplication | Raw string parsing |
| **Local Servers** | **Route-locked endpoints** + 5s timeouts | Open/wildcard handlers |
| **Clipboard** | Sensitive OTP handling | Raw copy-paste |

**Key advantages:**
- **12x stronger PBKDF2** (120K vs typical 10K) resists brute-force
- **Curve25519** ECDH (audited, patent-free) for transfers
- **No plaintext QR codes** — everything encrypted end-to-end

[LazySodium](https://github.com/terl/lazysodium-android) powers asymmetric crypto.
  
---

## 🛠️ Utilized tools
- Kotlin One-Time Password for TOTP/HOTP generation
- ZXing for QR code generation
- Jetpack Compose including Compose UI, Material 3, and lifecycle-aware state collection.
- Kotlin Coroutines
- Android ViewModel + StateFlow used for speed in some areas.

---

## Acknowledgements
Lovingly inspired by Wristkey core.  

---

## License

**Source-available for non-commercial use only.**

- ✅ Free to view, fork, modify, and use personally.
- ✅ Free to share for non-commercial purposes.
- ❌ Commercial use (app stores, sales, business use) requires prior written permission.

See [LICENSE](LICENSE) for full terms. For commercial licensing, email OutlawCecil@gmail.com.

[![GitHub Sponsors](https://img.shields.io/badge/sponsor-4285f4?style=flat-square&logo=github)](https://github.com/sponsors/OutlawCecil) or  
[![Buy Me a Coffee](https://img.shields.io/badge/Buy%20Me%20a%20Coffee-Donate-yellow?style=flat-square&logo=buymeacoffee)](https://buymeacoffee.com/outlawcecil)
