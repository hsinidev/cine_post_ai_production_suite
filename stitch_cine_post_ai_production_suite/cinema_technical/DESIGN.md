---
name: Cinema Technical
colors:
  surface: '#121414'
  surface-dim: '#121414'
  surface-bright: '#383939'
  surface-container-lowest: '#0d0f0f'
  surface-container-low: '#1a1c1c'
  surface-container: '#1e2020'
  surface-container-high: '#282a2a'
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
  secondary: '#c7c6c6'
  on-secondary: '#303030'
  secondary-container: '#464747'
  on-secondary-container: '#b6b5b4'
  tertiary: '#f6f8f7'
  on-tertiary: '#2e3131'
  tertiary-container: '#d9dbdb'
  on-tertiary-container: '#5d6060'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#74f5ff'
  primary-fixed-dim: '#00dbe7'
  on-primary-fixed: '#002022'
  on-primary-fixed-variant: '#004f54'
  secondary-fixed: '#e3e2e2'
  secondary-fixed-dim: '#c7c6c6'
  on-secondary-fixed: '#1b1c1c'
  on-secondary-fixed-variant: '#464747'
  tertiary-fixed: '#e1e3e2'
  tertiary-fixed-dim: '#c5c7c6'
  on-tertiary-fixed: '#191c1c'
  on-tertiary-fixed-variant: '#444747'
  background: '#121414'
  on-background: '#e2e2e2'
  surface-variant: '#333535'
typography:
  headline-xl:
    fontFamily: Space Grotesk
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  body-base:
    fontFamily: Space Grotesk
    fontSize: 15px
    fontWeight: '400'
    lineHeight: '1.5'
    letterSpacing: 0em
  label-mono:
    fontFamily: Space Grotesk
    fontSize: 11px
    fontWeight: '500'
    lineHeight: '1'
    letterSpacing: 0.1em
  data-num:
    fontFamily: Space Grotesk
    fontSize: 13px
    fontWeight: '500'
    lineHeight: '1'
    letterSpacing: 0.05em
spacing:
  unit: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  gutter: 1px
  panel-margin: 12px
---

## Brand & Style

This design system is engineered for the high-stakes environment of professional film post-production. It adopts a **Technical Minimalism** aesthetic, blending the precision of aerospace "mission control" interfaces with the high-fidelity expectations of modern cinema. 

The personality is cold, disciplined, and hyper-functional. It prioritizes information density and visual accuracy over decorative elements. The UI should feel like a specialized hardware-software hybrid—an instrument rather than a website. Key attributes include thin structural lines, scanning UI animations (simulating data refreshes), and a strict adherence to a "Dark Mode Only" philosophy to preserve color accuracy and reduce eye strain in dimly lit editing suites.

## Colors

The palette is anchored by **Deep Space Black (#121414)** to maximize screen contrast and black-level depth. **Neon Cyan (#00F2FF)** serves as the high-visibility primary accent, used exclusively for active states, critical data points, and "scanning" elements. 

Secondary and tertiary grays are strictly neutral to avoid color contamination during grading tasks. The "Text Secondary" color is used for labels and inactive metadata to ensure the primary information remains the focal point. Functional colors (Success/Warning/Error) should be desaturated to maintain the technical atmosphere, except when an alert is critical.

## Typography

This design system exclusively utilizes **Space Grotesk**. Its geometric construction and idiosyncratic technical details provide the necessary "cutting-edge" feel while maintaining legibility at high densities.

- **Headlines:** Large and impactful, used sparingly for section headers.
- **Body:** Sized at 15px for readability during long sessions.
- **Labels:** Set in all-caps with wide letter-spacing to mimic traditional equipment marking and digital readouts.
- **Numerical Data:** All timecodes, frame counts, and coordinates must use the `data-num` style to ensure tabular alignment in grids.

## Layout & Spacing

The layout follows a **Fixed Grid** model based on a 4px base unit. UI components are housed within defined "panels" rather than floating freely.

- **12-Column Layout:** Used for dashboard-level arrangements.
- **Micro-Grids:** Within panels, a 1px "grid line" (Gutter) is used to separate tools, creating a drafting-table appearance.
- **Density:** High density is preferred. Minimize whitespace in favor of data proximity, using thin borders (#2A2D2D) rather than large gaps to define structure.
- **Alignment:** Elements should feel "locked" to the grid. Use 12px internal padding for most containers.

## Elevation & Depth

Depth is conveyed through **Tonal Layering** and **Low-Contrast Outlines**. Avoid traditional shadows which "bleed" and soften the technical look.

1. **Base Layer:** Deep Space Black (#121414).
2. **Panel Layer:** Slightly lifted surface (#161818) with a 1px solid border (#2A2D2D).
3. **Active/Interactive Layer:** Use a subtle "Cyan Glow" (0.15 opacity) behind primary buttons or active indicators to simulate a backlit console.
4. **Glassmorphism:** Use sparingly for overlays (modals) with a high blur (20px) and 40% opacity background to maintain context without sacrificing clarity.

## Shapes

To reinforce the cinema-technical aesthetic, this design system uses **Sharp (0px)** corners for all primary structural elements, panels, and data visualizations. 

Softness is avoided to maintain a "machined" feel. Only internal status pips or small toggle switches may use a slight 2px radius if necessary for accessibility, but the default state across buttons, cards, and inputs is strictly orthogonal.

## Components

- **Buttons:** Sharp corners. Primary buttons are #00F2FF with black text. Secondary buttons are outlined in #2A2D2D with a cyan hover state. Use `label-mono` for button text.
- **Chips/Badges:** Small, rectangular containers with 1px borders. Used for metadata like "4K", "RAW", or "LOG".
- **Lists:** High-density, separated by 1px horizontal lines. Hover states should trigger a "scanning" effect—a thin, Cyan vertical bar on the left edge.
- **Input Fields:** Flat #161818 backgrounds with a 1px bottom border. On focus, the border transitions to #00F2FF.
- **Data Visualizations:** Waveforms, histograms, and audio meters use Neon Cyan. Background grids for charts are 1px semi-transparent lines.
- **Timecode Display:** Large, monospaced digits using the primary accent color to highlight the "current position" in a timeline.
- **Scanning UI:** Add a rhythmic, subtle vertical scanline animation (linear-gradient) to large data panels to simulate a live-processing state.