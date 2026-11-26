---
title: "LockScreen — lnXzJmFw0lQ_I_brought_androi (02:44.500)"
description: "LockScreen UI component (recon_lnXzJmFw0lQ_I_brought_android_style_app_bubbles_to_the_web_s3_00_l) with SSIM 0.9992, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_lnXzJmFw0lQ_I_brought_android_style_app_bubbles_to_the_web_s3_00_lockscreen"
category: "LockScreen"
ssim: 0.9992
quality_score: 8.72
tags: [lockscreen, ui-design, design-tokens, react, flutter]
---

# LockScreen — lnXzJmFw0lQ_I_brought_androi (02:44.500)

> **Category:** [[07_LockScreen|LockScreen]] | **SSIM Fidelity:** `0.9992` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[03_GlassMenu|GlassMenu]], [[09_SplashAuth|SplashAuth]], [[01_Card|Card]]

Professional LockScreen reverse-engineered from lnXzJmFw0lQ_I_brought_android_style_app_bubbles_to_the_web at 02:44.500. Features FADE_IN_SCALE micro-interaction animation with 12.94:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#000000` | `rgb(0, 0, 0)` | `oklch(0.00 0.000 0.0)` | `82.3%` |
| `surface` | `#454647` | `rgb(69, 70, 71)` | `oklch(0.39 0.002 247.9)` | `1.5%` |
| `accent` | `#138ABB` | `rgb(19, 138, 187)` | `oklch(0.60 0.120 233.4)` | `0.3%` |
| `text` | `#CBCBCB` | `rgb(203, 203, 203)` | `oklch(0.84 0.000 89.9)` | `2.4%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `24.5 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.04`

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
  };

  return (
    <motion.div
      className={
        'fixed inset-0 z-50 bg-black flex items-center justify-center ' + (className || '')
      }
      initial='initial'
      animate='animate'
      transition={transition}
      role='dialog'
      aria-modal='true'
      aria-label='Lock screen'
    >
      <div className='w-[74px] h-[306px] bg-[#454647] rounded-none shadow-none relative overflow-hidden'>
        {/* Vertical accent line matching screenshot */}
        <div className='absolute left-1/2 top-0 bottom-0 w-[2px] bg-white transform -translate-x-1/2' />
      </div>
    </motion.div>
  );
};

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
      duration: const Duration(milliseconds: 24500),
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
    return Scaffold(
      backgroundColor: Colors.black,
      body: Center(
        child: FadeTransition(
          opacity: _opacity,
          child: ScaleTransition(
            scale: _scale,
            child: Container(
              width: 74,
              height: 306,
              color: const Color(0xFF454647),
              child: const VerticalLine(),
            ),
 
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
