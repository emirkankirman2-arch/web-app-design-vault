---
title: "SplashAuth — DcGq_G_sfwF_Video_by_figma_c (00:00.000)"
description: "SplashAuth UI component (recon_DcGq_G_sfwF_Video_by_figma_create_s1_01_splashauth) with SSIM 0.9768, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_DcGq-G-sfwF_Video_by_figma.create_s1_01_splashauth"
category: "SplashAuth"
ssim: 0.9768
quality_score: 8.72
tags: [splashauth, ui-design, design-tokens, react, flutter]
---

# SplashAuth — DcGq_G_sfwF_Video_by_figma_c (00:00.000)

> **Category:** [[09_SplashAuth|SplashAuth]] | **SSIM Fidelity:** `0.9768` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[06_Input|Input]], [[07_LockScreen|LockScreen]], [[05_Hero|Hero]]

Professional SplashAuth reverse-engineered from DcGq-G-sfwF_Video_by_figma.create at 00:00.000. Features FADE_IN_SCALE micro-interaction animation with 15.7:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#BCEDE4` | `rgb(188, 237, 228)` | `oklch(0.91 0.052 182.7)` | `31.0%` |
| `surface` | `#90B8B3` | `rgb(144, 184, 179)` | `oklch(0.75 0.043 186.9)` | `3.9%` |
| `accent` | `#55F6BC` | `rgb(85, 246, 188)` | `oklch(0.87 0.157 165.1)` | `7.5%` |
| `text` | `#06070A` | `rgb(6, 7, 10)` | `oklch(0.13 0.008 268.5)` | `5.5%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `9.4 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.02`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react'
import { motion } from 'framer-motion'

interface SplashAuthProps {
  className?: string
  onComplete?: () => void
}

const SplashAuth: React.FC<SplashAuthProps> = ({ className, onComplete }) => {
  return (
    <motion.div
      initial={{ opacity: 0, scale: 0.95 }}
      animate={{ opacity: 1, scale: 1 }}
      transition={
        type: 'spring',
        stiffness: 260,
        damping: 20,
        duration: 9.4
      }
      className={
        'fixed inset-0 z-50 flex items-center justify-center bg-[#BCEDE4] ' +
        className
      }
      onAnimationComplete={onComplete}
    >
      <div className="relative w-[355px] h-[262px] rounded-lg overflow-hidden shadow-lg">
        {/* Decorative top light streaks */}
        <div className="absolute top-0 left-0 w-full h-12 overflow-hidden pointer-events-none">
          <div className="absolute top-0 left-0 w-full h-full bg-white opacity-30 transform skew-x-[-15deg] animate-[stripe_3s_linear_infinite]"></div>
        </div>

        {/* Main content area */}
        <div className="absolute inset-0 flex flex-col items-center justify-center p-6 text-center">
          <div className="relative w-32 h-32 mb-6">
            {/* Abstract splash shape */}
            <div className="absolute inset-0 bg-[#90B8B3] rounded-full opacity-60 blur-xl animate-pulse"></div>
            <div className="absolute inset-4 bg-[#55F6BC] rounded-full opacity-40 blur-lg animate-[spin_10s_linear_infinite]"></div>
            <div className="absolute inset-8 bg-white rounded-full opacity-20 blur-md"></div>
          </d
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class SplashAuth extends StatefulWidget {
  const SplashAuth({Key? key}) : super(key: key);

  @override
  State<SplashAuth> createState() => _SplashAuthState();
}

class _SplashAuthState extends State<SplashAuth>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scale;
  late Animation<double> _opacity;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 9400),
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

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: const Color(0xFFBCEDE4),
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
     
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
