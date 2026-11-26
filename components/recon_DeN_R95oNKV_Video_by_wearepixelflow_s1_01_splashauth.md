---
title: "SplashAuth — DeN_R95oNKV_Video_by_wearepi (00:08.000)"
description: "SplashAuth UI component (recon_DeN_R95oNKV_Video_by_wearepixelflow_s1_01_splashauth) with SSIM 0.9556, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_DeN-R95oNKV_Video_by_wearepixelflow_s1_01_splashauth"
category: "SplashAuth"
ssim: 0.9556
quality_score: 8.72
tags: [splashauth, ui-design, design-tokens, react, flutter]
---

# SplashAuth — DeN_R95oNKV_Video_by_wearepi (00:08.000)

> **Category:** [[09_SplashAuth|SplashAuth]] | **SSIM Fidelity:** `0.9556` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[06_Input|Input]], [[07_LockScreen|LockScreen]], [[05_Hero|Hero]]

Professional SplashAuth reverse-engineered from DeN-R95oNKV_Video_by_wearepixelflow at 00:08.000. Features FADE_IN_SCALE micro-interaction animation with 5.69:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#000000` | `rgb(0, 0, 0)` | `oklch(0.00 0.000 0.0)` | `55.3%` |
| `surface` | `#81858F` | `rgb(129, 133, 143)` | `oklch(0.62 0.016 268.4)` | `0.6%` |
| `accent` | `#A30D2D` | `rgb(163, 13, 45)` | `oklch(0.46 0.177 19.0)` | `0.6%` |
| `text` | `#81858F` | `rgb(129, 133, 143)` | `oklch(0.62 0.016 268.4)` | `0.6%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `2.0 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react'
import { motion } from 'framer-motion'

interface SplashAuthProps {
  onSignIn?: () => void
  onCreateAccount?: () => void
  onForgotPassword?: () => void
}

export const SplashAuth: React.FC<SplashAuthProps> = ({
  onSignIn,
  onCreateAccount,
  onForgotPassword,
}) => {
  return (
    <motion.div
      initial={{ opacity: 0, scale: 0.95 }}
      animate={{ opacity: 1, scale: 1 }}
      transition={{ type: 'spring', stiffness: 260, damping: 20 }}
      className="fixed inset-0 z-50 flex items-center justify-center bg-black"
    >
      <div className="relative w-[221px] h-[284px] rounded-[28px] bg-black/80 border border-white/10 p-6 shadow-2xl overflow-hidden">
        {/* Neon border glow effect */}
        <div className="absolute inset-0 rounded-[28px] border border-cyan-500/30 blur-[8px] pointer-events-none" />

        {/* Header */}
        <div className="flex items-center gap-2 mb-6">
          <div className="w-3 h-3 rounded-full bg-cyan-400 animate-pulse" />
          <span className="text-sm font-medium text-white tracking-tight">ArcLine</span>
        </div>

        {/* Auth Tabs */}
        <div className="flex gap-2 mb-8">
          <button
            onClick={onSignIn}
            className="flex-1 py-2 rounded-lg bg-blue-600 text-white text-xs font-medium shadow-lg shadow-blue-500/30"
          >
            Sign in
          </button>
          <button
            onClick={onCreateAccount}
            className="flex-1 py-2 rounded-lg bg-white/5 text-gray-400 text-xs font-medium hover:bg-white/10 transition"
          >
        
```

## 4. Flutter / Dart Implementation

```dart
// Flutter Material widget template
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
