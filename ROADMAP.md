# Outlaw 2FA: Technical Roadmap

## 🔄 In Progress
- Stabilization of everything after recent MAJOR rewrite.
- Continue to move all strings to allow for easy translations

## ✅ Done ( 0.7-beta )
- Nicer Themes configuration. Seperated background color from accent color. And new menu.
- Rewrite imports to ensure support for latest Bitwarden (csv & json), Aegis (json), andOPT (json). Filetype not required, only format. Likely also support Raivo OTP and plain otpauth. Chance of success with 2FAuth, 2FAS, and Authy as well.

## ✅ Done ( 0.6-beta )
- SDK 33 -> 34 and updating of some dependencies
- Revamped wifi transfer screens
- Revamped export and allowed for unencrypted types
- Revamped manual entry form

## ✅ Done ( 0.5-beta )
- Replaced "round device" setting with new 30 second "Global Countdown" timer.
- Added full themes support for all pages and preconfigured 11 themes to choose from.
- Disabled send/receive in wifi transfer (with indicator) if disconnected to wifi

## ✅ Done ( 0.4-beta )
- Optimization pass to ensure main page is absolutely as fast loading as possible.
- Implemented app "heartbeat" and reworked clock and  auth codes to use it. -Big battery saver!

## ✅ Done ( 0.3-beta )
- Rewrite of all pages from Android View system (XML) to Jetpack Compose.
- Created export system to backup codes in password-protected encrypted custom format.
- Added support to import from my custom format.

## ✅ Done ( 0.2-beta )
- Modernization of general coding and libraries. Cleared many deprecated alerts and handled all reported coding issues.
- Removed Wristkey ADB import which is nolonger supported or working.

## ✅ Done ( 0.1-beta )
- Forked from WristKey
- Cleaned up unused resources and consolidated some to remove them.
- Fixed multiple bugs.


## ⏳ Upcoming planned changes
- Continued optimizations for speed (especially on the main page) and battery efficiency.
- Increase target SDK incrementally. (at least 36 eventually)
- Tile support (4 "quick codes")
- Slim down and consolidate imports & libraries
- Auth groups
