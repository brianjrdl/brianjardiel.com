---
name: Cyber-Arcade
colors:
  surface: '#161309'
  surface-dim: '#161309'
  surface-bright: '#3d392d'
  surface-container-lowest: '#110e05'
  surface-container-low: '#1f1b11'
  surface-container: '#231f15'
  surface-container-high: '#2e2a1e'
  surface-container-highest: '#393429'
  on-surface: '#eae2d0'
  on-surface-variant: '#d0c6ac'
  inverse-surface: '#eae2d0'
  inverse-on-surface: '#343024'
  outline: '#999078'
  outline-variant: '#4d4632'
  surface-tint: '#ebc300'
  primary: '#fff4db'
  on-primary: '#3b2f00'
  primary-container: '#ffd524'
  on-primary-container: '#715c00'
  inverse-primary: '#715c00'
  secondary: '#ffd261'
  on-secondary: '#3e2e00'
  secondary-container: '#e9b400'
  on-secondary-container: '#5f4800'
  tertiary: '#d7fcff'
  on-tertiary: '#00363a'
  tertiary-container: '#00effd'
  on-tertiary-container: '#00696f'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffe179'
  primary-fixed-dim: '#ebc300'
  on-primary-fixed: '#231b00'
  on-primary-fixed-variant: '#554500'
  secondary-fixed: '#ffdf98'
  secondary-fixed-dim: '#f6bf16'
  on-secondary-fixed: '#251a00'
  on-secondary-fixed-variant: '#5a4300'
  tertiary-fixed: '#79f5ff'
  tertiary-fixed-dim: '#00dbe8'
  on-tertiary-fixed: '#002022'
  on-tertiary-fixed-variant: '#004f54'
  background: '#161309'
  on-background: '#eae2d0'
  surface-variant: '#393429'
typography:
  display-lg:
    fontFamily: Anybody
    fontSize: 64px
    fontWeight: '900'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  display-lg-mobile:
    fontFamily: Anybody
    fontSize: 40px
    fontWeight: '900'
    lineHeight: '1.1'
  headline-md:
    fontFamily: Anybody
    fontSize: 32px
    fontWeight: '800'
    lineHeight: '1.2'
  body-lg:
    fontFamily: JetBrains Mono
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: JetBrains Mono
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-caps:
    fontFamily: Space Mono
    fontSize: 14px
    fontWeight: '700'
    lineHeight: '1.0'
    letterSpacing: 0.1em
  cta:
    fontFamily: Anybody
    fontSize: 20px
    fontWeight: '900'
    lineHeight: '1.0'
spacing:
  unit: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 48px
  container-max: 1280px
  gutter: 24px
---

## Brand & Style
This design system captures the electric energy of 1980s arcade culture and the nocturnal mood of synthwave music. The brand personality is nostalgic yet futuristic, targeting a tech-savvy audience that appreciates retro-computing aesthetics, gaming, and "low-fi" high-tech.

The visual style is a fusion of **Retro-Vaporwave** and **Neon-Brutalism**. It utilizes CRT-inspired effects, including scanlines, chromatic aberration, and luminous glows, to create an immersive, screen-based experience. The emotional response should be one of "digital warmth" and high-energy excitement.

## Colors
The palette is built on a "Deep Night" foundation with "Neon Sun" accents. 
- **Primary Background (#290849):** A deep, saturated violet that serves as the void for neon elements to pop.
- **Surface/Container (#55185d):** A slightly lighter, more magenta-tinted purple used for interactive areas and card backgrounds.
- **Primary Glow (#ffd524):** The main functional accent. Used for CTAs, active states, and critical information.
- **Secondary Accent (#ecb602):** A deeper gold used for hover states and secondary information.
- **System Accents:** High-frequency Pink and Cyan are reserved for data visualization and status indicators to maintain the synthwave spectrum.

## Typography
The typography strategy creates a contrast between "The Machine" and "The Player." 

- **Display & CTAs:** Use **Anybody** with heavy weights (800-900) and condensed widths. This provides the "Arcade Cabinet" impact. Titles should often be italicized to imply speed and momentum.
- **Interface & Readability:** Use **JetBrains Mono** for all body text. This reinforces the terminal/hacker aesthetic while ensuring high legibility for technical data.
- **System Labels:** **Space Mono** is used for small metadata, providing a structured, geometric feel to the UI.

## Layout & Spacing
The layout follows a **Fixed Grid** model reminiscent of 80s computer interfaces. Elements are aligned to a strict 4px baseline grid to ensure "pixel-perfect" placement.

- **Desktop:** 12-column grid with a fixed 1280px max-width.
- **Margins:** Heavy outer margins (48px+) are encouraged to create a "contained" screen feel, like looking at a monitor within a frame.
- **Borders:** Use thick 2px or 3px borders for containers instead of soft shadows to maintain the brutalist-arcade structure.

## Elevation & Depth
Depth is not communicated through realistic shadows, but through **Luminance and Layering**.

- **Z-Axis Hierarchy:** Higher elevation elements do not cast black shadows; instead, they cast **Neon Glows** (drop-shadows with 0 blur, or high-spread blurs in the accent color).
- **Inner Shadows:** Active containers use a subtle, dark inner shadow to create a "sunken" CRT screen effect.
- **Glassmorphism:** Use backdrop blurs (10px - 20px) on modal overlays with a 20% opacity purple tint to simulate frosted acrylic.
- **The CRT Overlay:** A global fixed overlay of 2px scanlines (semi-transparent black lines) and a subtle vignette should be applied to the entire viewport to unify the aesthetic.

## Shapes
The shape language is strictly **Sharp (0px)**. Rounded corners are avoided to maintain the retro-digital, pixel-based feel. 

For specific "hero" elements, use **beveled corners** (45-degree cuts) rather than radii to mimic hardware chassis designs. Interactive elements should feel like physical toggle switches or heavy-duty arcade buttons.

## Components
- **Buttons:** Primary buttons use the #ffd524 background with black text. Apply a `box-shadow` offset (e.g., 4px 4px 0px #ecb602) to create a "3D" push-button effect. On hover, the button should "sink" (transform: translate(2px, 2px)) and the glow intensity should increase.
- **Input Fields:** Use the #55185d background with a 2px solid #ffd524 border. Use a blinking "block" cursor for text entry.
- **Cards:** Containers must have a 1px solid border in a slightly brighter purple than the surface color, with a faint outer glow (bloom effect).
- **Scanline Overlay:** A persistent, non-interactive absolute div with a repeating linear gradient of `rgba(0,0,0,0.1)` and `transparent` to simulate CRT scanlines.
- **Chips/Badges:** Use high-contrast combinations (e.g., Magenta background with White text) and sharp corners.
- **Progress Bars:** Use segmented blocks (discrete steps) rather than a smooth continuous fill to mimic 8-bit loading sequences.