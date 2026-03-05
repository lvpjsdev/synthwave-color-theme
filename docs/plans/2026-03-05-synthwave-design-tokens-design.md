# Synthwave Web Design Tokens

## Overview

Design system for web based on Synthwave '84 VS Code theme. JSON-based tokens for maximum portability and automation potential.

## Structure

```
design-tokens/
├── colors.json          — color palette + semantic colors
├── typography.json      — fonts, sizes, weights, line-height
├── spacing.json         — margins, paddings, gaps
├── borders.json         — radii, border widths
├── shadows.json         — shadows + neon glow effects
├── effects.json         — animations, transitions, filters
└── index.json           — combined export
```

## Color Palette

### Backgrounds (Dark Purple Base)
| Token | HEX | Usage |
|-------|-----|-------|
| `bg-primary` | `#262335` | Main background |
| `bg-secondary` | `#241b2f` | Sidebar, panels |
| `bg-tertiary` | `#171520` | Activity bar, deepest |
| `bg-elevated` | `#2a2139` | Cards, modals |
| `bg-hover` | `#ffffff20` | Hover overlay (white 12%) |

### Neon Colors
| Token | HEX | Usage |
|-------|-----|-------|
| `neon-pink` | `#ff7edb` | Primary accent, variables |
| `neon-cyan` | `#36f9f6` | Functions, links |
| `neon-yellow` | `#fede5d` | Keywords, operators |
| `neon-green` | `#72f1b8` | Success, tags |
| `neon-orange` | `#ff8b39` | Strings |
| `neon-red` | `#fe4450` | Errors, important |
| `neon-coral` | `#f97e72` | Constants, numbers |

### Foreground
| Token | HEX | Usage |
|-------|-----|-------|
| `fg-primary` | `#ffffff` | Main text |
| `fg-secondary` | `#ffffff99` | Muted text (60% opacity) |
| `fg-tertiary` | `#ffffff73` | Disabled, hints (45% opacity) |
| `fg-comment` | `#848bbd` | Comments |

### Semantic Colors
| Token | Color | Usage |
|-------|-------|-------|
| `semantic-success` | `neon-green` | Success states |
| `semantic-warning` | `neon-yellow` | Warnings |
| `semantic-error` | `neon-red` | Errors |
| `semantic-info` | `neon-cyan` | Info states |

## Typography

### Font Families
- **Display:** `Orbitron` — retro-futuristic headings
- **Mono:** `Fira Code` — code, technical content
- **Body:** `Inter` / `Fira Sans` — UI text

### Font Sizes
| Token | Size | Usage |
|-------|------|-------|
| `xs` | 12px | Captions, labels |
| `sm` | 14px | Small text |
| `md` | 16px | Body text |
| `lg` | 18px | Large body |
| `xl` | 20px | Subheadings |
| `2xl` | 24px | Headings |
| `3xl` | 32px | Large headings |
| `4xl` | 48px | Display |
| `5xl` | 64px | Hero |

### Font Weights
- `regular`: 400
- `medium`: 500
- `semibold`: 600
- `bold`: 700

## Spacing

Base unit: `4px` (0.25rem)

| Token | Value |
|-------|-------|
| `0` | 0 |
| `1` | 4px |
| `2` | 8px |
| `3` | 12px |
| `4` | 16px |
| `5` | 20px |
| `6` | 24px |
| `8` | 32px |
| `10` | 40px |
| `12` | 48px |
| `16` | 64px |
| `20` | 80px |
| `24` | 96px |

## Borders

### Border Radius
| Token | Value |
|-------|-------|
| `none` | 0 |
| `sm` | 4px |
| `md` | 8px |
| `lg` | 12px |
| `xl` | 16px |
| `2xl` | 24px |
| `full` | 9999px |

### Border Widths
- `thin`: 1px
- `medium`: 2px
- `thick`: 4px

## Shadows

### Standard Shadows
| Token | Value |
|-------|-------|
| `sm` | `0 1px 2px rgba(0,0,0,0.3)` |
| `md` | `0 4px 6px rgba(0,0,0,0.3)` |
| `lg` | `0 10px 15px rgba(0,0,0,0.4)` |
| `xl` | `0 20px 25px rgba(0,0,0,0.5)` |

### Neon Glow Effects (Optional)
| Token | Value |
|-------|-------|
| `glow-pink` | `0 0 10px #ff7edb, 0 0 20px #ff7edb80, 0 0 30px #ff7edb40` |
| `glow-cyan` | `0 0 10px #36f9f6, 0 0 20px #36f9f680, 0 0 30px #36f9f640` |
| `glow-yellow` | `0 0 10px #fede5d, 0 0 20px #fede5d80, 0 0 30px #fede5d40` |
| `glow-green` | `0 0 10px #72f1b8, 0 0 20px #72f1b880, 0 0 30px #72f1b840` |
| `glow-red` | `0 0 10px #fe4450, 0 0 20px #fe445080, 0 0 30px #fe445040` |

### Text Glow Effects
| Token | Value |
|-------|-------|
| `text-glow-pink` | `0 0 10px #ff7edb` |
| `text-glow-cyan` | `0 0 10px #36f9f6` |
| `text-glow-yellow` | `0 0 10px #fede5d` |
| `text-glow-green` | `0 0 10px #72f1b8` |

## Effects

### Transitions
| Token | Value |
|-------|-------|
| `fast` | `150ms ease` |
| `normal` | `250ms ease` |
| `slow` | `400ms ease` |
| `glow` | `300ms ease-out` |

### Animations
- `pulse-glow` — pulsing neon effect
- `flicker` — subtle CRT flicker
- `scanline` — retro scanline overlay

## Open Questions

> Questions to revisit later if needed

- [ ] Add gradients as tokens?
- [ ] Include dark/light mode switching?
- [ ] Add accessibility contrast ratios?
- [ ] Generate CSS/SCSS/Tailwind from tokens automatically?
