# PlayRank Images Repository Setup

This repository stores all game images for PlayRank platform.

## 📁 Directory Structure

```
playrank-images/
├── images/
│   ├── logos/           # Game logos (128x128px, PNG)
│   ├── covers/          # Game covers (1280x720px, JPG)
│   ├── screenshots/     # Game screenshots
│   └── avatars/         # User avatars (64x64px)
└── README.md
```

## 🚀 How to Use

All images are served via jsDelivr CDN automatically:

```
https://cdn.jsdelivr.net/gh/kennyzir/playrank-images@main/images/logos/moto-x3m.png
```

## 📝 Image Naming Convention

- **Lowercase**: all-lowercase-with-dashes
- **No spaces**: use dashes instead
- **Format**: 
  - Logos: `game-name.png`
  - Covers: `game-name-cover.jpg`
  - Screenshots: `game-name-ss1.jpg`

## 📐 Image Specifications

### Logos
- Size: 128x128px (square)
- Format: PNG (with transparency)
- Max size: 50KB

### Covers
- Size: 1280x720px (16:9)
- Format: JPG/WebP
- Max size: 200KB

### Screenshots
- Size: 1920x1080px or 1280x720px
- Format: JPG/WebP
- Max size: 300KB

## 🎯 Current Games

Add your game images here following the naming convention above.

## 🔧 Integration

Configured in PlayRank's `.env.local`:
```env
NEXT_PUBLIC_GITHUB_USERNAME=kennyzir
NEXT_PUBLIC_GITHUB_IMAGE_REPO=playrank-images
NEXT_PUBLIC_GITHUB_BRANCH=main
```

## 📊 CDN Cache

- First load: 5-10 minutes to cache
- Subsequent loads: Instant (cached globally)
- Cache duration: 1 year

## 🌍 Global CDN

jsDelivr provides:
- 🌏 Multi-CDN (Cloudflare, Fastly, etc.)
- 🚀 100+ global locations
- 📈 10 billion requests/month
- 🆓 100% free forever
