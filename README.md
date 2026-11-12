# LAVIEM - AI Skin Analysis

LAVIEM is an AI-powered skin analysis and diary application designed for tracking skin health over time. Users can capture face photos with guided facial alignment, manually or automatically mark spots, keep daily skincare routines, and observe per-zone skin trends.

- **Repository**: [https://github.com/dinhthianhsang/laviem-ai-skin-analysis](https://github.com/dinhthianhsang/laviem-ai-skin-analysis)
- **Platforms**: Web (Next.js 15) & Mobile (Expo React Native for Android)
- **Tech Stack**: TypeScript, Turborepo, Supabase, MediaPipe / TFLite, Tailwind CSS / NativeWind

---

## Features

- 📸 **Guided Face Capture**: Real-time camera overlay and face alignment using MediaPipe / TFLite.
- 🔍 **Spot Tracking & Redness Detection**: Tap-mark skin spots and analyze skin redness across different facial zones.
- 📝 **Skincare Routine & Checklist**: Log morning and evening skincare routines and track consistency.
- 📊 **Trend Analysis**: Monitor skin progress over time with visual analytics.
- 🛒 **Boutique & Marketplace Integration**: Explore recommended products tailored to skin condition.

---

## Quick Start

### Prerequisites
- [Bun](https://bun.sh) (v1.1+)
- Git
- For Mobile Development: [Android Studio](https://developer.android.com/studio) and Android Emulator or Physical Device

### Installation

```bash
# Clone the repository
git clone https://github.com/dinhthianhsang/laviem-ai-skin-analysis.git
cd laviem-ai-skin-analysis

# Install dependencies
bun install

# Verify workspace type checking & tests
bun run typecheck
bun run test
```

### Running the Web Application

```bash
cd apps/web
bun dev
```
Open [http://localhost:3000](http://localhost:3000) in your browser.

### Running the Mobile Application (Android)

```bash
cd apps/mobile
bun run start
```
Press `a` in the terminal to launch on the connected Android emulator or device.

---

## Setup & Configuration

To connect with a live backend, configure your Supabase credentials:
- **Supabase Setup**: See [docs/setup-guides/supabase.md](docs/setup-guides/supabase.md)
- **Google OAuth Setup**: See [docs/setup-guides/google-oauth.md](docs/setup-guides/google-oauth.md)
- **Deployment**: See [docs/setup-guides/deployment.md](docs/setup-guides/deployment.md)

---

## Project Structure

```
.
├── apps/
│   ├── mobile/   # Expo React Native App
│   └── web/      # Next.js 15 Web App
├── packages/
│   ├── domain/   # Shared business logic & database schemas
│   └── tokens/   # Shared design tokens & styles
├── docs/         # Setup & development documentation
└── mpbench/      # MediaPipe benchmark utilities
```

---

## License

This project is maintained under the LAVIEM repository.
