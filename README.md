# 🎮 Kenda Herbs Games Repository

This repository hosts downloadable mini-games for the Kenda Herbs mobile application.

## 📦 Available Games

1. **Herb Matching** 🌿 - Memory matching game with herb cards
2. **Memory Challenge** 🧠 - Sequential memory test
3. **Virtual Cooking** 🍵 - Recipe-based herbal tea brewing
4. **Quick Tap** ⚡ - Fast reflex tapping challenge
5. **Daily Spin** 🎡 - Daily bonus wheel (once per day)

## 🎯 How It Works

The Kenda Herbs mobile app downloads game configurations (JSON files) from this repository and renders them dynamically. This allows:
- **Small APK size** - Games are not bundled in the app
- **Easy updates** - Update games without app updates
- **User choice** - Download only desired games
- **New games** - Add games anytime without releasing new app version

## 📱 For App Users

Games are downloaded automatically through the Gaming Hub in the Kenda Herbs app. Each game awards points that can be redeemed for discounts up to 10% on your orders!

### Point System:
- 100 points = 1% discount
- Maximum 1000 points = 10% discount
- Points reset after purchase (encourages replay)

## 🛠️ For Developers

### Game Structure:
```
games/
├── [game_id]/
│   ├── manifest.json    # Game metadata
│   ├── game.json       # Game configuration & logic
│   ├── assets/         # Images, sounds (optional)
│   └── preview.png     # Thumbnail (400x300px)
```

### Game Configuration:
All games are JSON-based with the following structure:
- **manifest.json** - Metadata (name, version, size, etc.)
- **game.json** - Game rules, difficulty levels, scoring
- **preview.png** - Preview image shown in app

### Adding a New Game:
1. Create folder in `games/[game_id]/`
2. Add `manifest.json`, `game.json`, `preview.png`
3. Update `games_catalog.json` with new game entry
4. Commit and push
5. App automatically detects new game!

## 📊 Games Catalog

The master catalog is in `games_catalog.json` at the root. This file lists all available games and is fetched by the app on startup.

## 🔄 Updates

To update a game:
1. Modify the game files
2. Increment version in `manifest.json`
3. Update version in `games_catalog.json`
4. Commit and push
5. App users see update available!

## 📄 License

Proprietary - © 2025 Kenda Herbs  
All rights reserved.

## 📞 Contact

For questions or issues:
- **Email:** kenda.herbs@gmail.com
- **WhatsApp:** +20 103 514 3025

---

**Last Updated:** November 10, 2025  
**Repository Version:** 1.0.0  
**Total Games:** 5

