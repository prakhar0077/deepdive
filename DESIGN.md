---
name: Luminous Liquid
colors:
  surface: '#f9f9fb'
  surface-dim: '#d9dadc'
  surface-bright: '#f9f9fb'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f3f5'
  surface-container: '#edeef0'
  surface-container-high: '#e8e8ea'
  surface-container-highest: '#e2e2e4'
  on-surface: '#1a1c1d'
  on-surface-variant: '#4a4455'
  inverse-surface: '#2f3132'
  inverse-on-surface: '#f0f0f2'
  outline: '#7b7487'
  outline-variant: '#ccc3d8'
  surface-tint: '#732ee4'
  primary: '#630ed4'
  on-primary: '#ffffff'
  primary-container: '#7c3aed'
  on-primary-container: '#ede0ff'
  inverse-primary: '#d2bbff'
  secondary: '#006c49'
  on-secondary: '#ffffff'
  secondary-container: '#6cf8bb'
  on-secondary-container: '#00714d'
  tertiary: '#005091'
  on-tertiary: '#ffffff'
  tertiary-container: '#0668b9'
  on-tertiary-container: '#d9e7ff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#eaddff'
  primary-fixed-dim: '#d2bbff'
  on-primary-fixed: '#25005a'
  on-primary-fixed-variant: '#5a00c6'
  secondary-fixed: '#6ffbbe'
  secondary-fixed-dim: '#4edea3'
  on-secondary-fixed: '#002113'
  on-secondary-fixed-variant: '#005236'
  tertiary-fixed: '#d4e3ff'
  tertiary-fixed-dim: '#a4c9ff'
  on-tertiary-fixed: '#001c39'
  on-tertiary-fixed-variant: '#004883'
  background: '#f9f9fb'
  on-background: '#1a1c1d'
  surface-variant: '#e2e2e4'
typography:
  display-lg:
    fontFamily: Playfair Display
    fontSize: 56px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Playfair Display
    fontSize: 40px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-lg-mobile:
    fontFamily: Playfair Display
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Playfair Display
    fontSize: 28px
    fontWeight: '600'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 14px
    fontWeight: '600'
    lineHeight: '1.4'
    letterSpacing: 0.01em
  label-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 12px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  unit: 8px
  container-max: 1280px
  gutter: 24px
  margin-desktop: 64px
  margin-mobile: 20px
---

## Brand & Style
This design system is a light-mode evolution of organic glassmorphism, blending the ethereal qualities of fluid dynamics with the structured clarity of high-end editorial design. It targets a premium audience seeking a serene yet technologically advanced interface.

The design style is **Light Glassmorphism**. It relies on high-intensity backdrop blurs, translucent layers, and a "wet" look created through subtle specular highlights. The emotional response is one of calm sophistication, clarity, and precision. The aesthetic is anchored by soft pastel organic blurs that move behind glass surfaces, providing a sense of depth and life without compromising readability.

## Colors
The palette is centered around a crisp, off-white neutral base (#F9F9FB) that ensures a fresh, airy feel. 

*   **Primary & Secondary:** Violet (#7C3AED) and Mint Green (#10B981) serve as high-contrast neon accents for interactive states and gamified elements, carefully tuned for legibility against light backgrounds.
*   **Ambient Blurs:** Background "blobs" utilize Cloud Blue, Pale Lavender, and Mint. These are placed on the lowest layer, behind the main surface container, and should have a Gaussian blur of at least 80px.
*   **Surfaces:** Use a semi-transparent white (rgba(255, 255, 255, 0.7)) with a heavy backdrop-filter (blur: 24px) to create the signature glass effect.

## Typography
The typographic system creates a sophisticated tension between the classic elegance of **Playfair Display** (Headings) and the modern, approachable clarity of **Plus Jakarta Sans** (UI/Body).

Headlines should utilize slightly tighter letter-spacing to emphasize the editorial feel. Body text prioritizes generous line heights to maintain the "airy" brand personality. Use the uppercase Label-SM style for category tags and small navigation elements to provide a structured contrast to the organic shapes of the UI.

## Layout & Spacing
The layout follows a fluid 12-column grid system with generous negative space. 

*   **Desktop:** 12 columns with 24px gutters and wide 64px outer margins to allow the background blurs to "breathe" around the content edges.
*   **Mobile:** 4 columns with 16px gutters and 20px margins.
*   **Spacing Rhythm:** All spacing between elements must be a multiple of 8px. Use larger increments (64px, 80px, 96px) between major sections to reinforce the minimalist, premium feel. 

Containers should feel like floating "slabs" of glass, often utilizing asymmetrical padding to lean into the organic theme.

## Elevation & Depth
Depth is not communicated through traditional drop shadows, but through **translucency and refraction**.

*   **Level 1 (Base):** The off-white surface with ambient pastel blurs.
*   **Level 2 (Panels):** Glass containers with `backdrop-filter: blur(24px)` and a 1px solid border (#E2E2E7).
*   **Level 3 (Popovers/Modals):** Increased blur (40px) and a very subtle, large-radius ambient shadow (Color: Primary, Opacity: 4%, Blur: 40px) to simulate a physical lift from the surface.

Avoid inner shadows. Use a subtle top-to-bottom white gradient (100% white to 90% white) on the glass surfaces to mimic light hitting a physical pane.

## Shapes
Shapes are "Softly Organic." While primary containers use a 1rem (16px) radius, interactive elements like buttons and input fields should lean towards even softer edges to mimic smooth, water-worn pebbles. 

Avoid sharp 90-degree angles entirely. Use "Continuous Corner" (Squircle) smoothing where possible to enhance the premium, hardware-inspired look of the design system.

## Components
*   **Buttons:** Primary buttons use a solid Neon Violet or Mint with white text. Secondary buttons are "Glass" style: translucent white background, ultra-thin border, and primary-colored text.
*   **Input Fields:** Ghost-style inputs with a 1px bottom border or a very subtle 4% black fill. On focus, the border transitions to a Primary Neon Violet glow.
*   **Cards:** Use the standard Glass panel (Level 2 Elevation). Ensure content inside has high contrast against the blurred background.
*   **Chips/Badges:** Pill-shaped with a soft tint of the accent color (10% opacity) and high-saturation text for the "gamified" feel.
*   **Progress Bars:** Thin, high-gloss tracks with a neon gradient fill (Violet to Mint) to signify motion and energy.
*   **Lists:** Separated by thin #E2E2E7 lines with generous vertical padding (16px-24px).