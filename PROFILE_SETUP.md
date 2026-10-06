# GitHub Profile Setup Guide

This repository (`lyndon18-star`) is your **GitHub Profile README** — it renders on your profile page at `https://github.com/lyndon18-star`.

## ✅ What's Already Working (Purple Theme v2.0)

| Feature | Status |
|---------|--------|
| Hero Identity Header (animated SVG) | ✅ Live |
| Animated Section Dividers | ✅ Live |
| Tech Wave Dividers with floating labels | ✅ Live |
| Stats Grid with animated counters | ✅ Live |
| Skill Radar Chart (12-axis, morphing) | ✅ Live |
| Live Code Typing Animation | ✅ Live |
| Multi-layer Particle Background | ✅ Live |
| Floating Badge System | ✅ Live |
| Featured Projects Table | ✅ Updated |
| Typewriter Tagline | ✅ New |
| Skillicons Tech Stack | ✅ Live |
| GitHub Stats / Streak / Top Languages | ✅ Live |
| Contribution Activity Graph | ✅ Live |
| WakaTime Stats | ✅ Live |
| Visitor Map Badge | ✅ Live |
| Connect Buttons | ✅ Live |
| Support Buttons (Sponsors, Ko-fi) | ✅ Live |

## ⚙️ Dynamic Elements Requiring Setup

### 1. Contribution Snake Animation 🐍
**File:** `.github/workflows/snake.yml` (already created)

**To activate:**
1. Go to your repo → **Settings** → **Actions** → **General**
2. Under "Workflow permissions" → Select **"Read and write permissions"**
3. Save
4. Go to **Actions** tab → "Generate Snake Animation" → **Run workflow**
5. Wait for completion → The SVG will appear at `output/github-contribution-grid-snake.svg`
6. The README already references: `https://raw.githubusercontent.com/lyndon18-star/lyndon18-star/output/github-contribution-grid-snake.svg`

> **Note:** The workflow uses `outputs: dist/` but the README references `output/`. Either:
> - Change workflow `outputs:` to `output/`, OR
> - Update README to `dist/github-contribution-grid-snake.svg`

### 2. WakaTime Coding Activity 📊
**Current:** Shows in README but needs WakaTime account

**To activate:**
1. Sign up at [wakatime.com](https://wakatime.com)
2. Install WakaTime plugin for your editor (VS Code, JetBrains, etc.)
3. Get your **API Key** from [wakatime.com/settings](https://wakatime.com/settings)
4. Go to repo → **Settings** → **Secrets and variables** → **Actions** → **New repository secret**
   - Name: `WAKATIME_API_KEY`
   - Value: Your API key
5. The badge will auto-populate within 24 hours

### 3. Visitor Map 🌍
**Current:** Uses `visitor-badge.laobi.icu` (free, no setup needed)

**Optional - Better alternative (requires setup):**
1. Go to [github-profile-views](https://github.com/antonkomarev/github-profile-views)
2. Or use [visitor-badge.glitch.me](https://visitor-badge.glitch.me) with custom config

### 4. GitHub Stats Theme Customization
Current theme: `tokyonight` with custom purple colors matching the profile theme

**Color params used:**
- `bg_color=0F0A1A` (Deep Space)
- `title_color=A855F7` (Vibrant Violet)
- `text_color=E2E8F0` (Primary Text)
- `icon_color=C026D3` (Magenta)
- `border_color=3D2A5C` (Border Purple)

## 🎨 Custom SVG Assets (All in `/assets/`)

| Asset | Dimensions | Description |
|-------|------------|-------------|
| `hero-header.svg` | 1200×180 | Animated identity header with entrance fade, stronger glow-pulse orbs/rings, ambient code accents |
| `typewriter-tagline-purple.svg` | 600×32 | Character-by-character typewriter reveal of "Code should be useful, expressive, and a little bit magical" |
| `section-divider-purple.svg` | 1200×60 | Animated divider with pulsing diamond, circuit traces, floating particles |
| `tech-wave-purple.svg` | 1200×80 | 4-layer wave divider with entrance fade, stronger node pulses, tech labels, geometric shapes |
| `stats-grid-purple.svg` | 450×110 | Compact 2×2 stat cards with entrance fade, glow pulses, counters, progress-bar fills |
| `project-card-purple.svg` | 320×180 | Compact featured-project card (currently featuring **MUSEUM** — real stars/tech) with glow-border pulse, icon, title, animated status dot, tech pills, description, star line |
| `skill-radar-purple.svg` | 450×450 | 12-axis radar chart with morphing polygon, rotating rings, proficiency dots |
| `code-animation-purple.svg` | 700×220 | Terminal animation with 17 lines of TypeScript/React code typing sequentially |
| `arcade-game-purple.svg` | 1200×220 | Space-invaders arcade scene: stepped alien-fleet march, gliding ship, looping photon fire, falling bomb, blinking PRESS START, fake score ticker |
| `particles-purple.svg` | 1200×220 | Multi-layer particle background with 5 color gradients, floating symbols, circuit lines |
| `floating-badge-purple.svg` | 280×100 | 3 animated badges with pulsing borders, icons, floating particles |

**All animations use CSS SMIL** — compatible with GitHub README rendering (no JavaScript required).

**Cache-busting:** local asset URLs in `README.md` carry a `?v=2` query. When you edit an asset and GitHub keeps serving the old cached version, bump the version (`?v=3`) in the README.

## 🔧 Customization Checklist

### Update These with Your Info:
- [ ] Portfolio URL (currently placeholder)
- [ ] Discord invite link (currently placeholder)
- [ ] Twitter/X handle (currently placeholder)
- [ ] Project descriptions — add real descriptions to each repo
- [ ] Add screenshots/GIFs to project cards (optional but recommended) — drop images into `assets/screenshots/` and swap the pinned-card images in the README with `<img src="assets/screenshots/your-shot.png" />`

### Add to Repos (for better project cards):
For each featured repo, add:
- [ ] `description` in repo settings (shows in GitHub UI)
- [ ] `homepage` URL (live demo link)
- [ ] Topics/tags (e.g., `nextjs`, `typescript`, `portfolio`)
- [ ] README with screenshots/GIFs

### Optional Enhancements:
- [ ] Add **GitHub Sponsors** / **Ko-fi** button (already in template, just add your links)
- [ ] Add **Blog posts** section (if you write on Dev.to/Hashnode/Medium)
- [ ] Add **Certifications** / **Achievements** section
- [ ] Customize skill radar labels to match your actual focus areas

## 📁 File Structure

```
lyndon18-star/
├── README.md                    # Your profile README
├── PROFILE_SETUP.md             # This setup guide
├── assets/                      # Custom animated SVGs (purple theme)
│   ├── hero-header.svg
│   ├── typewriter-tagline-purple.svg
│   ├── section-divider-purple.svg
│   ├── tech-wave-purple.svg
│   ├── stats-grid-purple.svg
│   ├── project-card-purple.svg
│   ├── skill-radar-purple.svg
│   ├── code-animation-purple.svg
│   ├── arcade-game-purple.svg
│   ├── particles-purple.svg
│   ├── floating-badge-purple.svg
│   └── purple-theme-palette.md  # Color system documentation
├── .github/
│   └── workflows/
│       └── snake.yml            # Snake animation generator
└── output/                      # Generated by workflow (auto-created)
    ├── github-contribution-grid-snake.svg
    └── github-contribution-grid-snake-dark.svg
```

## 🚀 Quick Commands

```bash
# Trigger snake animation manually
gh workflow run snake.yml

# Check workflow status
gh run list --workflow=snake.yml

# View generated SVG locally
open dist/github-contribution-grid-snake.svg
```

## 🎨 Purple Theme Color Palette

| Color Role | Hex | Usage |
|------------|-----|-------|
| Deep Violet | `#4C1D95` | Primary actions, headers |
| Royal Purple | `#7C3AED` | Primary brand, borders |
| Vibrant Violet | `#A855F7` | Accents, glows, highlights |
| Magenta | `#C026D3` | Secondary accents, gradients |
| Pink Accent | `#F472B6` | Tertiary, playful elements |
| Electric Cyan | `#06B6D4` | Code, links, technical |
| Bright Cyan | `#22D3EE` | Highlights, data viz |
| Teal Green | `#14B8A6` | Success, growth indicators |
| Amber Gold | `#FBBF24` | Warnings, stars, energy |
| **Backgrounds** | | |
| Deep Space | `#0F0A1A` | Primary background |
| Dark Purple | `#1A0F2E` | Card backgrounds |
| Elevated Purple | `#24153B` | Elevated surfaces |
| Border Purple | `#3D2A5C` | Subtle borders, dividers |
| **Text** | | |
| Muted Text | `#94A3B8` | Secondary text |
| Primary Text | `#E2E8F0` | Main content |
| Bright Text | `#F8FAFC` | Headlines, emphasis |

See `assets/purple-theme-palette.md` for complete documentation including gradients, shadows, spacing, and z-index system.

## 🔗 Useful References

- [GitHub Profile README Guide](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme)
- [Shields.io Badge Docs](https://shields.io/)
- [Skillicons](https://skillicons.dev/)
- [GitHub Readme Stats](https://github.com/anuraghazra/github-readme-stats)
- [Streak Stats](https://github.com/DenverCoder1/github-readme-streak-stats)
- [GitHub Profile Trophy](https://github.com/ryo-ma/github-profile-trophy)
- [Snake Animation](https://github.com/Platane/snk)
- [SVG SMIL Animation Guide](https://developer.mozilla.org/en-US/docs/Web/SVG/SVG_animation_with_SMIL)

---

**Need help?** Open an issue in this repo or DM me on Discord! 💜