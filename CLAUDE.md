# Defactor Design System — AI Coding Guidelines

Live styleguide: https://brand.defactor.com

You MUST follow these guidelines when building UI for any Defactor-related project. Before creating any new component, check the styleguide link above for existing patterns. Reuse first, create second.

---

## Fonts

- **Display / Headings:** `'Space Grotesk', sans-serif` — weights: 300, 400, 500, 600, 700
- **Body / UI / Data:** `'Sora', sans-serif` — weights: 300, 400, 500, 600, 700, 800
- Load from Google Fonts:
  ```
  Space+Grotesk:wght@300;400;500;600;700
  Sora:wght@300;400;500;600;700;800
  ```

## Color Palette

### Brand
| Token | Hex | Usage |
|-------|-----|-------|
| Violet | `#5A5BEB` | Primary brand, hero CTAs, active states, focus indicators |
| Violet Light | `#8182EF` | Hover states, secondary accents, active indicators |
| Emerald | `#28A66B` | Invest, yield, success, growth, pool active states |
| Gold | `#E1A325` | Community, social, engagement, premium, warning states |
| Crimson | `#D3194E` | Direct Lending, alerts, destructive actions, error states |
| Navy | `#070118` | Primary dark background, sidebar |
| White | `#FFFFFF` | Card surfaces, light backgrounds |

### Purple Scale
| Token | Hex | Usage |
|-------|-----|-------|
| Purple 900 | `#070118` | Sidebar, primary dark bg |
| Purple 800 | `#0F0A1E` | Dark surface secondary |
| Purple 700 | `#1a0a40` | Dark surface tertiary |
| Violet 600 | `#5A5BEB` | Links, focus, eyebrow labels |
| Violet 400 | `#8182EF` | Accents, highlights |

### Violet Tints
| Token | Hex | Usage |
|-------|-----|-------|
| Violet 100 | `#E8E8FC` | Info badge backgrounds, tinted surfaces |
| Violet 50 | `#F0F0FD` | Subtle tinted surfaces |

### Neutral
| Token | Hex | Usage |
|-------|-----|-------|
| Gray 900 | `#0F0A1E` | Body text |
| Gray 700 | `#3D3648` | Secondary text |
| Gray 500 | `#6B7280` | Muted labels |
| Gray 400 | `#A8ABB0` | Placeholder text |
| Gray 200 | `#D6D8DB` | Borders, dividers |
| Gray 50 | `#F8F7FE` | Page bg |
| White | `#FFFFFF` | Card surfaces |

### Semantic
| Token | Hex | Usage |
|-------|-----|-------|
| Success | `#065F46` | Active, confirmed |
| Success bg | `#D1FAE5` | Success badge background |
| Danger | `#D3194E` | Failed, destructive actions |
| Danger bg | `#FCE8EF` | Danger badge background |
| Warning | `#92400E` | Pending, caution |
| Warning bg | `#FFFBEB` | Warning badge background |

### Dark Mode (CSS custom properties)
| Token | Light | Dark |
|-------|-------|------|
| `--dm-bg` | `#F5F6F8` | `#070118` |
| `--dm-surface` | `#ffffff` | `#0F0A1E` |
| `--dm-surf2` | `#EEEEF8` | `#1a0a40` |
| `--dm-ink` | `#070118` | `#F0F0FD` |
| `--dm-muted` | `#6B7280` | `#9CA3AF` |
| `--dm-border` | `rgba(90,91,235,.12)` | `rgba(90,91,235,.18)` |
| `--dm-divider` | `#EBEBF0` | `#1a0a40` |
| `--dm-header` | `#ffffff` | `#0F0A1E` |

## Spacing

| Token | Value | Usage |
|-------|-------|-------|
| space-1 | 4px | Inline gaps, icon padding |
| space-2 | 8px | Internal component gaps |
| space-3 | 12px | Small card padding |
| space-4 | 16px | Default padding, row gap |
| space-5 | 24px | Section gap, card padding |
| space-6 | 32px | Section spacing |
| space-8 | 48px | Page horizontal padding |
| space-10 | 72px | Major section breaks |

## Border Radius

| Token | Value | Usage |
|-------|-------|-------|
| r-sm | 6px | Badges, chips |
| r-md | 8px | Inputs, buttons |
| r-lg | 12px | Cards, panels |
| r-xl | 16px | Form cards, modals |
| r-2xl | 20px | Hero strips, sections |
| r-pill | 100px | Pill buttons, avatars |

## Shadows

| Level | Value | Usage |
|-------|-------|-------|
| S1 (Resting) | `0 1px 3px rgba(7,1,24,.06), 0 2px 8px rgba(7,1,24,.06)` | Default card elevation |
| S2 (Lifted) | `0 1px 3px rgba(7,1,24,.04), 0 4px 12px rgba(7,1,24,.06), 0 8px 24px rgba(7,1,24,.05)` | Hover lift, active cards |
| S3 (Floating) | `0 2px 4px rgba(7,1,24,.04), 0 6px 20px rgba(7,1,24,.07), 0 16px 40px rgba(7,1,24,.07)` | Modals, drawers, popovers |

## Typography Scale

### Casing Rules
- **Headings (H1–H4):** Title Case
- **Eyebrow labels:** Uppercase with letter-spacing `.16em`
- **Body & captions:** Sentence case
- **Buttons & CTAs:** Title Case
- **Data labels:** Preserve acronyms (APY, TVL, NAV, KYC, ETH stay uppercase)

### Website
| Element | Font | Weight | Size | Line-height | Letter-spacing |
|---------|------|--------|------|-------------|----------------|
| Eyebrow | Space Grotesk | SemiBold | 11px | — | .16em, uppercase |
| H1 Hero | Space Grotesk | Bold | 64px | 1.0 | -.04em |
| H2 Section | Space Grotesk | Bold | 46px | 1.05 | -.03em |
| H3 Feature | Space Grotesk | Medium | 22px | 1.3 | — |
| H3 Marketing | Space Grotesk | Bold | 18px | — | -.01em |
| Body | Sora | Regular | 16px | 1.6 | — |

### App UI
| Element | Font | Weight | Size | Line-height | Letter-spacing |
|---------|------|--------|------|-------------|----------------|
| App Body | Sora | Regular | 13px | 1.5 | — |
| App Label | Sora | Bold | 11px | — | .08em, uppercase |
| UI Caption | Sora | Regular | 11px | 1.4 | — |
| Numeric Hero | Space Grotesk | Light | 32px | — | -.02em |
| Numeric KPI | Space Grotesk | SemiBold | 20px | — | -.01em |
| Numeric Table | Sora | Regular | 13px | — | tabular-nums |

## Motion

### Duration
| Token | Value | Usage |
|-------|-------|-------|
| dur-fast | 150ms | Micro-interactions, hover |
| dur-base | 180ms | Buttons, toggles |
| dur-slow | 200ms | Background, color transitions |

## Design Tokens (CSS Variables)

| Token | Value | Usage |
|-------|-------|-------|
| `--violet` | `#5A5BEB` | Primary brand violet |
| `--emerald` | `#28A66B` | Invest, yield, success |
| `--gold` | `#E1A325` | Community, engagement |
| `--crimson` | `#D3194E` | Alerts, destructive |
| `--dark` | `#070118` | Primary dark bg |
| `--ink` | `#070118` | Text on light bg |
| `--muted` | `#6B7280` | Secondary text |
| `--surf` | `#F5F6F8` | Light page bg |
| `--err` | `#D3194E` | Error states |
| `--success` | `#065F46` | Confirmed states |
| `--font-display` | `Space Grotesk, sans-serif` | Headings, hero text |
| `--font-body` | `Sora, sans-serif` | Body, UI, data |
| `--font-numeric` | `Space Grotesk, sans-serif` | KPIs, metric values |
| `--shadow1` | `0 1px 4px rgba(12,14,26,.06)` | Cards at rest |
| `--shadow2` | `0 4px 16px rgba(12,14,26,.09)` | Lifted cards, dropdowns |
| `--shadow3` | `0 12px 40px rgba(12,14,26,.14)` | Modals, drawers |
| `--r-sm` | `6px` | Badges, chips |
| `--r-md` | `8px` | Inputs, buttons |
| `--r-lg` | `12px` | Cards, panels |
| `--r-xl` | `20px` | Form cards, modals |
| `--r-2xl` | `24px` | Hero strips |

---

## Component Rules

### Buttons
- **Pill-shaped** always: `border-radius: 100px`
- Font: Sora SemiBold (600), letter-spacing default
- Transition: `all .18s`
- Disabled: `opacity: .75`, `cursor: not-allowed`

| Size | Font Size | Padding |
|------|-----------|---------|
| XS | 11px | `6px 14px` |
| SM | 13px | `8px 18px` |
| MD | 14px | `10px 22px` |
| LG | 16px | `13px 28px` |

| Variant | Background | Text | When to use |
|---------|-----------|------|-------------|
| Primary | `#5A5BEB` + `box-shadow: 0 4px 14px rgba(90,91,235,.35)` | white | Main CTA — 1 per view max |
| Gradient | `linear-gradient(135deg, #5A5BEB, #E1A325)` | white | Hero CTA |
| Secondary | `#28A66B` | white | Key onboarding (tokenize, connect) |
| Outline | transparent, `1.5px solid #5A5BEB` | `#5A5BEB` | Secondary action alongside filled button |
| Ghost | transparent, `1.5px solid var(--dm-border)` | `var(--dm-ink)` | Tertiary — cancel, dismiss |
| Danger | `#D3194E` | white | Destructive action, always requires confirmation |

### Badges
- Rounded: `border-radius: 100px`
- Font: 13px, fontWeight 600
- Padding: `6px 14px`
- Include a 7px colored dot before label text

#### Status
| Badge | Text Color | Background | Dot |
|-------|-----------|------------|-----|
| Active | `#28A66B` | `rgba(40,166,107,.15)` | `#28A66B` |
| Verified | `#5A5BEB` | `rgba(129,130,239,.08)` | `#5A5BEB` |
| KYC Req. | `#E1A325` | `rgba(225,163,37,.14)` | `#E1A325` |
| Reg D | `#8182EF` | `rgba(90,91,235,.14)` | `#5A5BEB` |
| Pending | `#8182EF` | `rgba(90,91,235,.14)` | `#8182EF` |
| Suspended | `#D3194E` | `rgba(211,25,78,.15)` | `#D3194E` |
| Neutral | `#9CA3AF` | `rgba(107,114,128,.12)` | `#9CA3AF` |

#### Chain Badges
| Chain | Color |
|-------|-------|
| ETH | `#627EEA` |
| POLY | `#8247E5` |
| ARB | `#8182EF` |
| OP | `#FF0420` |
| BASE | `#0052FF` |
| SOL | `#14F195` |

### Form Inputs
- Background: `var(--dm-surface)` (light), `rgba(255,255,255,.04)` (dark)
- Border: `1.5px solid var(--dm-border)` (default), `#5A5BEB` (focused)
- Border radius: 8px
- Padding: `10px 14px`
- Focus ring: `box-shadow: 0 0 0 3px rgba(90,91,235,.12)`
- Error state: `#D3194E` border, `#FCE8EF` background
- Disabled: `opacity: .55`, `cursor: not-allowed`
- Layout: 2-column grid (`1fr 1fr`) for side-by-side fields

### Cards (Six Named Tiers)
| Tier | Background | Border | Radius | Shadow |
|------|-----------|--------|--------|--------|
| Surface | `var(--dm-surface)` | `1px solid var(--dm-border)` | 16px | S1 |
| Raised | `var(--dm-surface)` | `1px solid var(--dm-border)` | 16px | S2 |
| Dark | `#070118` | `1px solid rgba(90,91,235,.15)` | 16px | S2 |
| Glass | `linear-gradient(135deg, rgba(90,91,235,.08), rgba(90,91,235,.03))` | `1px solid rgba(90,91,235,.18)` | 16px | S1 |
| Accent | `linear-gradient(135deg, {color}0d, {color}05)` + 3px top stripe | `1px solid {color}30` | 16px | S1 |
| Section | `var(--dm-surface)` | `1px solid var(--dm-border)` | 20px | S2 |

**Card Rules:**
- Never compose card styles inline — always reference a named tier
- No custom border-radius outside the scale
- Never use `overflow:hidden` on elements with `boxShadow`
- Never mix card tiers on the same hierarchy level
- Always reference S1 / S2 / S3 — never inline shadow values

### Toasts / Alerts
- Border-radius: 12px
- Include icon (36px, rounded 10px) + title + description
- Layout: flex row, gap 12px

| Type | Accent Color | Background | Border |
|------|-------------|-----------|--------|
| Success | `#28A66B` | `rgba(40,166,107,.08)` | `rgba(40,166,107,.25)` |
| Info | `#5A5BEB` | `rgba(90,91,235,.06)` | `rgba(90,91,235,.2)` |
| Warning | `#E1A325` | `rgba(225,163,37,.07)` | `rgba(225,163,37,.3)` |
| Error | `#D3194E` | `rgba(211,25,78,.07)` | `rgba(211,25,78,.25)` |

### Modals
- Overlay: `rgba(7,1,24,.52)` with `backdrop-filter: blur(3px)`
- Card: `var(--dm-surface)`, border-radius 20px, max-width 420px
- Padding: 32px
- Variants: Confirm (centered), Form (multi-step), Info, Right Drawer, Bottom Sheet

### Navigation Sidebar
- Background: `#070118` (navy)
- Active item: inset left 2px border `#8182EF`
- Hover: `rgba(255,255,255,.04)` background

---

## Design Principles

1. **Violet-first identity** — `#5A5BEB` is the primary brand color. All accent states lead with violet.
2. **Two-font system** — Space Grotesk for display/headings/numbers. Sora for body/UI/data. No exceptions.
3. **4px spacing base** — All spacing is a multiple of 4px. Use the spacing tokens.
4. **Six card tiers** — Surface, Raised, Dark, Glass, Accent, Section. Never freestyle card styles.
5. **Pill-shaped buttons** — `border-radius: 100px` on all buttons and badges.
6. **Shadows use purple-black** — `rgba(7,1,24,...)` base for tonal harmony with the violet palette.
7. **Color encodes meaning** — Violet (tokenization/primary), Emerald (invest/success), Gold (community/warning), Crimson (lending/danger).
8. **Reuse tokens** — Never hardcode colors, spacing, or radii. Use CSS custom properties from this guide.
