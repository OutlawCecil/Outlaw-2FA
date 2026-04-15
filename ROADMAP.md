# Outlaw 2FA: Technical Roadmap

## ✅ Done ( 1.0-beta )
- Forked from WristKey
- Cleaned up unused resources and consolidated some to remove them.
- Fixed multiple bugs.
- Modernization of general coding and libraries. Cleared many deprecated alerts and handled all reported coding issues.
- Removed Wristkey ADB import which is nolonger supported or working.
- Rewrite of all pages from Android View system (XML) to Jetpack Compose.
- Created export system to backup codes in password-protected encrypted custom format.
- Added support to import from my custom format.
- Optimization pass to ensure main page is absolutely as fast loading as possible.
- Implemented app "heartbeat" and reworked clock and  auth codes to use it. -Big battery saver!
- Replaced "round device" setting with new 30 second "Global Countdown" timer.
- Added full themes support for all pages and preconfigured 11 themes to choose from.
- Disabled send/receive in wifi transfer (with indicator) if disconnected to wifi
- SDK 33 -> 34

## 🔄 In Progress
- Nicer Themes configuration.
- Stabilization of everything after recent MAJOR rewrite.
- Continue to move all strings to allow for easy translations

## ⏳ Upcoming planned changes
- Continued optimizations for speed (especially on the main page) and battery efficiency.
- Increase target SDK incrementally. (at least 36 eventually)
- Tile support (4 "quick codes")
- Slim down and consolidate imports & libraries
