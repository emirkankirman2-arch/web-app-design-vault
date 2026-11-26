---
title: "LockScreen — Dfcao2WMM6K_Video_by_vedant_ (00:08.567)"
description: "LockScreen UI component (recon_Dfcao2WMM6K_Video_by_vedant_design_tech_s2_00_lockscreen) with SSIM 0.9874, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_Dfcao2WMM6K_Video_by_vedant.design.tech_s2_00_lockscreen"
category: "LockScreen"
ssim: 0.9874
quality_score: 8.72
tags: [lockscreen, ui-design, design-tokens, react, flutter]
---

# LockScreen — Dfcao2WMM6K_Video_by_vedant_ (00:08.567)

> **Category:** [[07_LockScreen|LockScreen]] | **SSIM Fidelity:** `0.9874` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[03_GlassMenu|GlassMenu]], [[09_SplashAuth|SplashAuth]], [[01_Card|Card]]

Professional LockScreen reverse-engineered from Dfcao2WMM6K_Video_by_vedant.design.tech at 00:08.567. Features FADE_IN_SCALE micro-interaction animation with 10.33:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#D4BCA7` | `rgb(212, 188, 167)` | `oklch(0.81 0.040 63.4)` | `23.9%` |
| `surface` | `#B29C8A` | `rgb(178, 156, 138)` | `oklch(0.71 0.037 61.5)` | `21.1%` |
| `accent` | `#AC6750` | `rgb(172, 103, 80)` | `oklch(0.58 0.096 39.2)` | `13.4%` |
| `text` | `#160E20` | `rgb(22, 14, 32)` | `oklch(0.18 0.037 303.4)` | `7.8%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `6.567 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `1.21`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react'
import { motion } from 'framer-motion'

interface LockScreenProps {
  className?: string
}

const LockScreen: React.FC<LockScreenProps> = ({ className }) => {
  return (
    <motion.div
      initial={{ opacity: 0, scale: 0.95 }}
      animate={{ opacity: 1, scale: 1 }}
      transition={{ type: 'spring', stiffness: 260, damping: 20 }}
      className={
        'relative w-full h-full bg-[#D4BCA7] text-[#160E20] overflow-hidden ' +
        className
      }
    >
      {/* Top status bar area */}
      <div className="absolute top-0 left-0 right-0 h-16 flex items-center justify-between px-6 z-10">
        <div className="flex items-center gap-3">
          <div className="w-3 h-3 rounded-full bg-[#AC6750]" />
          <div className="w-3 h-3 rounded-full bg-[#AC6750]" />
          <div className="w-3 h-3 rounded-full bg-[#AC6750]" />
        </div>
        <div className="text-lg font-medium">10:00</div>
        <div className="flex items-center gap-2">
          <div className="w-2 h-2 rounded-full bg-[#AC6750]" />
          <div className="w-2 h-2 rounded-full bg-[#AC6750]" />
          <div className="w-2 h-2 rounded-full bg-[#AC6750]" />
        </div>
      </div>

      {/* Center content - time and date */}
      <div className="absolute inset-0 flex flex-col items-center justify-center z-20">
        <div className="text-9xl font-light tracking-tight">10:00</div>
        <div className="mt-2 text-2xl font-medium tracking-widest">
          MON, JAN 1
        </div>
      </div>

      {/* Bottom unlock hint */}
      <div className="absolu
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
  late Animation<double> _opacity;
  late Animation<double> _scale;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 6566),
    );
    _opacity = Tween<double>(begin: 0.0, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOut),
    );
    _scale = Tween<double>(begin: 0.95, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOut),
    );
    _controller.forward();
  }

  @override
  void dispose() {
    _controller.dispose();
    super.dispose();
  }

  @override
  Widget build(BuildContext context) {
    return AnimatedBuilder(
      animation: _controller,
      builder: (context, child) {
        return Opacity(
          opacity: _opacity.value,
          child: Transform.scale(
            scale: _scale.value,
            child: Scaffold(
              backgroundColor: const Color(0xFFD4BCA7),
              body: Stack(
                children: [
                  // Status b
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
