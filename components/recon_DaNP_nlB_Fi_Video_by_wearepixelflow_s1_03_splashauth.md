---
title: "SplashAuth — DaNP_nlB_Fi_Video_by_wearepi (00:08.400)"
description: "SplashAuth UI component (recon_DaNP_nlB_Fi_Video_by_wearepixelflow_s1_03_splashauth) with SSIM 0.9703, OKLCH design tokens, FADE_AND_SLIDE_UP motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_DaNP_nlB_Fi_Video_by_wearepixelflow_s1_03_splashauth"
category: "SplashAuth"
ssim: 0.9703
quality_score: 8.72
tags: [splashauth, ui-design, design-tokens, react, flutter]
---

# SplashAuth — DaNP_nlB_Fi_Video_by_wearepi (00:08.400)

> **Category:** [[09_SplashAuth|SplashAuth]] | **SSIM Fidelity:** `0.9703` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[06_Input|Input]], [[07_LockScreen|LockScreen]], [[05_Hero|Hero]]

Professional SplashAuth reverse-engineered from DaNP_nlB_Fi_Video_by_wearepixelflow at 00:08.400. Features FADE_AND_SLIDE_UP micro-interaction animation with 12.89:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#F0EDE6` | `rgb(240, 237, 230)` | `oklch(0.95 0.010 87.5)` | `48.4%` |
| `surface` | `#E9E3DB` | `rgb(233, 227, 219)` | `oklch(0.92 0.013 75.4)` | `18.8%` |
| `accent` | `#D6CAB8` | `rgb(214, 202, 184)` | `oklch(0.84 0.028 78.2)` | `5.0%` |
| `text` | `#282624` | `rgb(40, 38, 36)` | `oklch(0.27 0.005 67.6)` | `3.4%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_AND_SLIDE_UP`
- **Measured Duration:** `0.45 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `120.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
// SplashAuth component reconstructed from video evidence (MOBILE_PORTRAIT @ 00:08.400)
import React from 'react';
import { motion } from 'framer-motion';

export interface SplashAuthProps {
  className?: string;
  onComplete?: () => void;
}

export const SplashAuth: React.FC<SplashAuthProps> = ({ className, onComplete }) => {
  return (
    <motion.div
      initial={{ opacity: 0, y: 24 }}
      animate={{ opacity: 1, y: 0 }}
      transition={{ duration: 0.45, ease: [0.16, 1, 0.3, 1] }}
      className={
        'relative w-full max-w-[356px] h-[284px] bg-[#F0EDE6] rounded-[28px] overflow-hidden shadow-none ' +
        (className || '')
      }
      role="region"
      aria-label="Splash authentication screen"
    >
      {/* Decorative torn paper top strip */}
      <div className="absolute top-0 left-0 w-full h-12 bg-[#F0EDE6] border-b border-[#D6CAB8]" />

      {/* Main content area */}
      <div className="absolute inset-0 flex flex-col items-center justify-center p-8 text-center">
        {/* Speech bubble icon */}
        <div className="relative mb-6 w-16 h-16 bg-[#282624] rounded-full flex items-center justify-center">
          <div className="absolute -bottom-2 left-1/2 -translate-x-1/2 w-8 h-4 bg-[#282624] rounded-b-full" />
          <div className="flex gap-1.5">
            {[0, 1, 2].map((i) => (
              <div key={i} className="w-2.5 h-2.5 bg-[#F0EDE6] rounded-full" />
            ))}
          </div>
        </div>

        {/* Title */}
        <h1 className="text-3xl font-bold text-[#282624] tra
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';
import 'dart:async';

class SplashAuth extends StatefulWidget {
  final VoidCallback? onComplete;
  const SplashAuth({Key? key, this.onComplete}) : super(key: key);

  @override
  State<SplashAuth> createState() => _SplashAuthState();
}

class _SplashAuthState extends State<SplashAuth>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<Offset> _offsetAnimation;
  late Animation<double> _opacityAnimation;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      duration: const Duration(milliseconds: 450),
      vsync: this,
    );
    _offsetAnimation = Tween<Offset>(
      begin: const Offset(0, 0.15), // approx 24px on typical scale
      end: Offset.zero,
    ).animate(CurvedAnimation(
      parent: _controller,
      curve: Curves.easeInOutCubic, // closest to cubic-bezier(0.16,1,0.3,1)
    ));
    _opacityAnimation = Tween<double>(begin: 0.0, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeIn),
    );
    _controller.forward();

    // Auto trigger completion after animation
    Timer(const Duration(milliseconds: 450), () {
      widget.onComplete?.call();
    });
  }

  @override
  void dispose() {
    _controller.dispose();
    super.dispose();
  }

  @override
  Widget build(BuildContext context) {
    return
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
