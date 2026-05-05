---
name: Synthetic Vision
colors:
  surface: '#131314'
  surface-dim: '#131314'
  surface-bright: '#3a393a'
  surface-container-lowest: '#0e0e0f'
  surface-container-low: '#1c1b1c'
  surface-container: '#201f20'
  surface-container-high: '#2a2a2b'
  surface-container-highest: '#353436'
  on-surface: '#e5e2e3'
  on-surface-variant: '#b9cacb'
  inverse-surface: '#e5e2e3'
  inverse-on-surface: '#313031'
  outline: '#849495'
  outline-variant: '#3b494b'
  surface-tint: '#00dbe9'
  primary: '#dbfcff'
  on-primary: '#00363a'
  primary-container: '#00f0ff'
  on-primary-container: '#006970'
  inverse-primary: '#006970'
  secondary: '#ebb2ff'
  on-secondary: '#520072'
  secondary-container: '#b600f8'
  on-secondary-container: '#fff6fc'
  tertiary: '#ddffd3'
  on-tertiary: '#003907'
  tertiary-container: '#00fb40'
  on-tertiary-container: '#006e16'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#7df4ff'
  primary-fixed-dim: '#00dbe9'
  on-primary-fixed: '#002022'
  on-primary-fixed-variant: '#004f54'
  secondary-fixed: '#f8d8ff'
  secondary-fixed-dim: '#ebb2ff'
  on-secondary-fixed: '#320047'
  on-secondary-fixed-variant: '#74009f'
  tertiary-fixed: '#72ff70'
  tertiary-fixed-dim: '#00e639'
  on-tertiary-fixed: '#002203'
  on-tertiary-fixed-variant: '#00530e'
  background: '#131314'
  on-background: '#e5e2e3'
  surface-variant: '#353436'
typography:
  display-xl:
    fontFamily: Space Grotesk
    fontSize: 72px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Space Grotesk
    fontSize: 40px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 24px
    fontWeight: '500'
    lineHeight: '1.4'
  body-lg:
    fontFamily: Manrope
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Manrope
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-caps:
    fontFamily: Space Grotesk
    fontSize: 12px
    fontWeight: '700'
    lineHeight: '1'
    letterSpacing: 0.1em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  container-max: 1440px
  edge-margin: 4rem
  gutter: 2rem
  section-gap: 8rem
  stack-sm: 0.5rem
  stack-md: 1.5rem
---

## Brand & Style

This design system is built for the intersection of human creativity and machine intelligence. The brand personality is enigmatic, high-tech, and premium, positioning the artist not just as a creator but as a "prompt architect." 

The design style is a hybrid of **Futuristic Minimalism** and **Glassmorphism**. It utilizes expansive negative space—rendered in deep, ink-like blacks—to make AI-generated artwork appear as if it is illuminating the screen. Visual interest is generated through light refraction, subtle glows, and razor-sharp typography rather than heavy decorative elements. The goal is to evoke a sense of digital "prestige" and technical mastery.

## Colors

The palette is rooted in a "True Dark" philosophy. The background canvas uses a near-black hex to ensure maximum contrast for high-dynamic-range (HDR) artwork. 

*   **Primary (Electric Blue):** Used for primary actions, active states, and "data-streaming" accents.
*   **Secondary (Cyber Purple):** Used for hover states, depth gradients, and secondary creative highlights.
*   **Tertiary (Emerald Green):** Reserved for success states, "Online/Available" indicators, and technical readouts.
*   **Neutrals:** A range of deep charcoals are used to define surface hierarchy without breaking the dark-mode immersion.

## Typography

This design system employs **Space Grotesk** for headlines and technical labels to lean into a futuristic, "NASA-meets-Gallery" aesthetic. Its geometric quirks provide character at large sizes. 

**Manrope** is used for body copy to ensure maximum readability against dark backgrounds. The line height is intentionally generous to prevent eye fatigue. Technical metadata (like AI prompt parameters or camera settings) should use the `label-caps` style to differentiate data from narrative text.

## Layout & Spacing

The layout follows a **Fixed Grid** model for desktop, centered within the viewport to create a "letterboxed" cinematic feel. 

1.  **The Hero:** Should always be a full-bleed or wide-aspect ratio image container that ignores standard margins to achieve maximum impact.
2.  **The Spacing Rhythm:** We use a "Breathable Grid." Large vertical gaps (`8rem`) between sections ensure that the viewer’s eye focuses on one piece of artwork at a time.
3.  **Masonry Layouts:** For gallery views, use a staggered masonry grid with `2rem` gutters to accommodate varied aspect ratios produced by AI generators.

## Elevation & Depth

Depth is achieved through **Glassmorphism** and light-source simulation rather than traditional shadows.

*   **Glass Layers:** Use `backdrop-filter: blur(12px)` combined with a `1px` border of `rgba(255, 255, 255, 0.1)`. This creates the "frosted tech" look.
*   **Glow States:** Instead of drop shadows, use `box-shadow: 0 0 20px rgba(0, 240, 255, 0.2)` on active elements to simulate the light of a screen or interface.
*   **Layering:** Navigation bars and floating cards should always sit on top of the content using the glass effect, allowing the colors of the artwork to bleed through the UI subtly.

## Shapes

The design system uses **Soft (0.25rem)** rounding for a "precision-engineered" look. While large pills or circles are too friendly for this aesthetic, sharp 90-degree corners feel too aggressive. The subtle radius on images and buttons suggests high-end hardware design, like the corners of a premium smartphone or tablet.

## Components

*   **Primary Buttons:** High-contrast backgrounds (Electric Blue) with black text. On hover, they should trigger a "glow" effect.
*   **Ghost Buttons:** Transparent background with a `1px` border and text in the primary accent color.
*   **Glass Cards:** Used for project descriptions. These feature a semi-transparent dark fill and a blurred backdrop.
*   **Social Icons (Instagram/Telegram):** Icons should be monochromatic (white or light grey) by default. On hover, Instagram should transition to the Cyber Purple accent, and Telegram to the Electric Blue accent.
*   **Status Chips:** Small, pill-shaped indicators for "AI Model Used" or "Availability." Use a dark fill with a `1px` colored border.
*   **Image Hero:** A specialized component that supports lazy-loading and a "shimmer" loading state using a gradient of deep charcoals.