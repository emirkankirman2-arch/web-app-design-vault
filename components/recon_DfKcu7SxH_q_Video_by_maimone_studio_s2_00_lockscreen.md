---
title: "LockScreen — DfKcu7SxH_q_Video_by_maimone (00:07.300)"
description: "LockScreen UI component (recon_DfKcu7SxH_q_Video_by_maimone_studio_s2_00_lockscreen) with SSIM 0.9941, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_DfKcu7SxH_q_Video_by_maimone.studio_s2_00_lockscreen"
category: "LockScreen"
ssim: 0.9941
quality_score: 8.72
tags: [lockscreen, ui-design, design-tokens, react, flutter]
---

# LockScreen — DfKcu7SxH_q_Video_by_maimone (00:07.300)

> **Category:** [[07_LockScreen|LockScreen]] | **SSIM Fidelity:** `0.9941` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[03_GlassMenu|GlassMenu]], [[09_SplashAuth|SplashAuth]], [[01_Card|Card]]

Professional LockScreen reverse-engineered from DfKcu7SxH_q_Video_by_maimone.studio at 00:07.300. Features FADE_IN_SCALE micro-interaction animation with 14.91:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#140F13` | `rgb(20, 15, 19)` | `oklch(0.18 0.011 332.9)` | `23.0%` |
| `surface` | `#463D3B` | `rgb(70, 61, 59)` | `oklch(0.37 0.013 32.6)` | `22.3%` |
| `accent` | `#CDB8A9` | `rgb(205, 184, 169)` | `oklch(0.80 0.032 57.8)` | `3.1%` |
| `text` | `#F0E2D2` | `rgb(240, 226, 210)` | `oklch(0.92 0.026 71.2)` | `15.4%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `7.3 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `2.63`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
import React from 'react';
import { motion } from 'framer-motion';

interface LockScreenProps {
  className?: string;
}

export const LockScreen: React.FC<LockScreenProps> = ({ className }) => {
  const variants = {
    initial: { opacity: 0, scale: 0.95 },
    animate: { opacity: 1, scale: 1 },
  };

  const transition = {
    type: 'spring',
    stiffness: 260,
    damping: 20,
    duration: 7.3,
  };

  return (
    <motion.div
      variants={variants}
      initial="initial"
      animate="animate"
      transition={transition}
      className={
        'fixed inset-0 z-50 bg-[#140F13] text-[#F0E2D2] flex flex-col items-center justify-center p-6 overflow-hidden ' +
        className
      }
      aria-label="Lock screen"
      role="region"
    >
      {/* Card surface matching screenshot dimensions (105x171 scaled via aspect-ratio) */}
      <div
        className="relative w-full max-w-xs aspect-[105/171] bg-[#463D3B] rounded-2xl shadow-none overflow-hidden border border-white/10"
      >
        {/* Branding area at bottom-left as seen in screenshot */}
        <div className="absolute bottom-4 left-4 z-10">
          <h2 className="text-lg font-semibold text-[#F0E2D2] tracking-tight">Marlim</h2>
          <p className="text-xs text-[#CDB8A9]/80 uppercase tracking-wider mt-0.5">
            47 30304
          </p>
        </div>

        {/* Decorative subtle gradient overlay to mimic card depth */}
        <div className="absolute inset-0 bg-gradient-to-t from-black/40 to-transparent pointer-events-none" />
      <
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class LockScreen extends StatefulWidget {
  const LockScreen({Key? key}) : super(key: key);

  @override
  State<LockScreen> createState() => _LockScreenState();
}

class _LockScreenState extends State<LockScreen>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scale;
  late Animation<double> _opacity;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 7300),
    );
    // Spring-like curve approximation
    final curved = CurvedAnimation(parent: _controller, curve: Curves.easeOutBack);
    _scale = Tween<double>(begin: 0.95, end: 1.0).animate(curved);
    _opacity = Tween<double>(begin: 0.0, end: 1.0).animate(curved);
    _controller.forward();
  }

  @override
  void dispose() {
    _controller.dispose();
    super.dispose();
  }

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: const Color(0xFF140F13),
      body: Center(
        child: AnimatedBuilder(
          animation: _controller,
          builder: (context, child) {
            return Opacity(
              opacity: _opacity.value,
              child: Transform.scale(
                scale: _scale.value,
                child: child,
              ),
            );
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
