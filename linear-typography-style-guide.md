# Linear Typography Style Guide
> Extracted directly from linear.app CSS source — `/_next/static/css/3815d844e4bc9875.css`
> Base font size: 16px (browser default, `html { font-size: 100% }`)

---

## Font Families

| Token | Stack |
|-------|-------|
| `--font-regular` | **Inter Variable**, SF Pro Display, -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Oxygen, Ubuntu, Cantarell, Open Sans, Helvetica Neue, sans-serif |
| `--font-serif-display` | **Tiempos Headline**, ui-serif, Georgia, Cambria, Times New Roman, Times, serif |
| `--font-monospace` | **Berkeley Mono**, ui-monospace, SF Mono, Menlo, monospace |
| `--font-emoji` | Apple Color Emoji, Segoe UI Emoji, Segoe UI Symbol, Segoe UI, Twemoji Mozilla, Noto Color Emoji, Android Emoji |

**Font loading:** Inter Variable loaded as `.woff2` from `https://static.linear.app/fonts/InterVariable.woff2?v=4.1`.
Font feature settings: `"cv01", "ss03"`. Font variation settings: `"opsz" auto`.

---

## Font Weights

Variable font axis values — require **Inter Variable** (not standard Inter).

| Token | Value | Name |
|-------|-------|------|
| `--font-weight-light` | `300` | Light |
| `--font-weight-normal` | `400` | Regular |
| `--font-weight-medium` | `510` | Medium |
| `--font-weight-semibold` | `590` | Semibold |
| `--font-weight-bold` | `680` | Bold |

> **Figma:** Manually type `510`, `590`, `680` in the weight field when Inter Variable is selected.
> Standard Inter only supports 400 and 700.

---

## Title Scale

All titles: **Inter Variable**, weight `590` (semibold).

| Token | rem | px | Line Height | Letter Spacing |
|-------|-----|----|-------------|----------------|
| `--title-1` | `1.0625rem` | **17px** | `1.4` | `-0.012em` / `-1.2%` |
| `--title-2` | `1.25rem` | **20px** | `1.33` | `-0.012em` / `-1.2%` |
| `--title-3` | `1.5rem` | **24px** | `1.33` | `-0.012em` / `-1.2%` |
| `--title-4` | `2rem` | **32px** | `1.125` | `-0.022em` / `-2.2%` |
| `--title-5` | `2.5rem` | **40px** | `1.1` | `-0.022em` / `-2.2%` |
| `--title-6` | `3rem` | **48px** | `1.0` | `-0.022em` / `-2.2%` |
| `--title-7` | `3.5rem` | **56px** | `1.1` | `-0.022em` / `-2.2%` |
| `--title-8` | `4rem` | **64px** | `1.06` | `-0.022em` / `-2.2%` |
| `--title-9` | `4.5rem` | **72px** | `1.0` | `-0.022em` / `-2.2%` |

**Pattern:** Title 1-3 use `-0.012em` tracking. Title 4-9 jump to `-0.022em` (tighter) as sizes grow to display scale.

---

## Text (Body) Scale

All text: **Inter Variable**, weight `400` (normal).

| Token | rem | px | Line Height | Letter Spacing |
|-------|-----|----|-------------|----------------|
| `--text-large` | `1.0625rem` | **17px** | `1.6` | `0` |
| `--text-regular` | `0.9375rem` | **15px** | `1.6` | `-0.011em` / `-1.1%` |
| `--text-small` | `0.875rem` | **14px** | `1.5` | `-0.013em` / `-1.3%` |
| `--text-mini` | `0.8125rem` | **13px** | `1.5` | `-0.01em` / `-1.0%` |
| `--text-micro` | `0.75rem` | **12px** | `1.4` | `0` |
| `--text-tiny` | `0.625rem` | **10px** | `1.5` | `-0.015em` / `-1.5%` |

---

## Legacy Font Size Tokens

Older scale still in codebase alongside the title/text system above.

| Token | rem | px |
|-------|-----|----|
| `--font-size-micro` | `0.6875rem` | 11px |
| `--font-size-mini` | `0.75rem` | 12px |
| `--font-size-small` | `0.8125rem` | 13px |
| `--font-size-regular` | `0.9375rem` | 15px |
| `--font-size-large` | `1.125rem` | 18px |
| `--font-size-title3` | `1.25rem` | 20px |
| `--font-size-title2` | `1.5rem` | 24px |
| `--font-size-title1` | `2.25rem` | 36px |

---

## Text Color Tokens

### Dark Theme (`[data-theme=dark]`)

| Token | Hex | Usage |
|-------|-----|-------|
| `--color-text-primary` | `#f7f8f8` | Primary body text |
| `--color-text-secondary` | `#d0d6e0` | Subtitles, secondary text |
| `--color-text-tertiary` | `#8a8f98` | Muted text, placeholders |
| `--color-text-quaternary` | `#62666d` | Disabled, hints |
| `--color-link-primary` | `#828fff` | Links |
| `--color-link-hover` | `#ffffff` | Link hover |

### Light Theme (`[data-theme=light]`)

| Token | Hex | Usage |
|-------|-----|-------|
| `--color-text-primary` | `#282a30` | Primary body text |
| `--color-text-secondary` | `#3c4149` | Subtitles, secondary text |
| `--color-text-tertiary` | `#6f6e77` | Muted text, placeholders |
| `--color-text-quaternary` | `#86848d` | Disabled, hints |
| `--color-link-primary` | `#7070ff` | Links |
| `--color-link-hover` | `#282a30` | Link hover (matches primary) |

### Glass Theme (`[data-theme=glass]` — dark marketing pages)

| Token | Value | Usage |
|-------|-------|-------|
| `--color-text-primary` | `#f7f8f8` | Primary body text |
| `--color-text-secondary` | `#b4bcd0` | Secondary text |
| `--color-text-tertiary` | `#b4bcd099` | Muted (~60% opacity on #b4bcd0) |
| `--color-text-quaternary` | `#b4bcd066` | Hint (~40% opacity on #b4bcd0) |

---

## Brand / Accent Colors

| Token | Dark | Light | Usage |
|-------|------|-------|-------|
| `--color-brand-bg` | `#5e6ad2` | `#7070ff` | Brand accent, CTA buttons |
| `--color-accent` | `#7170ff` | `#7170ff` | Interactive accent |
| `--color-accent-hover` | `#828fff` | `#8989f0` | Hover state |

---

## Typography Combinations (Observed In-Use)

### Marketing Hero (Title 7-9)
```
Font:           Inter Variable
Weight:         590 (semibold)
Size:           56–72px (title-7 to title-9)
Line height:    1.0–1.1
Letter spacing: -2.2%
Color:          text-primary
```

### Section Heading (Title 4-6)
```
Font:           Inter Variable
Weight:         590 (semibold)
Size:           32–48px (title-4 to title-6)
Line height:    1.0–1.125
Letter spacing: -2.2%
Color:          text-primary
```

### UI Heading / Card Title (Title 1-3)
```
Font:           Inter Variable
Weight:         590 (semibold)
Size:           17–24px (title-1 to title-3)
Line height:    1.33–1.4
Letter spacing: -1.2%
Color:          text-primary
```

### Body / Paragraph (Default)
```
Font:           Inter Variable
Weight:         400 (normal)
Size:           15px (text-regular)
Line height:    1.6
Letter spacing: -1.1%
Color:          text-primary
```

### Lead Paragraph
```
Font:           Inter Variable
Weight:         400 (normal)
Size:           17px (text-large)
Line height:    1.6
Letter spacing: 0%
Color:          text-secondary
```

### Small / Description
```
Font:           Inter Variable
Weight:         400 (normal)
Size:           14px (text-small)
Line height:    1.5
Letter spacing: -1.3%
Color:          text-secondary or text-tertiary
```

### Label / Caption
```
Font:           Inter Variable
Weight:         400–510 (normal to medium)
Size:           10–13px (text-tiny to text-mini)
Line height:    1.4–1.5
Color:          text-tertiary
```

### Code
```
Font:           Berkeley Mono, ui-monospace, SF Mono, Menlo
Size:           0.875em (relative to parent)
Background:     none (inline code has no background)
```

---

## Underline Tokens

| Token | Value | Resolves to |
|-------|-------|-------------|
| `--underline-thickness` | `clamp(1px, 0.0625em, 3px)` | 1–3px based on font size |
| `--underline-offset` | `clamp(2px, 0.225em, 6px)` | 2–6px based on font size |

---

## Figma Import Checklist

### Fonts to install
- [ ] **Inter Variable** — Google Fonts (free) or rsms.me/inter
- [ ] **Berkeley Mono** — berkeleygraphics.com (commercial) for code styles
- [ ] **Tiempos Headline** — klim.co.nz (commercial) for serif display moments

### Text Styles to create (18 total)
- [ ] `Title/9` — 72px / weight 590 / leading 1.0 / tracking -2.2%
- [ ] `Title/8` — 64px / weight 590 / leading 1.06 / tracking -2.2%
- [ ] `Title/7` — 56px / weight 590 / leading 1.1 / tracking -2.2%
- [ ] `Title/6` — 48px / weight 590 / leading 1.0 / tracking -2.2%
- [ ] `Title/5` — 40px / weight 590 / leading 1.1 / tracking -2.2%
- [ ] `Title/4` — 32px / weight 590 / leading 1.125 / tracking -2.2%
- [ ] `Title/3` — 24px / weight 590 / leading 1.33 / tracking -1.2%
- [ ] `Title/2` — 20px / weight 590 / leading 1.33 / tracking -1.2%
- [ ] `Title/1` — 17px / weight 590 / leading 1.4 / tracking -1.2%
- [ ] `Text/Large` — 17px / weight 400 / leading 1.6 / tracking 0%
- [ ] `Text/Regular` — 15px / weight 400 / leading 1.6 / tracking -1.1%
- [ ] `Text/Small` — 14px / weight 400 / leading 1.5 / tracking -1.3%
- [ ] `Text/Mini` — 13px / weight 400 / leading 1.5 / tracking -1.0%
- [ ] `Text/Micro` — 12px / weight 400 / leading 1.4 / tracking 0%
- [ ] `Text/Tiny` — 10px / weight 400 / leading 1.5 / tracking -1.5%
- [ ] `Code/Regular` — 14px / Berkeley Mono / leading 1.5
- [ ] `Display/Serif` — Tiempos Headline / weight 400 / for editorial moments

### Color Styles to create
- [ ] `Text/Dark/Primary` — `#f7f8f8`
- [ ] `Text/Dark/Secondary` — `#d0d6e0`
- [ ] `Text/Dark/Tertiary` — `#8a8f98`
- [ ] `Text/Dark/Quaternary` — `#62666d`
- [ ] `Text/Light/Primary` — `#282a30`
- [ ] `Text/Light/Secondary` — `#3c4149`
- [ ] `Text/Light/Tertiary` — `#6f6e77`
- [ ] `Text/Light/Quaternary` — `#86848d`
- [ ] `Link/Dark` — `#828fff`
- [ ] `Link/Light` — `#7070ff`
- [ ] `Brand/Dark` — `#5e6ad2`
- [ ] `Brand/Light` — `#7070ff`

### Letter spacing conversion (em to Figma %)
Figma uses `%` not `em`. Multiply the em value by 100:
- `-0.022em` → **-2.2%**
- `-0.015em` → **-1.5%**
- `-0.013em` → **-1.3%**
- `-0.012em` → **-1.2%**
- `-0.011em` → **-1.1%**
- `-0.01em` → **-1.0%**
- `0` → **0%**

### Line height in Figma
Set as **Auto** for `1.0`, or use pixel values:
- `1.6` at 15px → 24px
- `1.6` at 17px → 27.2px (round to 27px)
- `1.5` at 14px → 21px
- `1.4` at 17px → 23.8px (round to 24px)
- `1.33` at 20px → 26.6px (round to 27px)
- `1.33` at 24px → 31.9px (round to 32px)
- `1.125` at 32px → 36px
- `1.1` at 40px → 44px
- `1.1` at 56px → 61.6px (round to 62px)
- `1.06` at 64px → 67.8px (round to 68px)
- `1.0` at 48px → 48px
- `1.0` at 72px → 72px
