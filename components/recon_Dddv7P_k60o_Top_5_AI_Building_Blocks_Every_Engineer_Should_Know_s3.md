---
title: "Hero — Dddv7P_k60o_Top_5_AI_Buildin (04:00.240)"
description: "Hero UI component (recon_Dddv7P_k60o_Top_5_AI_Building_Blocks_Every_Engineer_Should_Know_s3) with SSIM 0.9962, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_Dddv7P_k60o_Top_5_AI_Building_Blocks_Every_Engineer_Should_Know_s3_01_hero"
category: "Hero"
ssim: 0.9962
quality_score: 8.72
tags: [hero, ui-design, design-tokens, react, flutter]
---

# Hero — Dddv7P_k60o_Top_5_AI_Buildin (04:00.240)

> **Category:** [[05_Hero|Hero]] | **SSIM Fidelity:** `0.9962` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[10_ShaderCanvas|ShaderCanvas]], [[02_Button|Button]], [[04_Navbar|Navbar]]

Professional Hero reverse-engineered from Dddv7P_k60o_Top_5_AI_Building_Blocks_Every_Engineer_Should_Know at 04:00.240. Features FADE_IN_SCALE micro-interaction animation with 5.93:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#202020` | `rgb(32, 32, 32)` | `oklch(0.24 0.000 89.9)` | `89.2%` |
| `surface` | `#333F37` | `rgb(51, 63, 55)` | `oklch(0.35 0.021 156.0)` | `4.2%` |
| `accent` | `#601B7E` | `rgb(96, 27, 126)` | `oklch(0.38 0.160 313.1)` | `0.6%` |
| `text` | `#9C9C9B` | `rgb(156, 156, 155)` | `oklch(0.69 0.001 106.4)` | `1.0%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `52.552 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `0.7`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react'
import { motion } from 'framer-motion'

interface HeroProps {
  className?: string
}

export const Hero: React.FC<HeroProps> = ({ className }) => {
  const containerVariants = {
    hidden: { opacity: 0, scale: 0.95 },
    visible: {
      opacity: 1,
      scale: 1,
      transition: {
        type: 'spring',
        stiffness: 260,
        damping: 20,
        duration: 0.52552
      }
    }
  }

  return (
    <section
      className={
        'relative w-full h-[458px] bg-[#202020] flex items-center justify-center overflow-hidden ' +
        className
      }
    >
      <motion.div
        variants={containerVariants}
        initial="hidden"
        animate="visible"
        className="absolute inset-0 z-0"
      />
      <div className="relative z-10 max-w-7xl mx-auto px-6 text-center">
        <div className="flex justify-between items-start mb-8 gap-4">
          <div className="flex gap-2">
            <span className="px-3 py-1 rounded bg-white/10 border border-white/20 text-white text-sm font-medium">
              The
            </span>
            <span className="px-3 py-1 rounded bg-white/10 border border-white/20 text-white text-sm font-medium">
              ball
            </span>
            <span className="px-3 py-1 rounded bg-white/10 border border-white/20 text-white text-sm font-medium">
              falls
            </span>
          </div>
          <div className="flex items-center gap-2">
            <span className="px-3 py-1 rounded bg-[#333F37] border border-[#601B7E]/30 text-[#9C9C9B] text-sm font-medium">
    
```

## 4. Flutter / Dart Implementation

```dart
// Flutter Material widget template
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
