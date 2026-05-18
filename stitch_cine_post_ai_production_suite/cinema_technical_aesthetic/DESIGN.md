---
name: Cinema-Technical Aesthetic
colors:
  surface: '#121414'
  surface-dim: '#121414'
  surface-bright: '#37393a'
  surface-container-lowest: '#0c0f0f'
  surface-container-low: '#1a1c1c'
  surface-container: '#1e2020'
  surface-container-high: '#282a2b'
  surface-container-highest: '#333535'
  on-surface: '#e2e2e2'
  on-surface-variant: '#b9cacb'
  inverse-surface: '#e2e2e2'
  inverse-on-surface: '#2f3131'
  outline: '#849495'
  outline-variant: '#3a494b'
  surface-tint: '#00dbe7'
  primary: '#e1fdff'
  on-primary: '#00363a'
  primary-container: '#00f2ff'
  on-primary-container: '#006a71'
  inverse-primary: '#00696f'
  secondary: '#c5c6cb'
  on-secondary: '#2e3134'
  secondary-container: '#44474b'
  on-secondary-container: '#b3b5ba'
  tertiary: '#f6f7ff'
  on-tertiary: '#2e3036'
  tertiary-container: '#d9dbe2'
  on-tertiary-container: '#5d6066'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#74f5ff'
  primary-fixed-dim: '#00dbe7'
  on-primary-fixed: '#002022'
  on-primary-fixed-variant: '#004f54'
  secondary-fixed: '#e1e2e7'
  secondary-fixed-dim: '#c5c6cb'
  on-secondary-fixed: '#191c1f'
  on-secondary-fixed-variant: '#44474b'
  tertiary-fixed: '#e1e2e9'
  tertiary-fixed-dim: '#c4c6cd'
  on-tertiary-fixed: '#191c21'
  on-tertiary-fixed-variant: '#44474d'
  background: '#121414'
  on-background: '#e2e2e2'
  surface-variant: '#333535'
typography:
  h1:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  h2:
    fontFamily: Space Grotesk
    fontSize: 24px
    fontWeight: '500'
    lineHeight: '1.3'
    letterSpacing: -0.01em
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
    letterSpacing: '0'
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: '1.5'
    letterSpacing: '0'
  mono-label:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.05em
  data-point:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '700'
    lineHeight: '1'
    letterSpacing: '0'
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  gutter: 12px
  margin: 16px
---

## Brand & Style

The brand identity centers on the concept of "Digital Precision." This design system communicates high-performance post-production capabilities through a technical, laboratory-grade interface. It targets professional film editors who require an environment that feels both authoritative and unobtrusive. 

The visual style is defined by **Sleek Glassmorphism** and **Technical Minimalism**. By utilizing deep backgrounds and luminous foreground elements, the interface mimics a dark editing suite. The emotional response is one of focus, clarity, and cutting-edge intelligence. Motion and patterns, specifically "scanning" horizontal lines and subtle pulse animations, should be used to indicate AI processing and data flow without distracting from the creative work.

## Colors

The palette is strictly high-contrast to ensure legibility in low-light environments typical of editing bays. 

- **Primary:** Neon Cyan (#00F2FF) is reserved for critical actions, active states, and AI-driven insights. It serves as the "source of light" within the interface.
- **Backgrounds:** Deep Space Black (#05070A) provides the base canvas, while a secondary darker gray (#14171C) is used to define container levels.
- **Typography:** Pure White (#FFFFFF) is the standard for primary text, while reduced opacity whites (60% and 40%) are used for secondary and tertiary metadata.
- **Accents:** Utilize the accent glow for "active" indicators on the timeline or to highlight AI-detected scene changes.

## Typography

This design system uses a dual-font strategy to balance character with utility. **Space Grotesk** is used for headlines to provide a geometric, futuristic edge. **Inter** is the workhorse for the interface, chosen for its exceptional legibility at high densities and small sizes.

For technical data (timecodes, frame counts, bitrates), use the `mono-label` or `data-point` styles. These ensure that numerical values remain prominent and easy to scan. All labels should maintain a high degree of contrast against the dark background.

## Layout & Spacing

A **mobile-first, high-density fluid grid** is used to maximize the available screen real estate for video previews and timelines. The layout relies on an 8px rhythmic system, but allows for 4px increments (base) for tight technical controls.

- **Mobile:** Single column with horizontal scrolling "filmstrip" components.
- **Desktop/Tablet:** Multi-panel layout with collapsible sidebars.
- **Density:** Elements are packed tightly to minimize eye travel, using subtle borders rather than large margins to separate functional zones.

## Elevation & Depth

Depth is achieved through **Glassmorphism** and **Tonal Layering** rather than traditional drop shadows. 

1.  **Floor:** The base background (#05070A).
2.  **Surface:** Semi-transparent layers (10-15% white opacity) with a `backdrop-filter: blur(12px)`.
3.  **Stroke:** Every glass container must have a 1px inner border (`glass_stroke`) to define its edges against the dark background.
4.  **Luminescence:** "Scanning" line patterns (1px height, low-opacity Cyan) should move vertically across active processing cards to indicate background AI tasks.
5.  **Focus:** When an element is selected, it should emit a subtle Cyan outer glow (`accent_glow`) to simulate a backlit physical console.

## Shapes

The shape language is professional and "engineered." We use **Soft (0.25rem)** rounding for standard components like buttons and input fields to maintain a sleek, modern feel without appearing too consumer-oriented or "bubbly."

Larger containers (Cards) use `rounded-lg` (0.5rem) to provide clear structural definition. Interactive icons and status pips may use circular (pill) shapes to differentiate them from functional data containers.

## Components

- **Buttons:** Primary buttons use a solid Neon Cyan fill with black text. Secondary buttons are "Ghost" style with a Cyan stroke and subtle hover glow.
- **Input Fields:** Semi-transparent glass backgrounds with a 1px bottom border. On focus, the border transitions to Neon Cyan with a faint glow.
- **Chips/Badges:** Small, high-density labels with Inter font. Use for file formats (e.g., "RAW", "4K", "ProRes") with a subtle border and no fill.
- **Cards:** Utilize the glassmorphism effect. For AI-processing cards, overlay the "scanning" line pattern.
- **Timeline Rails:** Dark backgrounds with Neon Cyan playheads. AI-suggested edit points are marked with vertical Cyan "scanlines."
- **Checkboxes/Radios:** Square-format (0px or 2px radius) to maintain the technical aesthetic, using Neon Cyan for the "checked" state.
- **Progress Bars:** Thin 2px lines. AI tasks use a dual-tone Cyan gradient with a "pulsing" animation to show active computation.