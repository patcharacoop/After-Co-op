---
name: Academic Feedback System
colors:
  surface: '#f8f9ff'
  surface-dim: '#cbdbf5'
  surface-bright: '#f8f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#eff4ff'
  surface-container: '#e5eeff'
  surface-container-high: '#dce9ff'
  surface-container-highest: '#d3e4fe'
  on-surface: '#0b1c30'
  on-surface-variant: '#444653'
  inverse-surface: '#213145'
  inverse-on-surface: '#eaf1ff'
  outline: '#757684'
  outline-variant: '#c4c5d5'
  surface-tint: '#3755c3'
  primary: '#00288e'
  on-primary: '#ffffff'
  primary-container: '#1e40af'
  on-primary-container: '#a8b8ff'
  inverse-primary: '#b8c4ff'
  secondary: '#565e74'
  on-secondary: '#ffffff'
  secondary-container: '#dae2fd'
  on-secondary-container: '#5c647a'
  tertiary: '#003c36'
  on-tertiary: '#ffffff'
  tertiary-container: '#00554e'
  on-tertiary-container: '#5fcdbf'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dde1ff'
  primary-fixed-dim: '#b8c4ff'
  on-primary-fixed: '#001453'
  on-primary-fixed-variant: '#173bab'
  secondary-fixed: '#dae2fd'
  secondary-fixed-dim: '#bec6e0'
  on-secondary-fixed: '#131b2e'
  on-secondary-fixed-variant: '#3f465c'
  tertiary-fixed: '#89f5e7'
  tertiary-fixed-dim: '#6bd8cb'
  on-tertiary-fixed: '#00201d'
  on-tertiary-fixed-variant: '#005049'
  background: '#f8f9ff'
  on-background: '#0b1c30'
  surface-variant: '#d3e4fe'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
  title-sm:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: 16px
    letterSpacing: 0.05em
  data-tabular:
    fontFamily: Inter
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
  unit: 4px
  margin-page: 24px
  gutter-grid: 16px
  padding-card: 20px
  stack-sm: 8px
  stack-md: 16px
  stack-lg: 32px
---

## Brand & Style
The design system is engineered for the educational cooperative sector, focusing on the bridge between academic institutions and professional workplaces. The brand personality is **authoritative, analytical, and supportive**. It aims to evoke a sense of structured progress and objective clarity, ensuring that complex feedback data remains approachable for both administrators and students.

The design style follows a **Corporate / Modern** aesthetic. It prioritizes information density without sacrificing legibility, utilizing a "Layered Flat" approach. This involves using distinct surface levels to organize data, clear typographic hierarchies for rapid scanning, and a restrained use of color to ensure that critical data points remain the focal point of the user experience.

## Colors
The color palette is anchored by a **Trustworthy Blue** (`#1E40AF`) to instill confidence and professional stability. Text is rendered in **Slate Gray** to reduce the harshness of pure black while maintaining high accessibility ratios. 

Data visualization relies on a curated set of accents: **Teal** represents positive growth or completion; **Amber** denotes areas requiring attention or neutral status; **Indigo** is used for comparative metrics or secondary data sets. The background uses a very cool, desaturated off-white to provide a soft canvas for the white cards, reducing eye strain during long-form data analysis.

## Typography
This design system utilizes **Inter** for its exceptional legibility and neutral character. The type scale is optimized for data density. Large displays and headlines use tighter letter spacing and heavier weights to provide clear section anchors. 

For data tables and KPI cards, the `data-tabular` style must be used; this enables tabular num font features to ensure that columns of numbers align vertically for easier comparison. Labels are often presented in uppercase with increased tracking to differentiate metadata from primary content.

## Layout & Spacing
The layout follows a **Fluid Grid** model with a 12-column structure, allowing the dashboard to scale from tablet to ultra-wide displays. A 16px gutter ensures that even in high-density views, content blocks remain distinct.

The spacing rhythm is based on a **4px baseline grid**. Components are grouped using logical nesting: elements within a card use 8px or 12px spacing, while the cards themselves are separated by 16px or 24px. Plenty of whitespace is maintained around the page periphery (24px) to frame the data and prevent the interface from feeling cluttered.

## Elevation & Depth
Depth is conveyed through **Ambient Shadows** and tonal layering. This design system avoids heavy borders in favor of soft, diffused shadows that lift cards off the background.

- **Level 0 (Background):** Slate-50 (#F8FAFC) - The base canvas.
- **Level 1 (Cards):** White (#FFFFFF) - Primary content containers. They feature a 4px blur, 0px Y-offset, 2px spread shadow with a low-opacity slate tint (`rgba(15, 23, 42, 0.05)`).
- **Level 2 (Dropdowns/Modals):** White (#FFFFFF) - Floating elements that require higher prominence. These use an 8px Y-offset and 16px blur with `rgba(15, 23, 42, 0.1)`.

Interactive elements like buttons use a subtle inner shadow on press to simulate physical displacement.

## Shapes
The shape language is defined by **8px (0.5rem)** rounded corners for all primary containers, including cards and modals. This radius strikes a balance between professional rigor and modern approachability. 

Small components like buttons and input fields follow the same 8px radius to maintain consistency. Status chips and tags utilize a fully rounded (pill-shaped) radius to distinguish them from interactive buttons or navigational elements.

## Components

### KPI Cards
Standardized containers for high-level metrics. They must include a primary value (Inter Bold), a descriptive label (Slate Gray), and a trend indicator (Teal for up, Amber for down). Backgrounds are strictly white with Level 1 elevation.

### Data Tables
Tables use a **Zebra Striping** pattern where even rows are filled with a subtle gray (`#F1F5F9`). Headers are sticky, using the `label-caps` typography style. Cell padding is condensed (12px vertical) to maximize data visibility.

### Interactive Charts
Charts use the specified accent colors. Hover states must trigger a vertical "guide line" and a tooltip card that follows the Level 2 elevation rules. Grid lines within charts should be faint (`#E2E8F0`).

### Refined Filter Controls
Filters are grouped in a dedicated horizontal bar above the data. They use a "Ghost" style (border only) when inactive and a "Primary" style (Blue border/text) when an active selection is made.

### Buttons
- **Primary:** Solid Blue (`#1E40AF`) with white text.
- **Secondary:** Light Blue tint with Blue text.
- **Ghost:** Transparent background with Slate text for low-priority actions.

### Input Fields
Inputs use a 1px border (`#CBD5E1`). On focus, the border transitions to Primary Blue with a subtle 2px outer glow (Blue at 10% opacity).