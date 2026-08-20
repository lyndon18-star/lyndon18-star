# Profile Assets

This folder contains all custom SVG assets for the GitHub profile README (purple theme v2.0).

## Active Assets (Referenced in README)

| File | Dimensions | Description | Used In |
|------|------------|-------------|---------|
| `hero-header.svg` | 1200×280 | Animated identity badge with hexagon core, orbiting particles, circuit lines, floating code brackets | Top of README |
| `section-divider-purple.svg` | 1200×80 | Animated divider with pulsing diamond, circuit traces, floating particles | Between all major sections |
| `tech-wave-purple.svg` | 1200×140 | 4-layer wave divider with tech labels, pulsing nodes, geometric shapes | Section transitions |
| `stats-grid-purple.svg` | 900×200 | 4 animated stat cards with glowing borders, counters, progress bars | GitHub Analytics section |
| `skill-radar-purple.svg` | 450×450 | 12-axis radar chart with morphing polygon, rotating rings, proficiency dots | Skill Radar section |
| `code-animation-purple.svg` | 700×220 | Terminal animation with 17 lines of TypeScript/React code typing sequentially | Live Coding section |
| `particles-purple.svg` | 1200×220 | Multi-layer particle background with 5 color gradients, floating symbols | Visitor Map section |
| `floating-badge-purple.svg` | 280×100 | 3 animated badges with pulsing borders, icons, floating particles | About & Connect sections |

## Legacy Assets (Deprecated - Not Used)

| File | Reason for Deprecation |
|------|----------------------|
| `mascot.svg` | Replaced by hero-header.svg (better design, no profile picture needed) |
| `divider-wave.svg` | Replaced by tech-wave-purple.svg (richer animation) |
| `section-divider.svg` | Replaced by section-divider-purple.svg (purple theme) |
| `header-accent.svg` | Merged into hero-header.svg |
| `particles-bg.svg` | Replaced by particles-purple.svg (multi-layer, 5 colors) |
| `skill-radar.svg` | Replaced by skill-radar-purple.svg (12-axis, morphing) |
| `code-animation.svg` | Replaced by code-animation-purple.svg (purple theme) |
| `stats-counters.svg` | Replaced by stats-grid-purple.svg (cards layout) |
| `floating-badge.svg` | Replaced by floating-badge-purple.svg (purple theme) |
| `tech-wave.svg` | Replaced by tech-wave-purple.svg (purple theme) |

> **Note:** Legacy assets are kept for reference only. The README no longer references them. Safe to delete if you want a clean repo.

## Color Palette (CSS Variables)

```css
:root {
  /* Primary Brand */
  --deep-violet: #4C1D95;
  --royal-purple: #7C3AED;
  --vibrant-violet: #A855F7;
  --magenta: #C026D3;
  --pink-accent: #F472B6;

  /* Technical Accents */
  --electric-cyan: #06B6D4;
  --bright-cyan: #22D3EE;
  --teal-green: #14B8A6;
  --amber-gold: #FBBF24;

  /* Backgrounds */
  --deep-space: #0F0A1A;
  --dark-purple: #1A0F2E;
  --elevated-purple: #24153B;
  --border-purple: #3D2A5C;

  /* Text */
  --muted-text: #94A3B8;
  --primary-text: #E2E8F0;
  --bright-text: #F8FAFC;
}
```

See `purple-theme-palette.md` for complete documentation including gradients, shadows, spacing, and z-index system.

## Animation Guidelines

All SVGs use **CSS SMIL animations** (`<animate>`) which:
- ✅ Work in GitHub README (no JS allowed)
- ✅ Loop infinitely
- ✅ Respect `prefers-reduced-motion` (browser handles it)
- ✅ Lightweight (no external dependencies)

**Timing:** Consistent 2-6s durations for ambient loops, ease-in-out for transitions
**Easing:** Linear for mechanical feel, ease-in-out for organic movement

## Updating Assets

1. Edit the `.svg` file in this folder
2. Commit & push — changes reflect immediately on profile
3. For color updates, refer to `purple-theme-palette.md` for token values

## Adding New Assets

1. Create new `.svg` in this folder
2. Follow naming: `kebab-case-purpose.svg`
3. Use the established purple color palette
4. Add entry to this table
5. Embed in README where needed

See `PROFILE_SETUP.md` for the full setup guide.