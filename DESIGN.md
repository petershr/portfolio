---
name: High-Fidelity Engineering Portfolio
colors:
  surface: '#0c1324'
  surface-dim: '#0c1324'
  surface-bright: '#33394c'
  surface-container-lowest: '#070d1f'
  surface-container-low: '#151b2d'
  surface-container: '#191f31'
  surface-container-high: '#23293c'
  surface-container-highest: '#2e3447'
  on-surface: '#dce1fb'
  on-surface-variant: '#c1c8ca'
  inverse-surface: '#dce1fb'
  inverse-on-surface: '#2a3043'
  outline: '#8b9295'
  outline-variant: '#41484a'
  surface-tint: '#a5cdda'
  primary: '#bde5f2'
  on-primary: '#073540'
  primary-container: '#a1c9d6'
  on-primary-container: '#2e5560'
  inverse-primary: '#3d646f'
  secondary: '#c0c7d6'
  on-secondary: '#2a313d'
  secondary-container: '#404754'
  on-secondary-container: '#aeb5c5'
  tertiary: '#d4dff7'
  on-tertiary: '#263143'
  tertiary-container: '#b8c3da'
  on-tertiary-container: '#455064'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#c0e9f7'
  primary-fixed-dim: '#a5cdda'
  on-primary-fixed: '#001f27'
  on-primary-fixed-variant: '#244c57'
  secondary-fixed: '#dce2f3'
  secondary-fixed-dim: '#c0c7d6'
  on-secondary-fixed: '#151c27'
  on-secondary-fixed-variant: '#404754'
  tertiary-fixed: '#d8e3fb'
  tertiary-fixed-dim: '#bcc7de'
  on-tertiary-fixed: '#111c2d'
  on-tertiary-fixed-variant: '#3c475a'
  background: '#0c1324'
  on-background: '#dce1fb'
  surface-variant: '#2e3447'
  surface-stroke: '#334155'
  accent-glow: rgba(161, 201, 214, 0.15)
  terminal-white: '#F8FAFC'
typography:
  display:
    fontFamily: Hanken Grotesk
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Hanken Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-lg-mobile:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Hanken Grotesk
    fontSize: 20px
    fontWeight: '500'
    lineHeight: '1.4'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-md:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1.5'
    letterSpacing: 0.05em
  label-sm:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '400'
    lineHeight: '1.5'
    letterSpacing: 0.02em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 4px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 64px
  container-max: 1200px
---

## Brand & Style

The visual identity of the design system is rooted in **Engineering Minimalism**. It is designed to reflect the precision of hardware engineering and the clarity of academic research. The personality is immersive and technical, creating a "dark mode" laboratory environment that prioritizes deep focus and professional authority.

The aesthetic combines **Minimalism** with **Glassmorphism** and **Technical Brutalism**. It utilizes a strict grid, generous whitespace, and crisp, high-contrast borders to define structure, while subtle glows and translucent surfaces provide a sense of modern depth. The interface should feel like a high-end engineering terminal—sophisticated, functional, and unapologetically technical.

## Colors

The palette is anchored by a deep midnight navy (`#020617`), creating a low-light environment that reduces eye strain and emphasizes technical content. 

- **Primary**: A desaturated technical blue (`#A1C9D6`) used for highlights, interactive states, and branding.
- **Secondary**: A muted slate gray (`#6B7280`) for metadata and secondary descriptions.
- **Neutral**: The foundation is a range of deep navies and slates, moving from the true background to slightly lighter surface containers.
- **Named Colors**: We introduce a specific stroke color for borders and a subtle glow variant of the primary blue to be used for interactive hover states and focal points.

## Typography

The typography strategy leverages three distinct typefaces to balance character and utility:

1.  **Hanken Grotesk (Headlines)**: A sharp, contemporary sans-serif that provides a confident, professional voice for titles.
2.  **Inter (Body)**: Used for long-form project descriptions and narratives due to its exceptional legibility at small sizes.
3.  **JetBrains Mono (Accents)**: A monospaced font used for "metadata" roles—dates, technical specs, and UI labels—reinforcing the engineering theme.

Hierarchy is maintained through strict weight variation. Labels and technical data should always appear in the monospaced font to differentiate data from prose.

## Layout & Spacing

The layout utilizes a **Fixed Grid** system centered on the screen to maintain a structured, editorial feel. 

- **Grid**: A 12-column grid for desktop (reflowing to 1 column for mobile). 
- **Rhythm**: All spacing is derived from a 4px base unit. 
- **Project Cards**: On desktop, project entries are displayed in a 2-column masonry or strict grid.
- **Margins**: Generous outer margins (`64px`) ensure the content feels premium and uncrowded. 

Breakpoints are set at `768px` (Mobile to Tablet) and `1024px` (Tablet to Desktop). On mobile, padding is reduced and the typography scales down to maintain readability without horizontal scrolling.

## Elevation & Depth

This design system avoids traditional soft shadows in favor of **Tonal Layers** and **Glassmorphism**.

1.  **Surfaces**: Background is the lowest level (`#020617`). Project cards and containers sit one level above, using a slightly lighter navy with a 1px solid border (`#334155`).
2.  **Glass Effect**: Primary cards use a very subtle backdrop blur (8px) and a semi-transparent fill to suggest a technical glass overlay.
3.  **Interaction Depth**: Depth is communicated via "Glows" rather than "Shadows." When a card is hovered, it should emit a faint, soft outer glow using the `accent-glow` variable, making the component appear as if it is powered on.

## Shapes

The shape language is **Soft (0.25rem)**. This slight rounding takes the "edge" off the brutalist grid without sacrificing the technical, sharp aesthetic. 

- **Small elements** (buttons, chips): 4px radius.
- **Large elements** (cards, modal containers): 8px radius (`rounded-lg`).
- **Interactive Triggers**: Icons and small buttons may occasionally use a fully circular (pill) shape if they are purely functional (e.g., a "scroll to top" button).

## Components

### Project Cards
The primary vessel for content. Feature a 1px `surface-stroke` border. On hover, the border color transitions to the `primary` blue and the `accent-glow` is applied. Titles inside cards use `headline-md`.

### Technical Chips
Used for listing technologies (e.g., "Altium", "Python"). Styled with the `label-sm` font, a subtle dark background, and a secondary text color. No borders.

### Buttons
- **Primary**: Solid `primary` color background with `neutral` text for high contrast.
- **Secondary**: Ghost style with 1px `surface-stroke` and `primary` color text. 
- **Shape**: 4px radius across all variants.

### Input Fields & Terminal
Text inputs should resemble a code editor environment. Dark backgrounds, monospaced text, and a blinking underscore cursor for focus states.

### Navigation
Top-aligned, minimal text links using `label-md`. Use a "dimmed" state for inactive links (`secondary` color) and a "bright" state for active/hover (`primary` color).