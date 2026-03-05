# Theme Variants

This directory contains design tokens for multiple VS Code themes converted to web design systems.

## Available Themes

### 1. Synthwave '84 (Original)

**Path:** `../` (parent directory)

The original Synthwave '84 theme by @robb0wen with neon colors and glow effects.

### 2. Synesthesia

**Path:** `./synesthesia/`

4 dark themes inspired by synesthesia and 80s retrofuturism with music-themed color names.

- **Colors:** Neon pinks, mints, purples, blues
- **Style:** Ultra-colorful, hyper-legible
- **Font:** JetBrains Mono, Fira Code
- **Special:** Musical color names (forte, crescendo, legato...)

### 3. Min Darker

**Path:** `./min-darker/`

A minimal dark theme with low contrast and clean aesthetics.

- **Colors:** Dark grays, subtle accents
- **Style:** Minimal, low contrast
- **Font:** Fira Code
- **Special:** No neon effects, pure minimalism

## Usage

Each theme folder contains:
- `colors.json` — Color palette
- `typography.json` — Fonts, sizes, weights
- `spacing.json` — Spacing scale (4px base)
- `borders.json` — Border radii and widths
- `shadows.json` — Shadows and glow effects (where applicable)
- `effects.json` — Transitions and animations
- `index.json` — Combined export
- `README.md` — Theme documentation

## Structure

```
design-tokens/
├── colors.json          # Synthwave '84 colors
├── typography.json      # Synthwave '84 typography
├── ...                  # Other Synthwave '84 tokens
├── index.json           # Synthwave '84 index
├── README.md            # Synthwave '84 docs
└── themes/
    ├── synesthesia/     # Synesthesia theme tokens
    ├── min-darker/      # Min Darker theme tokens
    └── README.md        # This file
```
