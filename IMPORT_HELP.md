# In-and-Outs of Imports

Outlaw 2FA can import from a variety of **unencrypted** OTP export files and text layouts. In most cases, the file name and extension matter less than the actual content inside the file. Outlaw 2FA mainly looks for valid OTP data such as a secret, an `otpauth://` URI, or a known JSON structure.

In general, a **valid secret is required** for an item to import. If an entry includes a valid secret plus normal OTP fields, Outlaw 2FA will usually be able to import it. An issuer or account name is strongly recommended so the imported item is easy to recognize, but if both are missing and a valid secret is present, Outlaw 2FA can still import the entry.

## ✅ Fully supported

- **Outlaw 2FA encrypted backup (`.o2fa`)** — this is the only encrypted backup format officially supported for direct import.
- **Outlaw 2FA plain JSON export**.
- **Outlaw 2FA plain otpauth text export**.
- **Aegis unencrypted JSON export**.
- **Bitwarden JSON exports that include OTP data**.

## ✅ Supported generic layouts

These are not tied to one specific app, but they are accepted when the data layout is compatible:

- Plain `otpauth://...` text, including one or multiple entries.
- JSON arrays or objects containing recognizable OTP fields such as:
  - `secret`
  - `issuer`
  - `account`
  - `label`
  - `type`
  - `algorithm`
  - `digits`
  - `period`
  - `counter`
- Some CSV-style exports containing recognizable OTP fields such as secret, issuer, account, type, digits, period, counter, or otpauth URL.

## ⚠️ Likely supported, but not guaranteed

These may work **if exported in plain, compatible JSON/text form**:

- **andOTP** plain JSON or other compatible unencrypted exports.
- **Raivo OTP** data converted or exported into a standard JSON or otpauth-friendly structure.
- Other authenticator exports that include standard otpauth URIs or clearly structured OTP secrets.

## 🔍 Possible partial support

These may import partially, may need cleanup first, or may need conversion to a simpler format before importing:

- **2FAuth / 2FAS** backups.
- **Authy** exports or extracted OTP data.
- Other proprietary or encrypted third-party backup formats.

## Recommended import format

This is the simplest recommended JSON layout:

```json
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

## Minimum accepted format

A valid secret is the most important field. The rest can often be inferred or defaulted if needed, but including at least a name-related field is strongly recommended.

```json
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

## Plain otpauth example

Outlaw 2FA also supports plain otpauth URIs, which are commonly used by authenticator apps and OTP tools. The `secret` parameter is required, and `issuer` is strongly recommended.

```text
otpauth://totp/Google:alice@gmail.com?secret=JBSWY3DPEHPK3PXP&issuer=Google&algorithm=SHA1&digits=6&period=30
otpauth://hotp/Legacy%20VPN:alice?secret=KRSXG5CTMVRXGI3S&issuer=Legacy%20VPN&algorithm=SHA1&digits=6&counter=0
```

## Notes

- Imports lean toward best-effort. If format is incorrect, it will attempt to pull secrets along with whatever else it can.
- Encrypted imports are intentionally limited to Outlaw 2FA’s own secure backup format.
- If an import file contains duplicate secrets, existing items may be matched instead of added as new entries.
- For best results, include at least a valid `secret` plus an `issuer` or `account` name.
