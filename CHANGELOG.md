# Changelog

All notable changes to this project will be documented in this file as versions increase.

## 📈 Goal ( 1.0 ) soon-ish
- Initial public GitHub release.

...


## ✅ Done ( 0.7-beta )
- Nicer Themes configuration. Seperated background color from accent color. And new menu.
- Rewrite imports to ensure support for latest Bitwarden (csv & json), Aegis (json), andOPT (json). Filetype not required, only format. Likely also support Raivo OTP and plain otpauth. Chance of success with 2FAuth, 2FAS, and Authy as well.
- Touched up exporting to better match importing.
- Slight change in how themes apply to the main page. Will roll out to all others eventually.
- Increase security by hiding secret on edit screen and requiring device lock to view

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
- Realized I should do more than fork & fix.
