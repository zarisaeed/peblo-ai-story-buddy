---
name: Peblo Play System
colors:
  surface: '#f7f9fb'
  surface-dim: '#d8dadc'
  surface-bright: '#f7f9fb'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f4f6'
  surface-container: '#eceef0'
  surface-container-high: '#e6e8ea'
  surface-container-highest: '#e0e3e5'
  on-surface: '#191c1e'
  on-surface-variant: '#414751'
  inverse-surface: '#2d3133'
  inverse-on-surface: '#eff1f3'
  outline: '#717783'
  outline-variant: '#c1c7d3'
  surface-tint: '#0060ac'
  primary: '#005da7'
  on-primary: '#ffffff'
  primary-container: '#2976c7'
  on-primary-container: '#fdfcff'
  inverse-primary: '#a4c9ff'
  secondary: '#705d00'
  on-secondary: '#ffffff'
  secondary-container: '#fdd73b'
  on-secondary-container: '#715d00'
  tertiary: '#a82468'
  on-tertiary: '#ffffff'
  tertiary-container: '#c94081'
  on-tertiary-container: '#fffbff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d4e3ff'
  primary-fixed-dim: '#a4c9ff'
  on-primary-fixed: '#001c39'
  on-primary-fixed-variant: '#004883'
  secondary-fixed: '#ffe173'
  secondary-fixed-dim: '#e8c426'
  on-secondary-fixed: '#221b00'
  on-secondary-fixed-variant: '#554500'
  tertiary-fixed: '#ffd9e4'
  tertiary-fixed-dim: '#ffb0cd'
  on-tertiary-fixed: '#3e0021'
  on-tertiary-fixed-variant: '#8c0352'
  background: '#f7f9fb'
  on-background: '#191c1e'
  surface-variant: '#e0e3e5'
typography:
  headline-xl:
    fontFamily: Quicksand
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Quicksand
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
  body-lg:
    fontFamily: Quicksand
    fontSize: 18px
    fontWeight: '500'
    lineHeight: 28px
  body-md:
    fontFamily: Quicksand
    fontSize: 16px
    fontWeight: '500'
    lineHeight: 24px
  label-bold:
    fontFamily: Quicksand
    fontSize: 14px
    fontWeight: '700'
    lineHeight: 20px
    letterSpacing: 0.05em
  headline-xl-mobile:
    fontFamily: Quicksand
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 36px
rounded:
  sm: 0.5rem
  DEFAULT: 1rem
  md: 1.5rem
  lg: 2rem
  xl: 3rem
  full: 9999px
spacing:
  base: 8px
  margin-mobile: 20px
  gutter: 16px
  stack-sm: 12px
  stack-md: 24px
  stack-lg: 40px
---

## Brand & Style

The design system is built to evoke a sense of wonder, safety, and accomplishment. It targets children aged 4-10, prioritizing high legibility and tactile interactions that feel "toy-like" rather than "tool-like."

The visual style is **Soft Tactile**, a blend of modern minimalism and skeuomorphic playfulness. It utilizes generous white space to prevent cognitive overload, paired with "squishy" high-radius components that invite touch. The emotional response is one of encouragement—every interaction should feel like a small celebration.

Key aesthetic principles:
- **Exaggerated Rounding:** No sharp corners exist in this system.
- **Dimensionality:** Surfaces use subtle inner glows and soft drop shadows to suggest they can be pressed.
- **Micro-animations:** Elements should "pop" or "bounce" into view to maintain a magical, high-energy feel.

## Colors

The palette is anchored by **Peblo Blue**, a bright, trustworthy primary tone. **Joyful Yellow** is reserved for high-energy highlights and motivational moments, while **Playful Pink** serves as a charming accent for interactive flair.

- **Backgrounds:** Pure white (#FFFFFF) is the primary canvas to ensure maximum readability. A soft neutral (#F8FAFC) is used for secondary background containers to provide subtle depth.
- **Success/Error:** Feedback colors are saturated and clear. Success is a vibrant grass green, while errors use a soft coral red to remain gentle and non-punitive.
- **Accessibility:** All color combinations must maintain a high contrast ratio to accommodate varying visual development stages in children.

## Typography

This design system uses **Quicksand** exclusively. Its rounded terminals and open apertures create a friendly, approachable voice that mirrors the physical shape language of the UI.

- **Scale:** Font sizes are intentionally larger than standard applications to aid developing readers.
- **Weight:** Use Bold (700) for all interactive elements and headings to create a clear visual hierarchy. Medium (500) is used for body text to maintain softness.
- **Case:** Use Title Case for buttons and headers. Avoid All-Caps as it can be harder for young children to decode.

## Layout & Spacing

The layout is optimized for **Mobile-First** interaction. It uses a flexible 4-column grid for mobile devices with generous outer margins to prevent accidental touches near the screen edges.

- **Tap Targets:** Every interactive element must have a minimum tap target of 48x48px, though 64px is preferred for primary actions.
- **Vertical Rhythm:** Content is organized in a "stack" model. Related items (like a question and its options) use `stack-sm`, while distinct sections use `stack-lg`.
- **Safe Areas:** Ensure all critical learning content stays within the vertical center of the device to account for varying hand sizes.

## Elevation & Depth

Depth is used to signify "touchability." This design system avoids harsh shadows in favor of **Ambient Soft Shadows** and **Tonal Offsets**.

- **Level 1 (Base):** Flat white background.
- **Level 2 (Cards):** 20px blur, 10% opacity black shadow, offset Y by 4px. Used for Story Cards.
- **Level 3 (Interactive):** 0px blur, solid 4px bottom border (30% darker than the surface color). This creates a "3D Button" effect that flattens when pressed.
- **Level 4 (Modals):** High-diffusion shadows with a subtle backdrop blur (8px) to focus attention on rewards or feedback.

## Shapes

The shape language is defined by the **Pill-shaped** (Level 3) aesthetic. Every container should feel soft and safe.

- **Standard Containers:** Use 24px (rounded-xl) for cards and main UI blocks.
- **Buttons:** Use 32px or fully rounded ends for a "bubble" appearance.
- **Small Elements:** Even checkboxes and icons should have a minimum corner radius of 8px.

## Components

### Story Card
Large-format containers with a white background and a 1px soft grey stroke. They feature a top-heavy layout for illustrations, followed by a `headline-lg` title. The entire card has a subtle Y-axis lift on hover/active states.

### Action Buttons
Chunky, colorful buttons using a "3D" effect (a solid bottom shadow in a darker shade of the button's color).
- **Primary:** Peblo Blue with White text.
- **Secondary:** Joyful Yellow with Dark Grey text.
- **Active State:** On press, the button shifts down 4px and the shadow disappears, simulating a physical click.

### Quiz Options
Vertical list items with high-radius corners. Each option uses a white background with a thick 2px stroke in `neutral-color`. When selected, the stroke and background transition to `primary-color` with a celebratory "pop" animation.

### Feedback States
- **Success:** A full-screen overlay or modal with a Joyful Yellow star and Green typography. Trigger a confetti burst animation.
- **Error:** The card or input performs a horizontal "shake" (±10px). The border turns to Playful Pink/Red temporarily, accompanied by a "Try Again" prompt in `label-bold`.

### Progress Bar
A thick, rounded track in `neutral-color` with a `primary-color` fill. The "head" of the progress bar should feature a small circle or pebble icon to make tracking progress feel like a journey.