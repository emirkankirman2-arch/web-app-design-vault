---
title: "SplashAuth — DeEzPEXNDRw_Video_by_wearepi (00:00.000)"
description: "SplashAuth UI component (recon_DeEzPEXNDRw_Video_by_wearepixelflow_s1_02_splashauth) with SSIM 0.9542, OKLCH design tokens, FADE_AND_SLIDE_UP motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_DeEzPEXNDRw_Video_by_wearepixelflow_s1_02_splashauth"
category: "SplashAuth"
ssim: 0.9542
quality_score: 8.72
tags: [splashauth, ui-design, design-tokens, react, flutter]
---

# SplashAuth — DeEzPEXNDRw_Video_by_wearepi (00:00.000)

> **Category:** [[09_SplashAuth|SplashAuth]] | **SSIM Fidelity:** `0.9542` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[06_Input|Input]], [[07_LockScreen|LockScreen]], [[05_Hero|Hero]]

Professional SplashAuth reverse-engineered from DeEzPEXNDRw_Video_by_wearepixelflow at 00:00.000. Features FADE_AND_SLIDE_UP micro-interaction animation with 17.57:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#000000` | `rgb(0, 0, 0)` | `oklch(0.00 0.000 0.0)` | `54.2%` |
| `surface` | `#3A2E3D` | `rgb(58, 46, 61)` | `oklch(0.32 0.031 319.5)` | `5.1%` |
| `accent` | `#EFD045` | `rgb(239, 208, 69)` | `oklch(0.86 0.155 96.2)` | `1.1%` |
| `text` | `#ECE9F7` | `rgb(236, 233, 247)` | `oklch(0.94 0.019 295.9)` | `12.0%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_AND_SLIDE_UP`
- **Measured Duration:** `0.45 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `120.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react'
import { motion } from 'framer-motion'

interface SplashAuthProps {
  onSubmit?: (data: { name: string; email: string; project: string; type: string }) => void
  onClose?: () => void
}

export const SplashAuth: React.FC<SplashAuthProps> = ({ onSubmit, onClose }) => {
  const [formData, setFormData] = React.useState({
    name: '',
    email: '',
    project: '',
    type: 'Website'
  })

  const handleSubmit = (e: React.FormEvent) => {
    e.preventDefault()
    onSubmit?.(formData)
  }

  return (
    <motion.div
      initial={{ opacity: 0, y: 24 }}
      animate={{ opacity: 1, y: 0 }}
      transition={{ duration: 0.45, ease: [0.16, 1, 0.3, 1] }}
      className="fixed inset-0 z-50 flex items-center justify-center bg-black/80 backdrop-blur-sm"
    >
      <motion.div
        initial={{ opacity: 0, scale: 0.9 }}
        animate={{ opacity: 1, scale: 1 }}
        transition={{ duration: 0.45, ease: [0.16, 1, 0.3, 1] }}
        className="w-[244px] h-[300px] bg-[#3A2E3D] rounded-[28px] p-6 text-[#ECE9F7] shadow-2xl relative overflow-hidden"
      >
        {/* Pikachu mascot overlay */}
        <div className="absolute -top-16 left-1/2 -translate-x-1/2 w-32 h-32 flex items-center justify-center">
          <div className="relative w-full h-full">
            <div className="absolute inset-0 bg-yellow-400 rounded-full blur-xl opacity-50 animate-pulse"></div>
            <div className="relative z-10 w-24 h-24 bg-yellow-400 rounded-full flex items-center justify-center shadow-[0_0_20px_rgba(239,208,69,0.6)]">
              <svg className="w-16 h-16 t
```

## 4. Flutter / Dart Implementation

```dart
// Flutter Material widget template
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
