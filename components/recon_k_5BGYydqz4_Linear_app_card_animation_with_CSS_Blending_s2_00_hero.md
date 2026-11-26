---
title: "Hero — k_5BGYydqz4_Linear_app_card_ (00:29.400)"
description: "Hero UI component (recon_k_5BGYydqz4_Linear_app_card_animation_with_CSS_Blending_s2_00_hero) with SSIM 0.9918, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_k-5BGYydqz4_Linear.app_card_animation_with_CSS_Blending_s2_00_hero"
category: "Hero"
ssim: 0.9918
quality_score: 8.72
tags: [hero, ui-design, design-tokens, react, flutter]
---

# Hero — k_5BGYydqz4_Linear_app_card_ (00:29.400)

> **Category:** [[05_Hero|Hero]] | **SSIM Fidelity:** `0.9918` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[10_ShaderCanvas|ShaderCanvas]], [[02_Button|Button]], [[04_Navbar|Navbar]]

Professional Hero reverse-engineered from k-5BGYydqz4_Linear.app_card_animation_with_CSS_Blending at 00:29.400. Features FADE_IN_SCALE micro-interaction animation with 19.98:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#FDFDFD` | `rgb(253, 253, 253)` | `oklch(0.99 0.000 89.9)` | `51.4%` |
| `surface` | `#02031D` | `rgb(2, 3, 29)` | `oklch(0.12 0.059 270.6)` | `19.3%` |
| `accent` | `#0A0B37` | `rgb(10, 11, 55)` | `oklch(0.19 0.083 273.9)` | `7.1%` |
| `text` | `#02031D` | `rgb(2, 3, 29)` | `oklch(0.12 0.059 270.6)` | `19.3%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `6.267 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.41`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
// Reverse-engineered Hero component from video k-5BGYydqz4_Linear.app_card_animation_with_CSS_Blending.mp4
import React from 'react';
import { motion } from 'framer-motion';

export interface HeroSpotlightCardProps {
  className?: string;
}

export const HeroSpotlightCard: React.FC<HeroSpotlightCardProps> = ({ className }) => {
  const containerVariants = {
    hidden: { opacity: 0, scale: 0.95 },
    visible: {
      opacity: 1,
      scale: 1,
      transition: {
        type: 'spring',
        stiffness: 260,
        damping: 20,
        duration: 6.266,
      },
    },
  };

  return (
    <section
      className={
        'relative flex flex-col items-center justify-center min-h-screen bg-[#FDFDFD] text-[#02031D] font-sans ' +
        (className ?? '')
      }
    >
      <motion.div
        initial="hidden"
        animate="visible"
        variants={containerVariants}
        className="relative w-full max-w-[720px] h-[720px] rounded-[12px] overflow-hidden shadow-lg"
      >
        {/* Background surface */}
        <div className="absolute inset-0 bg-[#02031D]" />

        {/* Spotlight overlay using CSS blend mode */}
        <div
          className="absolute inset-0 bg-gradient-to-br from-[#0A0B37] via-transparent to-[#02031D] mix-blend-soft-light opacity-80"
        />

        {/* Card content */}
        <div className="absolute inset-0 flex flex-col items-center justify-center p-8 text-center z-10">
          <h1
            className="text-4xl font-bold tracking-tight text-white mb-2 drop-shadow-md"
     
```

## 4. Flutter / Dart Implementation

```dart
// Flutter Material widget template
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
