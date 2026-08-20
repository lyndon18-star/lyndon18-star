# Purple Theme Color Palette

## Core Purple Spectrum

| Role | Hex | HSL | Usage |
|------|-----|-----|-------|
| **Primary Deep** | `#0F0A1A` | 260° 40% 7% | Darkest background, near-black base |
| **Primary Base** | `#1A0F2E` | 270° 50% 12% | Card backgrounds, primary surface |
| **Primary Elevated** | `#24153B` | 270° 45% 15% | Hover states, elevated surfaces |
| **Primary Border** | `#3D2A5C` | 270° 35% 27% | Borders, subtle dividers |

## Violet Accents (Primary Brand)

| Role | Hex | HSL | Usage |
|------|-----|-----|-------|
| **Violet 600** | `#7C3AED` | 262° 83% 58% | Primary brand, main CTAs, active states |
| **Violet 500** | `#A855F7` | 262° 83% 66% | Hover states, primary highlights |
| **Violet 400** | `#C084FC` | 262° 83% 74% | Glows, particle effects, subtle accents |
| **Violet 300** | `#D8B4FE` | 262° 83% 82% | Light accents, disabled states |

## Magenta/Pink Accents (Secondary)

| Role | Hex | HSL | Usage |
|------|-----|-----|-------|
| **Magenta 600** | `#C026D3` | 287° 77% 49% | Secondary actions, gradient stops |
| **Magenta 500** | `#D946EF` | 287° 77% 57% | Hover states, emphasis |
| **Magenta 400** | `#E879F9` | 287° 77% 66% | Gradient highlights, particle variety |

## Cyan/Teal Accents (Tertiary - Tech Feel)

| Role | Hex | HSL | Usage |
|------|-----|-----|-------|
| **Cyan 500** | `#06B6D4` | 189° 94% 43% | Code syntax, tech highlights, data viz |
| **Cyan 400** | `#22D3EE` | 189° 94% 51% | Glows, connection lines, hover |
| **Teal 500** | `#14B8A6` | 173° 80% 40% | Success states, completed items |

## Semantic Colors

| Role | Hex | Usage |
|------|-----|-------|
| **Success** | `#22C55E` | Completed, online, positive metrics |
| **Warning** | `#FBBF24` | In progress, pending, attention |
| **Error** | `#EF4444` | Failed, offline, critical alerts |
| **Info** | `#38BDF8` | Neutral info, links, secondary text |

## Text Colors

| Role | Hex | Usage |
|------|-----|-------|
| **Primary** | `#F8FAFC` | Headlines, primary content |
| **Secondary** | `#CBD5E1` | Body text, descriptions |
| **Muted** | `#94A3B8` | Captions, labels, metadata |
| **Subtle** | `#64748B` | Placeholders, disabled text |
| **Inverse** | `#0F0A1A` | Text on light backgrounds |

## Gradient Definitions

### Primary Brand Gradient
```css
linear-gradient(135deg, #7C3AED 0%, #A855F7 50%, #C026D3 100%)
```

### Hero Background Gradient
```css
radial-gradient(ellipse at center, #1A0F2E 0%, #0F0A1A 70%)
```

### Card Gradient
```css
linear-gradient(145deg, #1A0F2E 0%, #24153B 100%)
```

### Glow Gradient (for particles/accents)
```css
radial-gradient(circle at center, #A855F7 0%, transparent 70%)
```

### Cyan-Tech Gradient
```css
linear-gradient(90deg, #06B6D4 0%, #22D3EE 100%)
```

### Sunset Gradient (warm accent)
```css
linear-gradient(135deg, #C026D3 0%, #F472B6 50%, #FBBF24 100%)
```

### Deep Space Gradient (footer/sections)
```css
linear-gradient(180deg, #0F0A1A 0%, #1A0F2E 50%, #0F0A1A 100%)
```

## Animation Timing Standards

| Animation Type | Duration | Easing |
|----------------|----------|--------|
| **Micro** (hover, tap) | 150-200ms | ease-out |
| **Standard** (transitions) | 300-400ms | ease-in-out |
| **Macro** (section enter) | 600-800ms | ease-out |
| **Ambient** (floating, pulse) | 3-6s | linear |
| **Stagger** (list items) | 80-120ms delay | ease-out |

## Shadow System

```css
/* Subtle elevation */
box-shadow: 0 1px 3px rgba(124, 58, 237, 0.1), 0 1px 2px rgba(0,0,0,0.3);

/* Medium elevation */
box-shadow: 0 4px 12px rgba(124, 58, 237, 0.15), 0 2px 6px rgba(0,0,0,0.4);

/* High elevation (modals, dropdowns) */
box-shadow: 0 12px 32px rgba(124, 58, 237, 0.2), 0 8px 16px rgba(0,0,0,0.5);

/* Glow shadows */
box-shadow: 0 0 20px rgba(168, 85, 247, 0.3), 0 0 40px rgba(124, 58, 237, 0.15);
```

## Border Radius Scale

| Size | Value | Usage |
|------|-------|-------|
| **xs** | 4px | Badges, small chips |
| **sm** | 8px | Buttons, inputs, cards |
| **md** | 12px | Standard cards, panels |
| **lg** | 16px | Large cards, hero sections |
| **xl** | 24px | Major containers, modals |
| **full** | 9999px | Pills, avatars, badges |

## Spacing Scale (8pt base)

| Token | Value |
|-------|-------|
| space-1 | 4px |
| space-2 | 8px |
| space-3 | 12px |
| space-4 | 16px |
| space-5 | 20px |
| space-6 | 24px |
| space-8 | 32px |
| space-10 | 40px |
| space-12 | 48px |
| space-16 | 64px |

## Z-Index Scale

| Layer | Value |
|-------|-------|
| Base | 0 |
| Dropdown | 10 |
| Sticky | 20 |
| Modal Backdrop | 30 |
| Modal | 40 |
| Popover | 50 |
| Tooltip | 60 |
| Toast | 70 |