---
name: Obsidian Sanguine
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#e3beb8'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#aa8984'
  outline-variant: '#5a403c'
  surface-tint: '#ffb4a8'
  primary: '#ffb4a8'
  on-primary: '#690000'
  primary-container: '#8b0000'
  on-primary-container: '#ff907f'
  inverse-primary: '#b52619'
  secondary: '#c8c6c5'
  on-secondary: '#303030'
  secondary-container: '#474747'
  on-secondary-container: '#b6b5b4'
  tertiary: '#c6c6c6'
  on-tertiary: '#2f3131'
  tertiary-container: '#414343'
  on-tertiary-container: '#afafb0'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffdad4'
  primary-fixed-dim: '#ffb4a8'
  on-primary-fixed: '#410000'
  on-primary-fixed-variant: '#920703'
  secondary-fixed: '#e4e2e1'
  secondary-fixed-dim: '#c8c6c5'
  on-secondary-fixed: '#1b1c1c'
  on-secondary-fixed-variant: '#474747'
  tertiary-fixed: '#e2e2e2'
  tertiary-fixed-dim: '#c6c6c6'
  on-tertiary-fixed: '#1a1c1c'
  on-tertiary-fixed-variant: '#454747'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  display-xl:
    fontFamily: anybody
    fontSize: 96px
    fontWeight: '800'
    lineHeight: 100px
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: anybody
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: anybody
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
  body-md:
    fontFamily: workSans
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-sm:
    fontFamily: jetbrainsMono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.1em
spacing:
  unit: 8px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 64px
  container-max: 1440px
---

## Brand & Style
The design system embodies a dark, aggressive, and cinematic aesthetic tailored for the metal genre. It prioritizes atmosphere and intensity, utilizing vast negative space to create a sense of impending heaviness. 

The visual direction is a fusion of **Brutalism** and **Glassmorphism**, where raw, sharp-edged structural elements meet sophisticated, glowing ethereal layers. The goal is to evoke a visceral response—coldness from the metallic textures, heat from the blood-red accents, and a sense of depth through "orbital" blurred gradients. The Damascus steel pattern serves as a foundational organic texture, grounding the digital interface in physical, forged metalwork.

## Colors
The palette is dominated by deep blacks and charcoal grays to maintain a high-contrast, atmospheric environment. 

- **Primary (Crimson):** A viscous, "blood" red used sparingly for critical actions, highlights, and glowing states.
- **Secondary (Iron):** A mid-tone charcoal for structural elements and secondary surfaces.
- **Tertiary (Cold Steel):** An off-white, metallic gray for high-readiness typography.
- **Neutral (Obsidian):** The void-like background color that provides the canvas for the Damascus textures and orbital glows.

## Typography
The typography strategy creates a stark contrast between raw aggression and technical precision.

- **Headlines:** Utilizes *Anybody* at heavy weights with tight tracking. It provides a modern, slightly industrial, and aggressive feel that anchors the brand. For a "distressed" look, apply a subtle CSS mask or displacement map using the Damascus steel pattern.
- **Body:** *Work Sans* is used for its exceptional readability against dark backgrounds. Its neutral, professional character ensures that complex information (tour dates, lyrics) remains accessible.
- **Technical Labels:** *JetBrains Mono* is used for metadata, timestamps, and secondary navigation, reinforcing the "precision-engineered" metallic aesthetic.

## Layout & Spacing
The layout follows a **Fixed Grid** model on desktop to maintain cinematic compositions, transitioning to a fluid model on mobile devices.

- **Negative Space:** Use generous margins (64px+) to isolate key imagery and text, mimicking the "Still Night" and "Octane" references.
- **Rhythm:** A strict 8px base unit governs all padding and margins. 
- **The "Orbit" Layer:** Beyond the grid, large-scale blurred radial gradients (Primary red and Neutral grays) should be positioned off-center to create asymmetrical depth and focal points behind the content.

## Elevation & Depth
Hierarchy is established through **Tonal Layers** and **Atmospheric Glows** rather than traditional shadows.

1.  **Base:** The `#0A0A0A` void with a low-opacity Damascus steel pattern overlay.
2.  **Surface:** Dark charcoal `#1A1A1A` containers with sharp edges and 1px "inner-glow" borders (0.5 opacity white) to simulate the edge of a steel blade.
3.  **Active Depth:** Elements "lift" via a primary red outer glow (drop-shadow with 15-20px blur, no offset) rather than black shadows, creating a "heated metal" effect.
4.  **Glassmorphism:** Use backdrop blurs (20px+) on navigation bars to allow the Damascus background pattern to bleed through while maintaining legibility.

## Shapes
The shape language is strictly **Sharp (0)**. Every container, button, and input field must feature 90-degree angles to reinforce the aggressive, metal-forged aesthetic. 

Rounded corners are prohibited, except for the "orbital" background shapes which must be perfectly circular and highly blurred to contrast with the rigid foreground elements.

## Components
- **Buttons:** Primary buttons are solid red (`#8B0000`) with white `label-sm` text. Hover states trigger a white "spark" inner border. Secondary buttons are transparent with a 1px steel border.
- **Input Fields:** Bottom-border only, using a subtle charcoal line that glows red when focused. Typography remains `jetbrainsMono`.
- **Cards:** Textured containers using the Damascus steel pattern at 5% opacity. Borders are sharp and use a linear gradient from charcoal to silver.
- **Chips/Tags:** Monospaced text inside a high-contrast charcoal box with zero padding on the top/bottom to keep the silhouette slim and "barcode-like."
- **Lists:** Tour dates or tracklists should be separated by thin, 1px horizontal lines that fade out at the edges (radial gradient stroke), creating a cinematic, disappearing-into-the-darkness effect.
- **Orbital Elements:** Interactive background elements that follow the cursor with a heavy lag, creating a lagging, atmospheric "smoke" or "glow" effect.