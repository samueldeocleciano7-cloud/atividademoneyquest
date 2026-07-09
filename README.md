---
name: Quest-Driven Finance
colors:
  surface: '#150a38'
  surface-dim: '#150a38'
  surface-bright: '#3c3261'
  surface-container-lowest: '#100433'
  surface-container-low: '#1e1341'
  surface-container: '#221845'
  surface-container-high: '#2d2350'
  surface-container-highest: '#382e5c'
  on-surface: '#e7deff'
  on-surface-variant: '#cac4d2'
  inverse-surface: '#e7deff'
  inverse-on-surface: '#332957'
  outline: '#938f9c'
  outline-variant: '#484550'
  surface-tint: '#cbbeff'
  primary: '#cbbeff'
  on-primary: '#33226f'
  primary-container: '#2d1b69'
  on-primary-container: '#9686d9'
  inverse-primary: '#6252a1'
  secondary: '#d7ffc5'
  on-secondary: '#053900'
  secondary-container: '#2ff801'
  on-secondary-container: '#0f6d00'
  tertiary: '#e9c400'
  on-tertiary: '#3a3000'
  tertiary-container: '#c9a900'
  on-tertiary-container: '#4c3f00'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#e7deff'
  primary-fixed-dim: '#cbbeff'
  on-primary-fixed: '#1e055a'
  on-primary-fixed-variant: '#4a3a87'
  secondary-fixed: '#79ff5b'
  secondary-fixed-dim: '#2ae500'
  on-secondary-fixed: '#022100'
  on-secondary-fixed-variant: '#095300'
  tertiary-fixed: '#ffe16d'
  tertiary-fixed-dim: '#e9c400'
  on-tertiary-fixed: '#221b00'
  on-tertiary-fixed-variant: '#544600'
  background: '#150a38'
  on-background: '#e7deff'
  surface-variant: '#382e5c'
typography:
  display-hero:
    fontFamily: Plus Jakarta Sans
    fontSize: 40px
    fontWeight: '800'
    lineHeight: 48px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
  headline-lg-mobile:
    fontFamily: Plus Jakarta Sans
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
  monetary-lg:
    fontFamily: Space Grotesk
    fontSize: 28px
    fontWeight: '700'
    lineHeight: 34px
    letterSpacing: -0.03em
  body-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-caps:
    fontFamily: Space Grotesk
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
  stats-sm:
    fontFamily: Space Grotesk
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  container-padding: 20px
  element-gap: 12px
  section-margin: 32px
  radius-inner: 12px
  radius-outer: 24px
---

## Brand & Style

This design system establishes a visual language that transforms mundane financial management into an epic adventure. It bridges the gap between high-stakes fintech reliability and the dopamine-driven engagement of modern gaming. 

The style is **Neo-Gaming Minimal**: a fusion of dark-mode professionalism and vibrant, "glow-in-the-dark" UI elements. It leverages the depth of a dark palette to make progress indicators and financial milestones feel like legendary achievements. The aesthetic is high-energy and motivating, using depth and bioluminescent accents to guide the user through their financial "campaign." 

The emotional response should be one of empowerment and momentum—turning the anxiety of budgeting into the excitement of leveling up.

## Colors

The palette is anchored in a rich, multi-layered dark purple environment. 

- **Primary Background (#2D1B69):** A deep, midnight violet that provides the "canvas" for the adventure.
- **Neon Green (#39FF14):** Reserved for "positive growth" signals—income, budget surplus, and health bars. This should feel like it's glowing.
- **Achievement Gold (#FFD700):** Used exclusively for rewards, currency (coins), streaks, and high-level milestones.
- **Soft Red (#FF4D4D):** Denotes danger zones, overspending, or critical alerts.
- **Surface Neutrals:** Use varying shades of the primary purple (#1A0F3D for deep backgrounds, #3D2A85 for elevated cards) to maintain a cohesive atmospheric feel without resorting to flat blacks or greys.

## Typography

The typography strategy employs a "dual-engine" approach:

1.  **Plus Jakarta Sans** provides a friendly, rounded, and approachable feel for the narrative and general interface elements. Its soft terminals prevent the app from feeling overly "aggressive" or corporate.
2.  **Space Grotesk** is used for all technical data, monetary values, and UI labels. Its geometric, slightly futuristic construction reinforces the "Quest" theme and ensures that financial figures are crystal clear and distinguished from descriptive text.

**Formatting Note:** Monetary values should always be rendered in Space Grotesk. For significant losses or gains, increase the font weight to Bold to emphasize the impact on the user's "stats."

## Layout & Spacing

The layout follows a **Fluid Grid** model with high internal padding to give elements "room to breathe" amidst the dark background. 

- **Mobile:** 4-column grid with 20px margins.
- **Tablet/Desktop:** 12-column grid with 24px gutters.

Spacing follows an 8px base unit. To maintain the gaming aesthetic, cards and containers should utilize generous internal padding (min 20px) to prevent the UI from feeling cramped. Content should be grouped into "Stages" or "Sections" separated by clear 32px vertical margins to create a sense of progression as the user scrolls.

## Elevation & Depth

Depth is achieved through **Tonal Layering** and **Glow Effects** rather than traditional drop shadows.

- **Level 0 (Background):** Primary Violet (#2D1B69).
- **Level 1 (Cards/Containers):** Lighter Surface Purple (#3D2A85). Use a subtle 1px inner border (opacity 10%) to define edges.
- **Level 2 (Active Elements):** Elements "glow" using a drop shadow that matches the element's color (e.g., a Neon Green button has a soft green outer glow with 40% opacity).
- **Backdrop Blurs:** Use 12px-20px blurs for overlays and bottom sheets to maintain visual context of the "world map" (the main dashboard) underneath.

## Shapes

The design system utilizes **Rounded (Level 2)** geometry to balance the "tech" feel with friendliness. 

- Standard components (buttons, input fields) use a 0.5rem (8px) radius.
- Feature cards and XP-style containers use a 1rem (16px) radius to feel more prominent.
- Interactive status indicators (streaks, coins) should be fully pill-shaped or circular.

## Components

### Buttons & Inputs
- **Primary Action:** Neon Green background with dark text. Apply a subtle outer glow.
- **Secondary Action:** Ghost style with Neon Green borders and Space Grotesk labels.
- **Inputs:** Deep violet background (#1A0F3D) with a subtle 1px border that turns Gold when focused.

### Gamified Progress
- **XP Bars:** Use thick, horizontal bars for budget progress. The background should be a desaturated purple, with the "fill" using Neon Green. For overspending, the bar should pulse in Soft Red.
- **Circular Budgets:** Use heavy stroke weights (12pt+) for circular progress rings.
- **Streak Counters:** Displayed in Gold with a flame icon. Use a "floating" elevation effect.

### Cards & Lists
- **Achievement Cards:** Feature Gold borders and a background gradient (from #3D2A85 to a slightly more metallic purple).
- **Transaction Lists:** Clean, 1-line or 2-line entries. Use icons with colored backgrounds (e.g., a green icon for income) inside 40x40px rounded squares.

### Icons
- **Category Icons:** Stylized, illustrated glyphs (e.g., a shield for insurance, a potion for health/wellness, a sword for "fighting" debt).
- **Interaction Feedback:** When a goal is met, trigger a Gold-tinted confetti overlay.
