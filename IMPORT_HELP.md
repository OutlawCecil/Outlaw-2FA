# In-and-Outs of Imports
Outlaw 2FA supports imports from other program's (unencrypted) exported files. File name and filetype do not matter as much as overall layout of the text. In general, Outlaw 2FA must find a secret to import otherwise it will fail to pull anything in. Secret + some sort of name is recommended minimum so you know where that secret belongs to.

## ✅ Fully supported formats
- Aegis
- BitWarden
- andOTP
- The only encrypted format supported is our own secured .o2fa format (exported from Outlaw 2FA)

## ⚠️ Likely Supported (Untested)
- Raivo OTP
- Plain otpauth

## 🔍 Possible Partial Support (Untested)
- 2FAuth / 2FAS backup
- Authy

Most simplistic, recommended & supported import format:
```JSON
[
  {
    "secret": "JBSWY3DPEHPK3PXP",
    "issuer": "Google",
    "account": "alice@gmail.com",
    "label": "Personal Gmail",
    "type": "TOTP",
    "algorithm": "SHA1",
    "digits": 6,
    "period": 30
  },
  {
    "secret": "KRSXG5CTMVRXGI3S",
    "issuer": "Legacy VPN",
    "account": "alice",
    "label": "Office Token",
    "type": "HOTP",
    "algorithm": "SHA1",
    "digits": 6,
    "counter": 0
  }
]
```


Minimal format for import:
```JSON
[
  {
    "secret": "JBSWY3DPEHPK3PXP",
    "type": "TOTP"
  },
  {
    "secret": "KRSXG5CTMVRXGI3S",
    "type": "HOTP",
    "counter": 0
  }
]
```
