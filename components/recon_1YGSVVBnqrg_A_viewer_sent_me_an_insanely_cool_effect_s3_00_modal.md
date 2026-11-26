---
title: "Modal — 1YGSVVBnqrg_A_viewer_sent_me (04:28.533)"
description: "Modal UI component (recon_1YGSVVBnqrg_A_viewer_sent_me_an_insanely_cool_effect_s3_00_modal) with SSIM 0.995, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_1YGSVVBnqrg_A_viewer_sent_me_an_insanely_cool_effect_s3_00_modal"
category: "Modal"
ssim: 0.995
quality_score: 8.72
tags: [modal, ui-design, design-tokens, react, flutter]
---

# Modal — 1YGSVVBnqrg_A_viewer_sent_me (04:28.533)

> **Category:** [[08_Modal|Modal]] | **SSIM Fidelity:** `0.995` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[02_Button|Button]], [[06_Input|Input]], [[01_Card|Card]]

Professional Modal reverse-engineered from 1YGSVVBnqrg_A_viewer_sent_me_an_insanely_cool_effect at 04:28.533. Features FADE_IN_SCALE micro-interaction animation with 11.71:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#0C0D08` | `rgb(12, 13, 8)` | `oklch(0.16 0.011 116.6)` | `90.9%` |
| `surface` | `#757272` | `rgb(117, 114, 114)` | `oklch(0.55 0.004 17.3)` | `0.2%` |
| `accent` | `#CDC8BF` | `rgb(205, 200, 191)` | `oklch(0.83 0.014 82.4)` | `0.1%` |
| `text` | `#CDC8BF` | `rgb(205, 200, 191)` | `oklch(0.83 0.014 82.4)` | `0.1%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `44.167 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `0.52`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react'
import { motion } from 'framer-motion'

interface ModalProps {
  isOpen: boolean
  onClose: () => void
}

export const Modal: React.FC<ModalProps> = ({ isOpen, onClose }) => {
  if (!isOpen) return null

  return (
    <div
      className="fixed inset-0 z-50 flex items-center justify-center"
      role="dialog"
      aria-modal="true"
      aria-label="Image rotation modal"
    >
      {/* Backdrop */}
      <motion.div
        initial={{ opacity: 0 }}
        animate={{ opacity: 1 }}
        exit={{ opacity: 0 }}
        className="absolute inset-0 bg-black/80 backdrop-blur-sm"
        onClick={onClose}
      />

      {/* Modal Container */}
      <motion.div
        initial={{ opacity: 0, scale: 0.95 }}
        animate={{ opacity: 1, scale: 1 }}
        exit={{ opacity: 0, scale: 0.95 }}
        transition={
          type: 'spring',
          stiffness: 260,
          damping: 20
        }
        className="relative w-[672px] h-[675px] bg-[#0C0D08] rounded-[28px] shadow-2xl border border-white/10 overflow-hidden"
      >
        {/* Close Button */}
        <button
          onClick={onClose}
          className="absolute top-6 right-6 w-8 h-8 rounded-full bg-white/10 hover:bg-white/20 transition-colors flex items-center justify-center text-white"
          aria-label="Close modal"
        >
          <svg className="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path strokeLinecap="round" strokeLinejoin="round" strokeWidth={2} d="M6 18L18 6M6 6l12 12" />
          </svg>
        </button>

        {/* Content Ar
```

## 4. Flutter / Dart Implementation

```dart
// Flutter Material widget template
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
