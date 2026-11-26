---
title: "Hero — 1FurWDiK9A4_Did_Anthropic_ju (02:21.850)"
description: "Hero UI component (recon_1FurWDiK9A4_Did_Anthropic_just_save_its_1_trillion_IPO_s2_00_hero) with SSIM 0.9928, OKLCH design tokens, SLIDE_DOWN motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_1FurWDiK9A4_Did_Anthropic_just_save_its_1_trillion_IPO_s2_00_hero"
category: "Hero"
ssim: 0.9928
quality_score: 8.72
tags: [hero, ui-design, design-tokens, react, flutter]
---

# Hero — 1FurWDiK9A4_Did_Anthropic_ju (02:21.850)

> **Category:** [[05_Hero|Hero]] | **SSIM Fidelity:** `0.9928` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[10_ShaderCanvas|ShaderCanvas]], [[02_Button|Button]], [[04_Navbar|Navbar]]

Professional Hero reverse-engineered from 1FurWDiK9A4_Did_Anthropic_just_save_its_1_trillion_IPO at 02:21.850. Features SLIDE_DOWN micro-interaction animation with 18.35:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#F9F8F4` | `rgb(249, 248, 244)` | `oklch(0.98 0.005 95.1)` | `53.6%` |
| `surface` | `#C2CEC7` | `rgb(194, 206, 199)` | `oklch(0.84 0.016 160.6)` | `13.2%` |
| `accent` | `#ACB3AE` | `rgb(172, 179, 174)` | `oklch(0.76 0.011 155.0)` | `3.5%` |
| `text` | `#0E0C0D` | `rgb(14, 12, 13)` | `oklch(0.16 0.004 345.8)` | `14.0%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `SLIDE_DOWN`
- **Measured Duration:** `25.359 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `2.75`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react'
import { motion } from 'framer-motion'

interface HeroProps {
  className?: string
}

export const Hero: React.FC<HeroProps> = ({ className }) => {
  const motionVariants = {
    initial: { opacity: 0, y: -8.088949203491211 },
    animate: { opacity: 1, y: 0 },
    transition: {
      duration: 25.36,
      ease: [0.16, 1, 0.3, 1]
    }
  }

  return (
    <section
      className={
        'relative w-full min-h-screen bg-[#F9F8F4] text-[#0E0C0D] overflow-hidden ' + (className || '')
      }
    >
      <motion.div
        variants={motionVariants}
        initial="initial"
        animate="animate"
        transition={motionVariants.transition}
        className="absolute inset-0 z-0"
      >
        {/* Decorative background elements matching surface/accent palette */}
        <div className="absolute top-0 left-1/4 w-96 h-96 bg-[#C2CEC7]/40 rounded-full blur-3xl" />
        <div className="absolute bottom-0 right-1/4 w-80 h-80 bg-[#ACB3AE]/30 rounded-full blur-3xl" />
      </motion.div>

      <div className="relative z-10 max-w-7xl mx-auto px-6 py-12 md:py-24">
        <motion.div
          className="text-center"
          initial={{ opacity: 0, y: 20 }}
          animate={{ opacity: 1, y: 0 }}
          transition={{ duration: 0.8, ease: 'easeOut' }}
        >
          <h1
            className="text-5xl md:text-7xl font-bold tracking-tight text-[#0E0C0D] mb-6"
          >
            Next-Gen AI Benchmarks
          </h1>
          <p className="text-lg md:text-xl text-[#0E0C0D]/80 max-w-2xl mx-auto mb-10 leading-relaxed">
            Com
```

## 4. Flutter / Dart Implementation

```dart
// Flutter Material widget template
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
