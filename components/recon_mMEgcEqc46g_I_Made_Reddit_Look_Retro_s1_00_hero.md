---
title: "Hero — mMEgcEqc46g_I_Made_Reddit_Lo (00:00.000)"
description: "Hero UI component (recon_mMEgcEqc46g_I_Made_Reddit_Look_Retro_s1_00_hero) with SSIM 0.992, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_mMEgcEqc46g_I_Made_Reddit_Look_Retro_s1_00_hero"
category: "Hero"
ssim: 0.992
quality_score: 8.72
tags: [hero, ui-design, design-tokens, react, flutter]
---

# Hero — mMEgcEqc46g_I_Made_Reddit_Lo (00:00.000)

> **Category:** [[05_Hero|Hero]] | **SSIM Fidelity:** `0.992` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[10_ShaderCanvas|ShaderCanvas]], [[02_Button|Button]], [[04_Navbar|Navbar]]

Professional Hero reverse-engineered from mMEgcEqc46g_I_Made_Reddit_Look_Retro at 00:00.000. Features FADE_IN_SCALE micro-interaction animation with 17.37:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#000000` | `rgb(0, 0, 0)` | `oklch(0.00 0.000 0.0)` | `78.4%` |
| `surface` | `#727376` | `rgb(114, 115, 118)` | `oklch(0.56 0.005 271.3)` | `2.2%` |
| `accent` | `#28E762` | `rgb(40, 231, 98)` | `oklch(0.81 0.228 147.6)` | `2.7%` |
| `text` | `#E7EAEB` | `rgb(231, 234, 235)` | `oklch(0.94 0.004 219.5)` | `1.4%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `23.767 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.84`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
// Reconstructed Hero component from video evidence
// Source: mMEgcEqc46g_I_Made_Reddit_Look_Retro.mp4 (DESKTOP view at 00:00.000)

import React from 'react'
import { motion } from 'framer-motion'

interface HeroProps {
  className?: string
}

export const Hero: React.FC<HeroProps> = ({ className }) => {
  const heroMotion = {
    initial: { opacity: 0, scale: 0.95 },
    animate: { opacity: 1, scale: 1 },
    transition: {
      type: 'spring',
      stiffness: 260,
      damping: 20,
      duration: 23.766,
    },
  }

  return (
    <section
      className={
        'relative w-full h-screen bg-black overflow-hidden flex items-center justify-center ' +
        className
      }
    >
      {/* Starfield background */}
      <div className="absolute inset-0 z-0" />

      {/* Hero content */}
      <motion.div className="relative z-10 flex flex-col items-center justify-center text-center px-4" {...heroMotion}>
        <h1
          className={
            'text-6xl md:text-8xl font-bold text-white tracking-tight leading-tight mb-8 ' +
            'bg-clip-text text-transparent bg-gradient-to-r from-white via-gray-300 to-gray-500'
          }
        >
          Retro Reddit
        </h1>

        <p
          className={
            'text-xl md:text-2xl text-gray-300 max-w-2xl mb-12 leading-relaxed'
          }
        >
          Experience the classic forum feel with modern performance.
        </p>

        <div className="flex gap-4">
          <button
            className={
              'px-8 py-3 bg-green-500 ho
```

## 4. Flutter / Dart Implementation

```dart
// Flutter Material widget template
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
