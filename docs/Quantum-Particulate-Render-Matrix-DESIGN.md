---
version: "alpha"
name: "Quantum Particulate — Render Matrix"
description: "Quantum Particulate Dashboard Section is designed for demonstrating application workflows and interface hierarchy. Key features include clear information density, modular panels, and interface rhythm. It is suitable for product showcases, admin panels, and analytics experiences."
colors:
  primary: "#8B5CF6"
  secondary: "#27272A"
  tertiary: "#FB61FB"
  neutral: "#27272A"
  background: "#FAFAFA"
  surface: "#8B5CF6"
  text-primary: "#27272A"
  text-secondary: "#18181B"
  border: "#E4E4E7"
  accent: "#8B5CF6"
typography:
  display-lg:
    fontFamily: "Inter"
    fontSize: "72px"
    fontWeight: 300
    lineHeight: "72px"
    letterSpacing: "-0.05em"
  body-md:
    fontFamily: "Inter"
    fontSize: "12px"
    fontWeight: 500
    lineHeight: "16px"
spacing:
  base: "4px"
  sm: "4px"
  md: "6px"
  lg: "12px"
  xl: "16px"
  gap: "8px"
  card-padding: "9px"
  section-padding: "32px"
---

## Overview

- **Composition cues:**
  - Layout: Grid
  - Content Width: Bounded
  - Framing: Open
  - Grid: Strong

## Colors

The color system uses light mode with #8B5CF6 as the main accent and #27272A as the neutral foundation.

- **Primary (#8B5CF6):** Main accent and emphasis color.
- **Secondary (#27272A):** Supporting accent for secondary emphasis.
- **Tertiary (#FB61FB):** Reserved accent for supporting contrast moments.
- **Neutral (#27272A):** Neutral foundation for backgrounds, surfaces, and supporting chrome.

- **Usage:** Background: #FAFAFA; Surface: #8B5CF6; Text Primary: #27272A; Text Secondary: #18181B; Border: #E4E4E7; Accent: #8B5CF6

## Typography

Typography relies on Inter across display, body, and utility text.

- **Display (`display-lg`):** Inter, 72px, weight 300, line-height 72px, letter-spacing -0.05em.
- **Body (`body-md`):** Inter, 12px, weight 500, line-height 16px.

## Layout

Layout follows a grid composition with reusable spacing tokens. Preserve the grid, bounded structural frame before changing ornament or component styling. Use 4px as the base rhythm and let larger gaps step up from that cadence instead of introducing unrelated spacing values.

Treat the page as a grid / bounded composition, and keep that framing stable when adding or remixing sections.

- **Layout type:** Grid
- **Content width:** Bounded
- **Base unit:** 4px
- **Scale:** 4px, 6px, 12px, 16px, 24px, 32px, 48px, 64px
- **Section padding:** 32px, 40px, 64px
- **Card padding:** 9px, 32px, 64px
- **Gaps:** 8px, 12px, 16px, 24px

## Elevation & Depth

Depth is communicated through elevated, border contrast, and reusable shadow or blur treatments. Keep those recipes consistent across hero panels, cards, and controls so the page reads as one material system.

Surfaces should read as elevated first, with borders, shadows, and blur only reinforcing that material choice.

- **Surface style:** Elevated
- **Borders:** 1px #E4E4E7; 1px #F4F4F5; 1px #27272A
- **Shadows:** rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.03) 20px 0px 40px 0px; rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0) 0px 0px 0px 0px, rgba(0, 0, 0, 0.05) 0px 1px 2px 0px

### Techniques
- **Gradient border shell:** Use a thin gradient border shell around the main card. Wrap the surface in an outer shell with 0px padding and a 0px radius. Drive the shell with linear-gradient(to right, rgb(228, 228, 231) 1px, rgba(0, 0, 0, 0) 1px), linear-gradient(rgb(228, 228, 231) 1px, rgba(0, 0, 0, 0) 1px) so the edge reads like premium depth instead of a flat stroke. Keep the actual stroke understated so the gradient shell remains the hero edge treatment. Inset the real content surface inside the wrapper with a slightly smaller radius so the gradient only appears as a hairline frame.

## Shapes

Shapes rely on a tight radius system anchored by 6px and scaled across cards, buttons, and supporting surfaces. Icon geometry should stay compatible with that soft-to-controlled silhouette.

Use the radius family intentionally: larger surfaces can open up, but controls and badges should stay within the same rounded DNA instead of inventing sharper or pill-only exceptions.

- **Corner radii:** 6px, 16px, 9999px
- **Icon treatment:** Linear
- **Icon sets:** Solar

## Components

Component styling should inherit the shared button, icon, spacing, and surface rules instead of inventing one-off treatments. Favor a small family of repeatable patterns for actions, content containers, and fields.

### Iconography
- **Treatment:** Linear.
- **Sets:** Solar.

## Do's and Don'ts

Use these constraints to keep future generations aligned with the current system instead of drifting into adjacent styles.

### Do
- Do use the primary palette as the main accent for emphasis and action states.
- Do keep spacing aligned to the detected 4px rhythm.
- Do reuse the Elevated surface treatment consistently across cards and controls.
- Do keep corner radii within the detected 6px, 16px, 9999px family.

### Don't
- Don't introduce extra accent colors outside the core palette roles unless the page needs a new semantic state.
- Don't mix unrelated shadow or blur recipes that break the current depth system.
- Don't exceed the detected minimal motion intensity without a deliberate reason.

## Motion

Motion stays restrained and interface-led across text, layout, and scroll transitions. Timing clusters around 2000ms. Easing favors ease and cubic-bezier(0.4. Scroll choreography uses GSAP ScrollTrigger for section reveals and pacing.

**Motion Level:** minimal

**Durations:** 2000ms

**Easings:** ease, cubic-bezier(0.4, 0, 0.6, 1)

**Scroll Patterns:** gsap-scrolltrigger

## WebGL

Reconstruct the graphics as a inset canvas accent using alpha, antialias, custom shaders. The effect should read as retro-futurist, technical, and meditative: dot-matrix particle field with indigo on white and sparse spacing. Build it from dot particles + soft depth fade so the effect reads clearly. Animate it as slow breathing pulse. Interaction can react to the pointer, but only as a subtle drift. Preserve reduced motion + dom fallback.

**Id:** webgl

**Label:** WebGL

**Stack:** WebGL

**Insights:**
  - **Scene:**
    - **Value:** Inset canvas accent
  - **Effect:**
    - **Value:** Dot-matrix particle field
  - **Primitives:**
    - **Value:** Dot particles + soft depth fade
  - **Motion:**
    - **Value:** Slow breathing pulse
  - **Interaction:**
    - **Value:** Pointer-reactive drift
  - **Render:**
    - **Value:** alpha, antialias, custom shaders

**Techniques:** Dot matrix, Breathing pulse, Pointer parallax, Shader gradients, DOM fallback

**Code Evidence:**
  - **HTML reference:**
    - **Language:** html
    - **Snippet:**
      ```html
      <!-- Canvas -->
      <div class="absolute inset-0 z-10 overflow-hidden flex items-center justify-center">
          <canvas id="gl" class="w-full h-full block opacity-90"></canvas>
      </div>
      ```
