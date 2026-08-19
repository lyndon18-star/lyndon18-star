# Profile Assets

This folder contains all custom SVG assets for the GitHub profile README.

## Files

| File | Description | Used In |
|------|-------------|---------|
| `mascot.svg` | Custom "Code Cat" mascot with circuit tail, animated eyes, floating code particles | Hero section, project cards, footer |
| `divider-wave.svg` | Animated wave divider with pulsing center node | Section dividers |
| `section-divider.svg` | Minimal line divider with pulsing center dot | Between major sections |
| `header-accent.svg` | Dual circuit lines with expanding pulse rings | Header accent below avatar |

## Usage in README

Since GitHub README renders inline SVG directly, these files serve as:
1. **Reference source** — Easy to edit and maintain
2. **Embeddable** — Can be referenced via raw GitHub URL if needed
3. **Version controlled** — Track changes to visual identity

## Embedding Options

### Option 1: Inline (Current - Recommended)
Copy SVG content directly into README.md. Renders immediately, no external requests.

### Option 2: Raw GitHub URL
```markdown
![Mascot](https://raw.githubusercontent.com/lyndon18-star/lyndon18-star/main/assets/mascot.svg)
```
**Pros:** Single source of truth, easy updates
**Cons:** Extra HTTP request, may be blocked by some viewers

### Option 3: GitHub User Content (Profile-specific)
```markdown
![Mascot](https://github.com/lyndon18-star/lyndon18-star/raw/main/assets/mascot.svg)
```

## Color Palette (CSS Variables for Reference)

```css
:root {
  --navy-900: #0B1220;      /* Primary dark */
  --navy-800: #161B22;      /* Card backgrounds */
  --navy-700: #1E293B;      /* Borders */
  --cyan-400: #38BDF8;      /* Primary accent */
  --cyan-500: #0EA5E9;      /* Hover accent */
  --emerald-500: #22C55E;   /* Success/available */
  --amber-400: #FBBF24;     /* Learning/warning */
  --violet-400: #A78BFA;    /* Learning/purple */
  --pink-400: #F472B6;      /* Fun accents */
}
```

## Animation Guidelines

All SVGs use **CSS SMIL animations** (`<animate>`) which:
- ✅ Work in GitHub README (no JS allowed)
- ✅ Loop infinitely
- ✅ Respect `prefers-reduced-motion` (browser handles it)
- ✅ Lightweight (no external dependencies)

**Timing:** All animations use 2s duration for consistency
**Easing:** Linear (default) for mechanical feel

## Updating Assets

1. Edit the `.svg` file in this folder
2. Copy the updated content to README.md (if inlined)
3. Commit & push — changes reflect immediately on profile

## Adding New Assets

1. Create new `.svg` in this folder
2. Follow naming: `kebab-case-purpose.svg`
3. Use the established color palette
4. Add entry to this table
5. Embed in README where needed