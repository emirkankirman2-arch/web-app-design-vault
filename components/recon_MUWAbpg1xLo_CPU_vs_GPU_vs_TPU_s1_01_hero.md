---
title: "Hero — MUWAbpg1xLo_CPU_vs_GPU_vs_TP (00:08.360)"
description: "Hero UI component (recon_MUWAbpg1xLo_CPU_vs_GPU_vs_TPU_s1_01_hero) with SSIM 0.9937, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_MUWAbpg1xLo_CPU_vs_GPU_vs_TPU_s1_01_hero"
category: "Hero"
ssim: 0.9937
quality_score: 8.72
tags: [hero, ui-design, design-tokens, react, flutter]
---

# Hero — MUWAbpg1xLo_CPU_vs_GPU_vs_TP (00:08.360)

> **Category:** [[05_Hero|Hero]] | **SSIM Fidelity:** `0.9937` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[10_ShaderCanvas|ShaderCanvas]], [[02_Button|Button]], [[04_Navbar|Navbar]]

Professional Hero reverse-engineered from MUWAbpg1xLo_CPU_vs_GPU_vs_TPU at 00:08.360. Features FADE_IN_SCALE micro-interaction animation with 8.81:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#252525` | `rgb(37, 37, 37)` | `oklch(0.26 0.000 89.9)` | `86.5%` |
| `surface` | `#374C48` | `rgb(55, 76, 72)` | `oklch(0.40 0.027 181.9)` | `5.6%` |
| `accent` | `#DCC52C` | `rgb(220, 197, 44)` | `oklch(0.82 0.159 100.1)` | `0.9%` |
| `text` | `#DCC52C` | `rgb(220, 197, 44)` | `oklch(0.82 0.159 100.1)` | `0.9%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `51.68 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
import React from 'react';
import { motion } from 'framer-motion';

interface HeroProps {
  className?: string;
}

export const Hero: React.FC<HeroProps> = ({ className }) => {
  return (
    <section
      className={
        'relative w-full h-[438px] bg-[#252525] overflow-hidden ' + (className || '')
      }
    >
      {/* Background grid / subtle texture */}
      <div className="absolute inset-0 opacity-10 bg-[url('https://grainy-gradients.vercel.app/noise.svg')] pointer-events-none" />

      {/* Title */}
      <div className="absolute top-6 left-6 z-10">
        <h2 className="text-xl font-semibold text-white tracking-tight">GPU vs TPU</h2>
      </div>

      {/* Logo */}
      <div className="absolute top-6 right-6 z-10">
        <div className="flex items-center gap-2 text-white text-sm font-medium">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            className="h-5 w-5 text-[#DCC52C]"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
          >
            <path
              strokeLinecap="round"
              strokeLinejoin="round"
              strokeWidth={2}
              d="M9 19v-6a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2a2 2 0 002-2zm0 0V9a2 2 0 012-2h2a2 2 0 012 2v10m-6 0a2 2 0 002 2h2a2 2 0 002-2m0 0V5a2 2 0 012-2h2a2 2 0 012 2v14a2 2 0 01-2 2h-2a2 2 0 01-2-2z"
            />
          </svg>
          ByteIQ
        </div>
      </div>

      {/* Diagram container */}
      <motion.div
        initial={{ opacity: 0, scale: 0.95 }}
    
```

## 4. Flutter / Dart Implementation

```dart
// Flutter Material widget template
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
