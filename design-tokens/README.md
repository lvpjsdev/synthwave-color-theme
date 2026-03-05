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
