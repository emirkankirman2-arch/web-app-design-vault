---
title: "LockScreen — 5zl1jJGCzVI_Visually_explain (00:38.000)"
description: "LockScreen UI component (recon_5zl1jJGCzVI_Visually_explained_Bundling_in_60_seconds_s3_05_locksc) with SSIM 0.9937, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_5zl1jJGCzVI_Visually_explained_-_Bundling_in_60_seconds_s3_05_lockscreen"
category: "LockScreen"
ssim: 0.9937
quality_score: 8.72
tags: [lockscreen, ui-design, design-tokens, react, flutter]
---

# LockScreen — 5zl1jJGCzVI_Visually_explain (00:38.000)

> **Category:** [[07_LockScreen|LockScreen]] | **SSIM Fidelity:** `0.9937` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[03_GlassMenu|GlassMenu]], [[09_SplashAuth|SplashAuth]], [[01_Card|Card]]

Professional LockScreen reverse-engineered from 5zl1jJGCzVI_Visually_explained_-_Bundling_in_60_seconds at 00:38.000. Features FADE_IN_SCALE micro-interaction animation with 4.65:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#000000` | `rgb(0, 0, 0)` | `oklch(0.00 0.000 0.0)` | `90.7%` |
| `surface` | `#3A3534` | `rgb(58, 53, 52)` | `oklch(0.33 0.007 31.1)` | `1.0%` |
| `accent` | `#030102` | `rgb(3, 1, 2)` | `oklch(0.08 0.013 345.0)` | `5.0%` |
| `text` | `#787676` | `rgb(120, 118, 118)` | `oklch(0.57 0.002 17.2)` | `0.1%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `14.0 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react'
import { motion } from 'framer-motion'

interface LockScreenProps {
  className?: string
}

export const LockScreen: React.FC<LockScreenProps> = ({ className }) => {
  const motionVariants = {
    initial: { opacity: 0, scale: 0.95 },
    animate: { opacity: 1, scale: 1 },
    transition: { type: 'spring', stiffness: 260, damping: 20 }
  }

  return (
    <motion.div
      variants={motionVariants}
      initial="initial"
      animate="animate"
      transition={motionVariants.transition}
      className={
        'relative w-[220px] h-[368px] bg-[#000000] rounded-[28px] overflow-hidden ' +
        className
      }
    >
      {/* Top circle: home.js */}
      <div className="absolute top-[48px] left-1/2 -translate-x-1/2 w-24 h-24 bg-[#3A3534] rounded-full border border-[#787676]/30 flex items-center justify-center text-center text-xs font-mono text-[#787676] shadow-[0_0_20px_rgba(120,118,118,0.15)]">
        home.js
      </div>

      {/* Connector line between home.js and 1.js */}
      <div className="absolute top-[112px] left-1/2 -translate-x-1/2 w-[1px] h-[16px] bg-[#787676]/40"></div>

      {/* Middle circle: 1.js */}
      <div className="absolute top-[144px] left-1/2 -translate-x-1/2 w-28 h-28 bg-[#3A3534] rounded-full border border-[#787676]/30 flex items-center justify-center text-center text-xs font-mono text-[#787676] shadow-[0_0_20px_rgba(120,118,118,0.15)]">
        1.js
      </div>

      {/* Small square connector between 1.js and 3.js */}
      <div className="absolute top-[224px] left-1/2 -translate-x-1/2 w-6 h-6 bg-[#3A3534]
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class LockScreen extends StatefulWidget {
  const LockScreen({Key? key}) : super(key: key);

  @override
  State<LockScreen> createState() => _LockScreenState();
}

class _LockScreenState extends State<LockScreen> with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scale;
  late Animation<double> _opacity;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 1400),
    );
    _scale = Tween<double>(begin: 0.95, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOut),
    );
    _opacity = Tween<double>(begin: 0.0, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOut),
    );
    _controller.forward();
  }

  @override
  void dispose() {
    _controller.dispose();
    super.dispose();
  }

  Widget _circle({required double size, required String label, required double top}) {
    return Positioned(
      top: top,
      left: MediaQuery.of(context).size.width / 2 - size / 2,
      child: Container(
        width: size,
        height: size,
        decoration: BoxDecoration(
          color: const Color(0xFF3A3534),
          shape: BoxShape.circle,
          border: Border.all(color: const Color(0xFF787676).withOpacity(0.3)
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
