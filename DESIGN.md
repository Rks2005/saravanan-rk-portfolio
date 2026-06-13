---
name: Kinetic Engineering Narrative
colors:
  surface: '#131316'
  surface-dim: '#131316'
  surface-bright: '#39393c'
  surface-container-lowest: '#0e0e11'
  surface-container-low: '#1b1b1e'
  surface-container: '#1f1f22'
  surface-container-high: '#2a2a2d'
  surface-container-highest: '#353438'
  on-surface: '#e4e1e6'
  on-surface-variant: '#c4c7c8'
  inverse-surface: '#e4e1e6'
  inverse-on-surface: '#303033'
  outline: '#8e9192'
  outline-variant: '#444748'
  surface-tint: '#c6c6c7'
  primary: '#ffffff'
  on-primary: '#2f3131'
  primary-container: '#e2e2e2'
  on-primary-container: '#636565'
  inverse-primary: '#5d5f5f'
  secondary: '#adc6ff'
  on-secondary: '#002e6a'
  secondary-container: '#0566d9'
  on-secondary-container: '#e6ecff'
  tertiary: '#ffffff'
  on-tertiary: '#003640'
  tertiary-container: '#acedff'
  on-tertiary-container: '#006e81'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e2e2e2'
  primary-fixed-dim: '#c6c6c7'
  on-primary-fixed: '#1a1c1c'
  on-primary-fixed-variant: '#454747'
  secondary-fixed: '#d8e2ff'
  secondary-fixed-dim: '#adc6ff'
  on-secondary-fixed: '#001a42'
  on-secondary-fixed-variant: '#004395'
  tertiary-fixed: '#acedff'
  tertiary-fixed-dim: '#4cd7f6'
  on-tertiary-fixed: '#001f26'
  on-tertiary-fixed-variant: '#004e5c'
  background: '#131316'
  on-background: '#e4e1e6'
  surface-variant: '#353438'
typography:
  display-lg:
    fontFamily: Space Grotesk
    fontSize: 64px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Space Grotesk
    fontSize: 40px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  headline-lg:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.3'
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 24px
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
  label-mono:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: '1.0'
    letterSpacing: 0.05em
  label-sm:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '500'
    lineHeight: '1.2'
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  container-max: 1280px
  gutter: 24px
  margin-desktop: 64px
  margin-mobile: 20px
  stack-xs: 4px
  stack-sm: 8px
  stack-md: 16px
  stack-lg: 32px
  stack-xl: 64px
---

## Brand & Style

This design system establishes a high-fidelity engineering aesthetic that bridges the gap between hardware prototyping and premium software interfaces. The brand personality is technical, precise, and sophisticated—evoking the feeling of a high-end R&D lab or an aerospace command center.

The style is a hybrid of **Minimalism** and **Glassmorphism**, grounded by a structural **Corporate Modern** framework. It utilizes deep blacks and high-contrast typography to create a sense of focused depth. Visual interest is driven by "technical artifacts": subtle grid overlays, hairline strokes, and micro-interactions that mimic precise instrumentation. The target audience includes engineering recruiters, technical founders, and hardware enthusiasts who value rigor and refined craft.

## Colors

The palette is engineered for maximum focus in low-light environments. 
- **Core Tones:** Deep Black (#000000) serves as the infinite canvas, with Dark Zinc (#18181b) providing structural surfaces.
- **Accents:** Electric Blue and Muted Cyan are reserved for interactive states, data visualization, and status indicators. They should be used sparingly as "glow" effects or single-pixel underlines to maintain a professional atmosphere.
- **Typography:** Pure White is utilized for primary headings to ensure maximum legibility against the dark background, while Slate Gray (#71717a) is used for secondary metadata to establish visual hierarchy.

## Typography

The typographic system utilizes **Space Grotesk** for display and headline roles to lean into its geometric, technical character. Its idiosyncratic letterforms provide a "designed" feel that resonates with ECE hardware aesthetics. 

**Inter** handles body copy for its neutral, highly legible performance at small scales, ensuring technical documentation remains readable. **JetBrains Mono** (or equivalent monospaced font) is introduced for labels, system status, and technical specs, reinforcing the engineering dashboard narrative. All display text should favor tighter tracking to maintain a premium, architectural look.

## Layout & Spacing

The layout follows a **Fixed Grid** philosophy for desktop (12 columns) and a **Fluid** model for mobile (4 columns). The system is built on a 4px baseline grid to ensure mathematical precision in all element placements.

- **Grid Patterns:** Large sections should be subtly underscored by a 24px background grid pattern in 5% opacity Zinc to emphasize the "blueprint" aesthetic.
- **Margins:** Generous white space (stack-xl) is used to separate high-level hardware projects, allowing each engineering feat to stand alone.
- **Alignment:** Elements should strictly adhere to the vertical grid lines. Use hairline vertical dividers (1px) to separate sidebar navigation or metadata columns from main content.

## Elevation & Depth

Depth is achieved through **Tonal Layering** and **Glassmorphism** rather than traditional drop shadows.

1.  **Level 0 (Floor):** Pure Black (#000000). Used for the base canvas.
2.  **Level 1 (Substrate):** Dark Zinc (#18181b). Used for main content cards or sections.
3.  **Level 2 (Float):** Semi-transparent surfaces with a 12px Backdrop Blur. Used for navigation bars and floating modals.
4.  **Stroke Elevation:** Instead of shadows, use 1px "inner-glow" borders. A top border of `rgba(255,255,255,0.1)` and a bottom border of `rgba(255,255,255,0.02)` creates a realistic, machined edge.

Interaction depth is signaled by a subtle Primary Blue outer glow (`box-shadow: 0 0 15px rgba(59, 130, 246, 0.3)`).

## Shapes

The shape language is **Soft** but disciplined. Primary containers and buttons use a 0.25rem (4px) corner radius to maintain a professional, high-end hardware feel (mimicking machined aluminum or glass panels). 

Larger components like project showcase cards can scale to `rounded-lg` (8px), but should never reach "pill" or "circle" status unless they are icon containers or status dots. This restraint ensures the UI feels like a piece of equipment rather than a social app.

## Components

- **Buttons:** Primary buttons are Solid White with Black text for maximum impact. Secondary buttons use a transparent background with a 1px Zinc border and subtle hover transitions to a Blue border.
- **Technical Chips:** Used for "Skills" or "Tools." These should be styled as "ghost" elements with Mono typography and a 1px border.
- **Inputs:** Darker than the surface background with a focused state that illuminates a 1px Blue bottom border.
- **Data Visualization:** Use the Cyan and Blue accents for charts. Lines should be 1.5px thick with "area" fills using a 10% opacity gradient.
- **Cards:** Project cards should feature a "Header-to-Image" layout with technical metadata (e.g., "REV: 2.1", "STATUS: COMPLETED") positioned in the top right using `label-mono`.
- **Instrumentation:** Small status LEDs (pulsing 4px circles) should be used next to active project titles to denote "Live" or "In Production."