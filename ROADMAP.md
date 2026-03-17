# Outlaw 2FA: Technical Roadmap

## ✅ Done (2.0 Snappy)
- Compose BOM 1.6.0‑rc01: 100% M3, adaptive ScalingLazyColumn (compact/expanded).
- Heartbeat Engine: MainViewModel StateFlow + Handler <API30 (anti‑throttle).
- SecurityManager: Tink AES256‑GCM‑HKDF, EncryptedDataStore, ghost WFS migration.
- Sync: DataLayer (/vaultsync urgent), WiFiTransfer (localhost:9999).
- Imports: ParserUtil IO (Bitwarden/Aegis/andOTP/otpauth‑migration).
- OtpTileService: Top 4 codes, 30s refresh, vault‑bound.
- Baselines: GMD API26 (32‑bit)/35 (64‑bit), ~20% startup.
- APK: ~5 MB (−60% vs WristKey). min26/target35.

## 🔄 In Progress
- Search: RemoteInput + MainViewModel.filter.
- AccountCard: OTP copy/beep/HOTP ±.
- NOTE: Goal is Wristkey feature base

## ⏳ Upcoming planned changes
- Theme Engine: Provide Built-in themes + allow importing / customizing
- Keyguard: Biometric/PIN
- Export: Vault QR/JSON
- HCE: NFC tap‑to‑auth (Wear 5+)
