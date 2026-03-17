# Outlaw 2FA

[![Wear OS](https://img.shields.io/badge/Made%20for-Wear%20OS%205.0+-4285f4.svg?style=flat-square&logo=android)](https://wearos.google.com)
[![License](https://img.shields.io/badge/License-MIT-purple?style=flat-square&logo=libreoffice)](LICENSE)
[![Version](https://img.shields.io/badge/Release-2.0--Snappy-orange?style=flat-square&logo=semver)](https://github.com/OutlawCecil/Outlaw-2FA/releases)

**Lightning‑fast, modern, secure 2FA authenticator completely rebuilt.** TOTP/HOTP codes from your wrist—standalone or phone‑synced. Smaller, safer, snappier than ever.

---

## ✨ Comparisons

| Feature                  | WristKey   | Stratum       | OneAuth    | WristGuardian | 2FA Hub | Google Auth  | **Outlaw 2FA**      |
|--------------------------|------------|---------------|------------|---------------|---------|--------------|---------------------|
| Works on Phone/WearOS    | ✅yes     | ✅companion  | ✅cloud   | ✅yes        | ✅yes  | ✅mirror    | **✅Standalone**   |
| 0 Ads/Nonsense           | ✅yes     | ✅yes        | ❌upsell  | ✅paid       | ✅yes  | ✅yes       | **✅Always**       |
| Battery Life             | ✅good    | ✅Good          | Avg       | ✅Good         | Avg    | Avg         | **✅Optimized**    |
| App Size                 | 13 MB     | ~15 MB       | 7 MB      | 5 MB         | 8 MB   | 10 MB       | **~5 MB**           |
| Old Watches (2018+)      | ✅yes     | ✅yes        | ✅yes     | ✅yes        | ✅yes  | ✅yes       | **✅Faster**       |
| New Watches (2025+)      | ❌risky   | ✅sideload   | ✅yes     | ✅yes        | ✅yes  | ✅yes       | **✅Perfect**      |
| Tile Support             | ❌         | ❌            | ❌         | ❌            | ❌      | ❌           | **✅4 Codes**      |
| Import Bitwarden/Aegis   | ❌manual  | QR/backup    | ❌ cloud   | ❌ manual     | ❌basic| QR only     | **✅Drag JSON**    |
| Google Play Safe         | ❌2022    | ❌ delisted   | ✅yes     | ❌ paid       | ✅yes  | ✅yes       | **✅2026 Std**     |
| Phone Sync               | ❌adb     | Companion req| Cloud req | None         | None   | Mirror      | **BT/WiFi**         |


---

## 📱 Install
1. Sideload APK (Wear OS 3.0+).
2. Import vault (QR/JSON).
3. Add tiles: Long‑press watch face → "Outlaw 2FA".

---

## 🔒 Security
- **Tink StreamingAEAD** (AES256‑GCM‑HKDF).
- Encrypted DataStore (MasterKey).
- Ghost migration from WristKey WFS.

---

## Acknowledgements
Inspired by [Wristkey](https://github.com/0x4f53/Wristkey) core.  
Thanks: Kotlin Onetimepassword, Wear Compose, Tink.

---

## License
MIT © 2026 Outlaw 2FA. Free to fork/use/sell
