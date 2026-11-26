---
title: "LockScreen — UYUAaAfvdA_Demo_video_of_my_ (00:00.000)"
description: "LockScreen UI component (recon_UYUAaAfvdA_Demo_video_of_my_most_ambitious_product_s1_00_lockscree) with SSIM 0.9848, OKLCH design tokens, SLIDE_UP motion spec, React/Tailwind & Flutter implementations."
component_id: "recon__UYUAaAfvdA_Demo_video_of_my_most_ambitious_product_s1_00_lockscreen"
category: "LockScreen"
ssim: 0.9848
quality_score: 8.72
tags: [lockscreen, ui-design, design-tokens, react, flutter]
---

# LockScreen — UYUAaAfvdA_Demo_video_of_my_ (00:00.000)

> **Category:** [[07_LockScreen|LockScreen]] | **SSIM Fidelity:** `0.9848` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[03_GlassMenu|GlassMenu]], [[09_SplashAuth|SplashAuth]], [[01_Card|Card]]

Professional LockScreen reverse-engineered from _UYUAaAfvdA_Demo_video_of_my_most_ambitious_product at 00:00.000. Features SLIDE_UP micro-interaction animation with 8.38:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#0C050C` | `rgb(12, 5, 12)` | `oklch(0.13 0.022 326.7)` | `38.9%` |
| `surface` | `#726B75` | `rgb(114, 107, 117)` | `oklch(0.54 0.018 315.9)` | `6.7%` |
| `accent` | `#A193F2` | `rgb(161, 147, 242)` | `oklch(0.71 0.136 289.2)` | `5.0%` |
| `text` | `#8BA7E3` | `rgb(139, 167, 227)` | `oklch(0.73 0.093 264.9)` | `3.8%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `SLIDE_UP`
- **Measured Duration:** `67.067 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `0.31`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
import React, { useState, useEffect } from 'react';
import { motion } from 'framer-motion';
import { Lock, Clock, User, Shield, ArrowRight } from 'lucide-react';

interface LockScreenProps {
  onUnlock?: () => void;
  className?: string;
}

export const LockScreen: React.FC<LockScreenProps> = ({ onUnlock, className }) => {
  const [time, setTime] = useState(new Date());
  const [isUnlocking, setIsUnlocking] = useState(false);

  useEffect(() => {
    const timer = setInterval(() => setTime(new Date()), 1000);
    return () => clearInterval(timer);
  }, []);

  const handleUnlock = () => {
    setIsUnlocking(true);
    setTimeout(() => {
      setIsUnlocking(false);
      onUnlock?.();
    }, 600);
  };

  const formatTime = (date: Date) => {
    return date.toLocaleTimeString('tr-TR', { hour: '2-digit', minute: '2-digit' });
  };

  const formatDate = (date: Date) => {
    return date.toLocaleDateString('tr-TR', { weekday: 'long', year: 'numeric', month: 'long', day: 'numeric' });
  };

  return (
    <motion.div
      initial={{ opacity: 0, y: 9.85 }}
      animate={{ opacity: 1, y: 0 }}
      transition={{ duration: 67.07, ease: [0.16, 1, 0.3, 1] }}
      className={
        'fixed inset-0 z-50 bg-[#0C050C] flex flex-col items-center justify-center p-6 ' +
        className
      }
    >
      {/* Lock Screen Card */}
      <motion.div
        whileHover={{ scale: 1.02 }}
        className={
          'w-full max-w-md bg-[#726B75]/10 backdrop-blur-xl border border-white/10 rounded-[28px] p-8 shadow-2xl overflow-hidden rel
```

## 4. Flutter / Dart Implementation

```dart
// Flutter Material widget template
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
