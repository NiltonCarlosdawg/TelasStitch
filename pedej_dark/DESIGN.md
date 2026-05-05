---
name: PedeJá Dark
colors:
  surface: '#1e100b'
  surface-dim: '#1e100b'
  surface-bright: '#47352f'
  surface-container-lowest: '#180b06'
  surface-container-low: '#271813'
  surface-container: '#2b1c16'
  surface-container-high: '#372620'
  surface-container-highest: '#42312b'
  on-surface: '#f9dcd3'
  on-surface-variant: '#e4beb2'
  inverse-surface: '#f9dcd3'
  inverse-on-surface: '#3e2c26'
  outline: '#aa897e'
  outline-variant: '#5b4137'
  surface-tint: '#ffb59b'
  primary: '#ffb59b'
  on-primary: '#5b1a00'
  primary-container: '#fb5b0f'
  on-primary-container: '#501600'
  inverse-primary: '#a93800'
  secondary: '#ffb94d'
  on-secondary: '#452b00'
  secondary-container: '#e79c00'
  on-secondary-container: '#583900'
  tertiary: '#9dcaff'
  on-tertiary: '#003257'
  tertiary-container: '#0795f3'
  on-tertiary-container: '#002b4c'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffdbcf'
  primary-fixed-dim: '#ffb59b'
  on-primary-fixed: '#380d00'
  on-primary-fixed-variant: '#812900'
  secondary-fixed: '#ffddb2'
  secondary-fixed-dim: '#ffb94d'
  on-secondary-fixed: '#291800'
  on-secondary-fixed-variant: '#624000'
  tertiary-fixed: '#d1e4ff'
  tertiary-fixed-dim: '#9dcaff'
  on-tertiary-fixed: '#001d35'
  on-tertiary-fixed-variant: '#00497c'
  background: '#1e100b'
  on-background: '#f9dcd3'
  surface-variant: '#42312b'
typography:
  display-lg:
    fontFamily: Be Vietnam Pro
    fontSize: 48px
    fontWeight: '800'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Be Vietnam Pro
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Be Vietnam Pro
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
  title-lg:
    fontFamily: Be Vietnam Pro
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-lg:
    fontFamily: Be Vietnam Pro
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Be Vietnam Pro
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-lg:
    fontFamily: Be Vietnam Pro
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  xs: 4px
  sm: 12px
  md: 16px
  lg: 24px
  xl: 32px
  gutter: 16px
  margin: 20px
---

## Brand & Style

The visual identity of the design system is rooted in "High-Octane Hospitality." It bridges the gap between the frantic energy of a delivery service and the comforting satisfaction of a late-night meal. The dark mode transformation shifts the brand from a daytime utility to a premium, nocturnal experience tailored for users browsing in low-light environments.

The style is **High-Contrast / Bold**, utilizing deep obsidian surfaces to let the signature orange and yellow accents "pop" with neon-like intensity. By focusing on high-chroma accents against a neutral dark foundation, the design system maintains its energetic personality while reducing eye strain and improving visual hierarchy for hungry users at any hour.

## Colors

The palette is anchored by **Neutral 900 (#121212)** for the base background to ensure pure contrast and power efficiency on OLED screens. **Neutral 800 (#1E1E1E)** serves as the primary surface color for cards and elevated containers, creating a clear but subtle distinction from the background.

The brand's "Vibrant" soul is preserved through the **Primary Orange (#F95A0D)**, used strictly for primary actions and critical brand moments, and **Secondary Yellow (#FBAC1D)**, used for secondary highlights, ratings, and promotions. Typography relies on **Neutral 100 (#F5F5F5)** for maximum legibility, ensuring the interface remains accessible under the strictest AA/AAA contrast guidelines.

## Typography

This design system utilizes **Be Vietnam Pro** across all levels. Its contemporary, geometric construction provides a friendly yet professional tone that feels at home in the food and drink sector. 

In dark mode, letter spacing for smaller body text and labels is slightly increased (+0.01em to +0.05em) to prevent "halation," where light text on dark backgrounds appears to bleed or blur. Headlines use heavy weights (700-800) to command attention and maintain the brand's bold, "vibrant" persona against the dark void of the background.

## Layout & Spacing

The layout philosophy follows a **fluid grid** model based on an 8px rhythmic scale. For mobile contexts, a 4-column grid is used, while desktop environments expand to a 12-column system. 

The rhythm is designed for high-density content—essential for menus and tracking screens—but maintains "breathability" through generous outer margins. We use a 16px gutter to ensure distinct separation between food cards and merchant listings, preventing the UI from feeling cluttered during the high-speed browsing typical of delivery apps.

## Elevation & Depth

In this design system, depth is communicated primarily through **Tonal Layering**. As elements move closer to the user in the Z-axis, their surface color becomes lighter. 

- **Level 0 (Base):** Neutral 900 (#121212)
- **Level 1 (Cards/Lists):** Neutral 800 (#1E1E1E)
- **Level 2 (Modals/Popovers):** Neutral 700 (#2C2C2C)

To maintain the "vibrant" feel, high-elevation components like primary buttons or active order trackers utilize **Ambient Glows** instead of traditional black shadows. These are low-opacity shadows tinted with the Primary Orange (#F95A0D) to simulate a light source emitting from the interactive element itself.

## Shapes

The shape language is consistently **Rounded**, mirroring the friendly curves found in the primary "P" hand-icon logo. A standard radius of 8px (0.5rem) is applied to small interactive elements like inputs and buttons. 

Larger containers, such as merchant cards and product modals, use a more pronounced 16px (1rem) radius. This softness balances the "aggressive" high-contrast color palette, ensuring the app feels approachable and "delicious" rather than cold or overly technical.

## Components

### Buttons
- **Primary:** Solid Primary Orange (#F95A0D) with white text. High-energy, impossible to miss.
- **Secondary:** Outlined with Primary Orange or solid Neutral 800.
- **Floating Action Buttons (FAB):** Always Primary Orange with a subtle orange ambient glow to denote priority.

### Cards
Cards are the workhorse of the design system. They use Neutral 800 surfaces with a 1px stroke of Neutral 700 to provide definition against the Neutral 900 background. Images within cards should have a subtle darkening overlay (10-15%) to ensure text overlays remain legible.

### Input Fields
Fields use a Neutral 800 fill. The "Active" state is signaled by a Primary Orange border and a glowing cursor. Error states utilize a high-visibility Red, while success states use a vibrant Emerald to stand out against the dark theme.

### Chips & Tags
Used for cuisine types (e.g., "Pizza," "Burgers"). These use a semi-transparent version of the Secondary Yellow with 10% opacity for the background and solid Secondary Yellow for the text to create a "lit from within" effect.

### Order Tracking
A unique component for this system, the progress bar utilizes a gradient from Secondary Yellow to Primary Orange to visualize the "heat" and speed of the delivery.