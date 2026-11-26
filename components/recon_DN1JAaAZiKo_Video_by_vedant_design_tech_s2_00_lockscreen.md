---
title: "LockScreen — DN1JAaAZiKo_Video_by_vedant_ (00:12.667)"
description: "LockScreen UI component (recon_DN1JAaAZiKo_Video_by_vedant_design_tech_s2_00_lockscreen) with SSIM 0.9921, OKLCH design tokens, SLIDE_UP motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_DN1JAaAZiKo_Video_by_vedant.design.tech_s2_00_lockscreen"
category: "LockScreen"
ssim: 0.9921
quality_score: 8.72
tags: [lockscreen, ui-design, design-tokens, react, flutter]
---

# LockScreen — DN1JAaAZiKo_Video_by_vedant_ (00:12.667)

> **Category:** [[07_LockScreen|LockScreen]] | **SSIM Fidelity:** `0.9921` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[03_GlassMenu|GlassMenu]], [[09_SplashAuth|SplashAuth]], [[01_Card|Card]]

Professional LockScreen reverse-engineered from DN1JAaAZiKo_Video_by_vedant.design.tech at 00:12.667. Features SLIDE_UP micro-interaction animation with 15.86:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#F7EFF0` | `rgb(247, 239, 240)` | `oklch(0.96 0.009 8.5)` | `50.8%` |
| `surface` | `#E4DCD4` | `rgb(228, 220, 212)` | `oklch(0.90 0.014 67.6)` | `15.5%` |
| `accent` | `#DAA4E6` | `rgb(218, 164, 230)` | `oklch(0.79 0.108 320.1)` | `15.0%` |
| `text` | `#141814` | `rgb(20, 24, 20)` | `oklch(0.20 0.010 145.2)` | `0.8%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `SLIDE_UP`
- **Measured Duration:** `5.0 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `20.83`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS
// Reconstructed LockScreen component based on video evidence
// Style: AUTO | Motion: SLIDE_UP | Duration: 5000ms

import React, { useEffect } from 'react';
import { motion } from 'framer-motion';

interface LockScreenProps {
  className?: string;
}

export const LockScreen: React.FC<LockScreenProps> = ({ className }) => {
  useEffect(() => {
    // Animation is handled by Framer Motion initial/animate props
    // Trigger: IN_VIEW - could be enhanced with IntersectionObserver
  }, []);

  return (
    <motion.div
      className={
        'relative w-full h-full rounded-3xl bg-[#F7EFF0] overflow-hidden ' +
        className
      }
      initial={{ opacity: 0, y: 5.032135963439941 }}
      animate={{ opacity: 1, y: 0 }}
      transition={
        {
          duration: 5.0,
          ease: [0.16, 1, 0.3, 1],
        }
      }
    >
      {/* Background accent shape - top right purple blob */}
      <div
        className="absolute top-[-10%] right-[-10%] w-[200px] h-[200px] bg-[#DAA4E6] rounded-full blur-3xl opacity-80"
      />

      {/* Background accent shape - bottom left dark green blob */}
      <div
        className="absolute bottom-[-15%] left-[-15%] w-[250px] h-[250px] bg-[#2D4A3E] rounded-full blur-3xl opacity-90"
      />

      {/* Main content area */}
      <div className="relative z-10 h-full flex flex-col items-center justify-center p-6 text-center">
        {/* Decorative cell shapes */}
        <div className="relative w-full h-[60%] flex items-center justify-center mb-8">
          {/* Purple cell shape */}
          
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
  late Animation<double> _opacityAnimation;
  late Animation<Offset> _slideAnimation;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      duration: const Duration(milliseconds: 5000),
      vsync: this,
    );
    _opacityAnimation = Tween<double>(begin: 0.0, end: 1.0).animate(
      CurvedAnimation(
        parent: _controller,
        curve: Curves.easeInOut,
      ),
    );
    _slideAnimation = Tween<Offset>(begin: const Offset(0, 0.1), end: Offset.zero).animate(
      CurvedAnimation(
        parent: _controller,
        curve: const Cubic(0.16, 1, 0.3, 1),
      ),
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
        return FadeTransition(
          opacity: _opacityAnimation,
          child: SlideTransition(
            position: _slideAnimation,
            child: Containe
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
