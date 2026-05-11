# Outlaw 2FA: Technical Roadmap

## 🔄 In Progress
- Stabilization of everything after recent MAJOR rewrite.
- Continue to move all strings to allow for easy translations
- Need to fix alignment of 30s round-screen WearOS countdown timer
- Fix odd delay visting settings, mainly on WearOS
- Additional top-padding needed on WearOS main screen

## ⏳ Upcoming planned changes
- Continued optimizations for speed (especially on the main page) and battery efficiency.
- Slim down and consolidate imports & libraries
- Re-enable Device unlock setting on WearOS
- Auth groups support. Possibly multiple "pages"?'
- Considering option to change theme from colored outlines to using background colors with no/minimal outlines.

## 🪳 Known bugs soon-to-be-fixed
- Manual entry lands you on main page, maybe change to account edit screen
- Padding adjustments, especially on round WearOS
- Manual entry doesn't allow blank account, just duplicates issuer
- Manual entry adds a space if you put a period, not .com friendly
- After an import, status screen needs adjusted to look nicer
- With scrolling long labels enabled, need to adjust long text (such as license page) to still use multiple lines.
