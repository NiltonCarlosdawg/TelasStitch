---
name: Vibrant Delivery
colors:
  surface: '#f9f9f9'
  surface-dim: '#dadada'
  surface-bright: '#f9f9f9'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f3f3f3'
  surface-container: '#eeeeee'
  surface-container-high: '#e8e8e8'
  surface-container-highest: '#e2e2e2'
  on-surface: '#1a1c1c'
  on-surface-variant: '#5b4137'
  inverse-surface: '#2f3131'
  inverse-on-surface: '#f1f1f1'
  outline: '#8f7066'
  outline-variant: '#e4beb2'
  surface-tint: '#a93800'
  primary: '#a53700'
  on-primary: '#ffffff'
  primary-container: '#ce4600'
  on-primary-container: '#fffbff'
  inverse-primary: '#ffb59b'
  secondary: '#815500'
  on-secondary: '#ffffff'
  secondary-container: '#feae20'
  on-secondary-container: '#6a4500'
  tertiary: '#5c5c5c'
  on-tertiary: '#ffffff'
  tertiary-container: '#757474'
  on-tertiary-container: '#fffcfb'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#ffdbcf'
  primary-fixed-dim: '#ffb59b'
  on-primary-fixed: '#380d00'
  on-primary-fixed-variant: '#812900'
  secondary-fixed: '#ffddb2'
  secondary-fixed-dim: '#ffb94d'
  on-secondary-fixed: '#291800'
  on-secondary-fixed-variant: '#624000'
  tertiary-fixed: '#e4e2e1'
  tertiary-fixed-dim: '#c8c6c5'
  on-tertiary-fixed: '#1b1c1c'
  on-tertiary-fixed-variant: '#474746'
  background: '#f9f9f9'
  on-background: '#1a1c1c'
  surface-variant: '#e2e2e2'
typography:
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '700'
    lineHeight: '1.2'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.5'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  label-lg:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '600'
    lineHeight: '1.2'
  button:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '600'
    lineHeight: '1'
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  space-xs: 4px
  space-sm: 8px
  space-md: 16px
  space-lg: 24px
  space-xl: 32px
  container-margin: 20px
  gutter: 16px
---

## Brand & Style

The brand personality is high-energy, reliable, and "crave-worthy." It targets a fast-paced urban audience that values convenience without sacrificing the excitement of a good meal. The design style is **Modern/Corporate with High-Contrast accents**, utilizing bold saturation to stimulate appetite and movement. 

The UI prioritizes clarity and speed, using a clean light background to let food photography shine, while employing the vibrant orange and yellow palette to guide the user's eye toward conversion points and essential delivery information.

## Colors

This color palette is designed to be "appetizing." The **Primary Orange (#F95A0D)** is the main action driver, used for primary buttons and critical brand moments. The **Secondary Yellow (#FBAC1D)** acts as an energetic highlight, perfect for promotions, ratings, and accents. 

**Neutro Escuro (#292929)** provides the grounding necessary for high legibility in typography and icon outlines. The background should remain primarily off-white to ensure the interface feels fresh and hygienic.

## Typography

This design system uses **Inter** exclusively to maintain a functional, systematic, and highly readable interface. Headlines are set with heavy weights and tight letter spacing to create a bold, "billboard" effect for food categories and restaurant names. Body text maintains a generous line height to ensure descriptions of dishes are easy to scan. Label styles use a semi-bold weight for clear information hierarchy in delivery times and pricing.

## Layout & Spacing

The system uses a **Fluid Grid** model. On mobile, it utilizes a 4-column layout with 20px side margins to ensure touch targets are comfortable. Desktop environments expand to a 12-column grid. The spacing rhythm is based on an 8px scale, though 4px increments are allowed for tight component internals (like icon-to-label spacing). Use "space-lg" (24px) to separate distinct sections of the app, such as "Recent Orders" from "Popular Near You."

## Elevation & Depth

Hierarchy is achieved through **Tonal Layers** and **Soft Ambient Shadows**. 
- **Surface Level 0:** The main page background (Neutral light).
- **Surface Level 1:** Cards and containers, using a subtle 1px border (#EEEEEE) or a very soft, diffused shadow (10% opacity of #292929, 12px blur) to lift them off the background.
- **Surface Level 2:** Floating action buttons and active cart drawers, using a more pronounced shadow to indicate immediate interactivity.

Avoid heavy dark shadows; the "appetizing" look is maintained by keeping shadows warm and transparent.

## Shapes

The shape language is friendly and modern. Large containers and cards must use **radius-lg (16px)** to feel approachable. Smaller nested elements like input fields or product thumbnails use **radius-md (12px)**. All interactive triggers, specifically buttons and category chips, follow a **Pill-shaped** (full-radius) geometry to reinforce the energetic and "fast" nature of the service.

## Components

- **Buttons:** All primary buttons are pill-shaped, using #F95A0D with white text. Secondary buttons use a pill shape with a #292929 border or a light yellow background.
- **Cards:** Restaurant and food cards use a 16px radius. Images should have a subtle inner glow or be clipped precisely to the card radius.
- **Chips:** Used for filters (e.g., "Free Delivery", "Burgers"). These are pill-shaped with #FBAC1D backgrounds when active.
- **Input Fields:** Use a 12px radius with a light grey stroke. On focus, the stroke changes to the primary Orange.
- **Progress Indicators:** For delivery tracking, use a combination of the Orange and Yellow palette to show movement and status.
- **Navigation Bar:** Keep it clean with a white background and Neutral Escuro (#292929) icons, using the Primary Orange only for the "Active" state.