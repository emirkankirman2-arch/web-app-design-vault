---
title: "LockScreen — taSmwcqdkQk_What_is_a_Data_L (00:11.440)"
description: "LockScreen UI component (recon_taSmwcqdkQk_What_is_a_Data_Lakehouse_s1_02_lockscreen) with SSIM 0.9938, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_taSmwcqdkQk_What_is_a_Data_Lakehouse_s1_02_lockscreen"
category: "LockScreen"
ssim: 0.9938
quality_score: 8.72
tags: [lockscreen, ui-design, design-tokens, react, flutter]
---

# LockScreen — taSmwcqdkQk_What_is_a_Data_L (00:11.440)

> **Category:** [[07_LockScreen|LockScreen]] | **SSIM Fidelity:** `0.9938` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[03_GlassMenu|GlassMenu]], [[09_SplashAuth|SplashAuth]], [[01_Card|Card]]

Professional LockScreen reverse-engineered from taSmwcqdkQk_What_is_a_Data_Lakehouse at 00:11.440. Features FADE_IN_SCALE micro-interaction animation with 7.96:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#252525` | `rgb(37, 37, 37)` | `oklch(0.26 0.000 89.9)` | `94.9%` |
| `surface` | `#3B403C` | `rgb(59, 64, 60)` | `oklch(0.37 0.010 151.6)` | `1.7%` |
| `accent` | `#6BC7E3` | `rgb(107, 199, 227)` | `oklch(0.78 0.096 220.0)` | `0.3%` |
| `text` | `#6BC7E3` | `rgb(107, 199, 227)` | `oklch(0.78 0.096 220.0)` | `0.3%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `80.08 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react'
import { motion } from 'framer-motion'

interface LockScreenProps {
  className?: string
}

export const LockScreen: React.FC<LockScreenProps> = ({ className }) => {
  return (
    <motion.div
      className={
        'fixed inset-0 z-50 bg-[#252525] flex items-center justify-center ' +
        className
      }
      initial={{ opacity: 0, scale: 0.95 }}
      animate={{ opacity: 1, scale: 1 }}
      transition={{ type: 'spring', stiffness: 260, damping: 20 }}
      aria-label="Lock screen"
      role="dialog"
      aria-modal="true"
    >
      <div className="w-[70px] h-[351px] bg-[#3B403C] relative overflow-hidden">
        {/* Vertical accent line matching screenshot crop */}
        <div className="absolute left-1/2 top-0 bottom-0 w-[1px] bg-[#6BC7E3] transform -translate-x-1/2" />
      </div>
    </motion.div>
  )
}

// Usage example:
// <LockScreen />
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
      duration: const Duration(milliseconds: 800),
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
              backgroundColor: const Color(0xFF252525),
              body: Center(
                child: Container(
                  width
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
