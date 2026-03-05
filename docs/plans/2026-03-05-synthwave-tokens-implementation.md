# Synthwave Design Tokens Implementation Plan

> **For Claude:** REQUIRED SUB-SKILL: Use superpowers:executing-plans to implement this plan task-by-task.

**Goal:** Create complete JSON design tokens for Synthwave web theme

**Architecture:** JSON tokens following Style Dictionary format with `{ value, description }` structure for each token. Organized into separate files by category, combined in index.json.

**Tech Stack:** JSON, Style Dictionary compatible format

---

## Task 1: Create colors.json

**Files:**
- Create: `design-tokens/colors.json`

**Step 1: Write colors.json with full palette**

```json
{
  "color": {
    "bg": {
      "primary": { "value": "#262335", "description": "Main background" },
      "secondary": { "value": "#241b2f", "description": "Sidebar, panels" },
      "tertiary": { "value": "#171520", "description": "Activity bar, deepest layer" },
      "elevated": { "value": "#2a2139", "description": "Cards, modals, elevated surfaces" },
      "hover": { "value": "#ffffff20", "description": "Hover overlay (white 12% opacity)" }
    },
    "fg": {
      "primary": { "value": "#ffffff", "description": "Main text color" },
      "secondary": { "value": "#ffffff99", "description": "Muted text (60% opacity)" },
      "tertiary": { "value": "#ffffff73", "description": "Disabled, hints (45% opacity)" },
      "comment": { "value": "#848bbd", "description": "Comments, annotations" }
    },
    "neon": {
      "pink": { "value": "#ff7edb", "description": "Primary accent, variables" },
      "cyan": { "value": "#36f9f6", "description": "Functions, links" },
      "yellow": { "value": "#fede5d", "description": "Keywords, operators" },
      "green": { "value": "#72f1b8", "description": "Success, tags" },
      "orange": { "value": "#ff8b39", "description": "Strings" },
      "red": { "value": "#fe4450", "description": "Errors, important" },
      "coral": { "value": "#f97e72", "description": "Constants, numbers" }
    },
    "semantic": {
      "success": { "value": "{color.neon.green}", "description": "Success states" },
      "warning": { "value": "{color.neon.yellow}", "description": "Warning states" },
      "error": { "value": "{color.neon.red}", "description": "Error states" },
      "info": { "value": "{color.neon.cyan}", "description": "Info states" }
    }
  }
}
```

**Step 2: Commit**

```bash
git add design-tokens/colors.json
git commit -m "feat(tokens): add color palette tokens"
```

---

## Task 2: Create typography.json

**Files:**
- Create: `design-tokens/typography.json`

**Step 1: Write typography.json**

```json
{
  "font": {
    "family": {
      "display": { "value": "Orbitron", "description": "Retro-futuristic headings" },
      "mono": { "value": "'Fira Code', monospace", "description": "Code, technical content" },
      "body": { "value": "Inter, 'Fira Sans', sans-serif", "description": "UI text" }
    },
    "size": {
      "xs": { "value": "12px", "description": "Captions, labels" },
      "sm": { "value": "14px", "description": "Small text" },
      "md": { "value": "16px", "description": "Body text" },
      "lg": { "value": "18px", "description": "Large body" },
      "xl": { "value": "20px", "description": "Subheadings" },
      "2xl": { "value": "24px", "description": "Headings" },
      "3xl": { "value": "32px", "description": "Large headings" },
      "4xl": { "value": "48px", "description": "Display" },
      "5xl": { "value": "64px", "description": "Hero text" }
    },
    "weight": {
      "regular": { "value": "400", "description": "Normal weight" },
      "medium": { "value": "500", "description": "Medium weight" },
      "semibold": { "value": "600", "description": "Semibold weight" },
      "bold": { "value": "700", "description": "Bold weight" }
    },
    "lineHeight": {
      "tight": { "value": "1.2", "description": "Tight line height" },
      "normal": { "value": "1.5", "description": "Normal line height" },
      "relaxed": { "value": "1.75", "description": "Relaxed line height" }
    },
    "letterSpacing": {
      "tight": { "value": "-0.025em", "description": "Tight letter spacing" },
      "normal": { "value": "0", "description": "Normal letter spacing" },
      "wide": { "value": "0.025em", "description": "Wide letter spacing" },
      "wider": { "value": "0.05em", "description": "Wider letter spacing" }
    }
  }
}
```

**Step 2: Commit**

```bash
git add design-tokens/typography.json
git commit -m "feat(tokens): add typography tokens"
```

---

## Task 3: Create spacing.json

**Files:**
- Create: `design-tokens/spacing.json`

**Step 1: Write spacing.json**

```json
{
  "spacing": {
    "0": { "value": "0", "description": "No spacing" },
    "1": { "value": "4px", "description": "4px spacing" },
    "2": { "value": "8px", "description": "8px spacing" },
    "3": { "value": "12px", "description": "12px spacing" },
    "4": { "value": "16px", "description": "16px spacing" },
    "5": { "value": "20px", "description": "20px spacing" },
    "6": { "value": "24px", "description": "24px spacing" },
    "8": { "value": "32px", "description": "32px spacing" },
    "10": { "value": "40px", "description": "40px spacing" },
    "12": { "value": "48px", "description": "48px spacing" },
    "16": { "value": "64px", "description": "64px spacing" },
    "20": { "value": "80px", "description": "80px spacing" },
    "24": { "value": "96px", "description": "96px spacing" }
  }
}
```

**Step 2: Commit**

```bash
git add design-tokens/spacing.json
git commit -m "feat(tokens): add spacing tokens"
```

---

## Task 4: Create borders.json

**Files:**
- Create: `design-tokens/borders.json`

**Step 1: Write borders.json**

```json
{
  "border": {
    "radius": {
      "none": { "value": "0", "description": "No radius" },
      "sm": { "value": "4px", "description": "Small radius" },
      "md": { "value": "8px", "description": "Medium radius" },
      "lg": { "value": "12px", "description": "Large radius" },
      "xl": { "value": "16px", "description": "Extra large radius" },
      "2xl": { "value": "24px", "description": "2x large radius" },
      "full": { "value": "9999px", "description": "Full/pill radius" }
    },
    "width": {
      "thin": { "value": "1px", "description": "Thin border" },
      "medium": { "value": "2px", "description": "Medium border" },
      "thick": { "value": "4px", "description": "Thick border" }
    }
  }
}
```

**Step 2: Commit**

```bash
git add design-tokens/borders.json
git commit -m "feat(tokens): add border tokens"
```

---

## Task 5: Create shadows.json

**Files:**
- Create: `design-tokens/shadows.json`

**Step 1: Write shadows.json with standard + glow effects**

```json
{
  "shadow": {
    "sm": { "value": "0 1px 2px rgba(0,0,0,0.3)", "description": "Small shadow" },
    "md": { "value": "0 4px 6px rgba(0,0,0,0.3)", "description": "Medium shadow" },
    "lg": { "value": "0 10px 15px rgba(0,0,0,0.4)", "description": "Large shadow" },
    "xl": { "value": "0 20px 25px rgba(0,0,0,0.5)", "description": "Extra large shadow" }
  },
  "glow": {
    "pink": { "value": "0 0 10px #ff7edb, 0 0 20px rgba(255,126,219,0.5), 0 0 30px rgba(255,126,219,0.25)", "description": "Pink neon glow" },
    "cyan": { "value": "0 0 10px #36f9f6, 0 0 20px rgba(54,249,246,0.5), 0 0 30px rgba(54,249,246,0.25)", "description": "Cyan neon glow" },
    "yellow": { "value": "0 0 10px #fede5d, 0 0 20px rgba(254,222,93,0.5), 0 0 30px rgba(254,222,93,0.25)", "description": "Yellow neon glow" },
    "green": { "value": "0 0 10px #72f1b8, 0 0 20px rgba(114,241,184,0.5), 0 0 30px rgba(114,241,184,0.25)", "description": "Green neon glow" },
    "red": { "value": "0 0 10px #fe4450, 0 0 20px rgba(254,68,80,0.5), 0 0 30px rgba(254,68,80,0.25)", "description": "Red neon glow" }
  },
  "textGlow": {
    "pink": { "value": "0 0 10px #ff7edb", "description": "Pink text glow" },
    "cyan": { "value": "0 0 10px #36f9f6", "description": "Cyan text glow" },
    "yellow": { "value": "0 0 10px #fede5d", "description": "Yellow text glow" },
    "green": { "value": "0 0 10px #72f1b8", "description": "Green text glow" }
  }
}
```

**Step 2: Commit**

```bash
git add design-tokens/shadows.json
git commit -m "feat(tokens): add shadow and glow effect tokens"
```

---

## Task 6: Create effects.json

**Files:**
- Create: `design-tokens/effects.json`

**Step 1: Write effects.json with transitions and animations**

```json
{
  "transition": {
    "duration": {
      "fast": { "value": "150ms", "description": "Fast transition" },
      "normal": { "value": "250ms", "description": "Normal transition" },
      "slow": { "value": "400ms", "description": "Slow transition" }
    },
    "easing": {
      "default": { "value": "ease", "description": "Default easing" },
      "in": { "value": "ease-in", "description": "Ease in" },
      "out": { "value": "ease-out", "description": "Ease out" },
      "inOut": { "value": "ease-in-out", "description": "Ease in out" }
    }
  },
  "animation": {
    "pulseGlow": {
      "value": "pulse-glow 2s ease-in-out infinite",
      "description": "Pulsing neon glow animation"
    },
    "flicker": {
      "value": "flicker 0.15s infinite",
      "description": "Subtle CRT flicker effect"
    }
  },
  "keyframes": {
    "pulseGlow": {
      "value": "@keyframes pulse-glow { 0%, 100% { opacity: 1; } 50% { opacity: 0.7; } }",
      "description": "Pulse glow keyframes"
    },
    "flicker": {
      "value": "@keyframes flicker { 0%, 100% { opacity: 1; } 50% { opacity: 0.8; } }",
      "description": "Flicker keyframes"
    }
  },
  "filter": {
    "blur": {
      "sm": { "value": "4px", "description": "Small blur" },
      "md": { "value": "8px", "description": "Medium blur" },
      "lg": { "value": "16px", "description": "Large blur" }
    }
  }
}
```

**Step 2: Commit**

```bash
git add design-tokens/effects.json
git commit -m "feat(tokens): add effects and animation tokens"
```

---

## Task 7: Create index.json (combined export)

**Files:**
- Create: `design-tokens/index.json`

**Step 1: Write index.json that imports all tokens**

```json
{
  "$schema": "https://tr.designtokens.org/format/",
  "name": "Synthwave '84 Design Tokens",
  "version": "1.0.0",
  "description": "A complete design system inspired by Synthwave '84 VS Code theme",
  "import": [
    "./colors.json",
    "./typography.json",
    "./spacing.json",
    "./borders.json",
    "./shadows.json",
    "./effects.json"
  ]
}
```

**Step 2: Commit**

```bash
git add design-tokens/index.json
git commit -m "feat(tokens): add index with all token imports"
```

---

## Task 8: Add README for design-tokens

**Files:**
- Create: `design-tokens/README.md`

**Step 1: Write README**

```markdown
# Synthwave '84 Design Tokens

Complete design system for web based on [Synthwave '84](https://github.com/robb0wen/synthwave-vscode) VS Code theme.

## Structure

- `colors.json` — Backgrounds, foregrounds, neon colors, semantic colors
- `typography.json` — Fonts, sizes, weights, line-height
- `spacing.json` — Margins, paddings, gaps (4px base)
- `borders.json` — Radii and widths
- `shadows.json` — Standard shadows + neon glow effects
- `effects.json` — Transitions, animations, filters
- `index.json` — Combined export

## Usage

### With Style Dictionary

```js
const StyleDictionary = require('style-dictionary');

StyleDictionary.extend({
  source: ['design-tokens/**/*.json'],
  platforms: {
    css: {
      transformGroup: 'css',
      buildPath: 'build/css/',
      files: [{ destination: 'variables.css', format: 'css/variables' }]
    }
  }
}).buildAllPlatforms();
```

### Direct Import

```js
import tokens from './design-tokens/index.json';
const pinkGlow = tokens.glow.pink.value;
```

## Neon Glow Effects

All glow effects are optional. Use them for:
- Buttons and interactive elements
- Text highlights
- Focus states
- Decorative elements

## Credits

Inspired by [Synthwave '84](https://github.com/robb0wen/synthwave-vscode) by @robb0wen
```

**Step 2: Commit**

```bash
git add design-tokens/README.md
git commit -m "docs: add README for design tokens"
```

---

## Summary

| Task | File | Description |
|------|------|-------------|
| 1 | `colors.json` | Color palette |
| 2 | `typography.json` | Typography system |
| 3 | `spacing.json` | Spacing scale |
| 4 | `borders.json` | Border tokens |
| 5 | `shadows.json` | Shadows + glow |
| 6 | `effects.json` | Animations, transitions |
| 7 | `index.json` | Combined export |
| 8 | `README.md` | Documentation |
