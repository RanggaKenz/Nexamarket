---
name: NexaMarket High-End Systems
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
  on-surface-variant: '#434655'
  inverse-surface: '#2d3133'
  inverse-on-surface: '#eff1f3'
  outline: '#737686'
  outline-variant: '#c3c6d7'
  surface-tint: '#0053db'
  primary: '#004ac6'
  on-primary: '#ffffff'
  primary-container: '#2563eb'
  on-primary-container: '#eeefff'
  inverse-primary: '#b4c5ff'
  secondary: '#565e74'
  on-secondary: '#ffffff'
  secondary-container: '#dae2fd'
  on-secondary-container: '#5c647a'
  tertiary: '#005e6e'
  on-tertiary: '#ffffff'
  tertiary-container: '#00788c'
  on-tertiary-container: '#d7f6ff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dbe1ff'
  primary-fixed-dim: '#b4c5ff'
  on-primary-fixed: '#00174b'
  on-primary-fixed-variant: '#003ea8'
  secondary-fixed: '#dae2fd'
  secondary-fixed-dim: '#bec6e0'
  on-secondary-fixed: '#131b2e'
  on-secondary-fixed-variant: '#3f465c'
  tertiary-fixed: '#acedff'
  tertiary-fixed-dim: '#4cd7f6'
  on-tertiary-fixed: '#001f26'
  on-tertiary-fixed-variant: '#004e5c'
  background: '#f7f9fb'
  on-background: '#191c1e'
  surface-variant: '#e0e3e5'
typography:
  display-xl:
    fontFamily: Inter
    fontSize: 64px
    fontWeight: '800'
    lineHeight: '1.1'
    letterSpacing: -0.04em
  display-xl-mobile:
    fontFamily: Inter
    fontSize: 40px
    fontWeight: '800'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.3'
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '700'
    lineHeight: '1.3'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  label-sm:
    fontFamily: Geist
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1'
    letterSpacing: 0.02em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 4px
  section-padding-desktop: 120px
  section-padding-mobile: 64px
  gutter: 24px
  container-max: 1280px
---

## Brand & Style
The design system is engineered to evoke technical excellence, reliability, and high-performance engineering. It targets high-end enterprises and ambitious startups requiring bespoke marketplace infrastructure.

The aesthetic is **Modern Minimalist with a Technical Edge**, drawing inspiration from the precise, utility-first interfaces of leading developer-centric platforms. The UI prioritizes extreme clarity through generous whitespace and a rigorous hierarchy. To elevate the experience beyond standard corporate design, the system utilizes "Glassmorphism" for utility layers and subtle gradients to imply depth. The result is a tactile, "high-spec" interface that feels both robust and frictionless.

## Colors
The palette is rooted in a professional "Utility Blue" core. 
- **Primary Blue (#2563EB):** Used for primary actions and brand emphasis.
- **Dark Navy (#0F172A):** Acts as the anchor for headings and high-contrast components, providing the "developer-tool" gravity.
- **Cyan Accent (#06B6D4):** Reserved for technical highlights, status indicators, and subtle gradients in process diagrams.
- **Background Strategy:** Surfaces primarily live on `#FFFFFF` for content clarity, while `#F8FAFC` is used for section differentiation and container grouping.

## Typography
This design system utilizes a unified sans-serif stack to maintain a systematic, technical feel. **Inter** is the workhorse for both display and body copy due to its exceptional legibility and modern apertures. 

For technical labels and small captions, **Geist** is introduced to provide a monospaced-adjacent aesthetic that reinforces the developer-centric nature of the service. Tighten letter spacing on large displays to achieve a high-fashion, premium look.

## Layout & Spacing
The layout follows a **Fluid Grid System** based on a 12-column desktop architecture. 
- **Rhythm:** An 8px incremental scale governs all internal component spacing (8, 16, 24, 32, 48, 64).
- **Sectioning:** Large vertical gaps (120px+) are used to separate major narrative blocks, ensuring the content has room to "breathe" and feels premium.
- **Responsiveness:** At the mobile breakpoint (768px), margins reduce to 24px and the grid collapses to 1-2 columns. Heavy use of `flex-gap` is encouraged for component internal layouts.

## Elevation & Depth
The system uses a "Layered Surface" philosophy:
1. **Base Layer:** `#F8FAFC` background.
2. **Card Layer:** `#FFFFFF` with a very soft, multi-stop shadow (0 4px 6px -1px rgb(0 0 0 / 0.05), 0 2px 4px -2px rgb(0 0 0 / 0.05)).
3. **Glass Layer:** Used for navigation bars and secondary overlays. Apply a `backdrop-blur: 12px` and a semi-transparent white fill (`rgba(255, 255, 255, 0.7)`).
4. **Interactive State:** Elements should lift slightly on hover using a more pronounced, diffused shadow and a -2px Y-axis translation.

## Shapes
The shape language is sophisticated and friendly. 
- **Standard Components:** Buttons and inputs use `rounded-lg` (0.5rem / 8px).
- **Containers & Cards:** High-level containers use `rounded-2xl` (1rem) or `rounded-3xl` (1.5rem) to create a distinct, modern silhouette that softens the technical data within.
- **Process Connectors:** Use 2px stroke widths for lines with 100% rounded caps.

## Components

### Buttons
- **Primary:** Solid `#2563EB` with white text. High-contrast, 0.5rem corner radius.
- **Secondary:** Ghost style with a subtle `#E2E8F0` border and `#0F172A` text. 
- **CTA:** Include a subtle right-arrow icon that translates 2px on hover.

### Pricing Cards
Inspired by Vercel's tiered architecture. Use a prominent `#0F172A` header for the "Enterprise" tier and a subtle border-gradient for the "Recommended" tier. Feature lists should use the Cyan accent for checkmarks.

### Connected Timeline
A vertical or horizontal path using a 2px dashed line in `#CBD5E1`. Active steps are marked by a `#2563EB` solid circle with a `#06B6D4` outer glow (ring).

### Form Fields
Inputs should have a `#F1F5F9` background and a focus state featuring a 2px `#2563EB` ring with 0% offset. Use Geist for placeholder text to maintain the technical vibe.

### Glassmorphic Overlays
For mobile menus or filter sidebars, use 70% opacity white with a heavy background blur and a 1px border of `rgba(255,255,255,0.4)` to simulate a glass edge.