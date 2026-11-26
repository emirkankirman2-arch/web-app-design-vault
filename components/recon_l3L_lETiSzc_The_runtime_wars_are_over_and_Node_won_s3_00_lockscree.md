---
title: "LockScreen — l3L_lETiSzc_The_runtime_wars (04:07.747)"
description: "LockScreen UI component (recon_l3L_lETiSzc_The_runtime_wars_are_over_and_Node_won_s3_00_lockscree) with SSIM 0.9925, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_l3L_lETiSzc_The_runtime_wars_are_over..._and_Node_won_s3_00_lockscreen"
category: "LockScreen"
ssim: 0.9925
quality_score: 8.72
tags: [lockscreen, ui-design, design-tokens, react, flutter]
---

# LockScreen — l3L_lETiSzc_The_runtime_wars (04:07.747)

> **Category:** [[07_LockScreen|LockScreen]] | **SSIM Fidelity:** `0.9925` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[03_GlassMenu|GlassMenu]], [[09_SplashAuth|SplashAuth]], [[01_Card|Card]]

Professional LockScreen reverse-engineered from l3L_lETiSzc_The_runtime_wars_are_over..._and_Node_won at 04:07.747. Features FADE_IN_SCALE micro-interaction animation with 9.93:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#0E0C0D` | `rgb(14, 12, 13)` | `oklch(0.16 0.004 345.8)` | `93.2%` |
| `surface` | `#493662` | `rgb(73, 54, 98)` | `oklch(0.37 0.076 302.8)` | `0.2%` |
| `accent` | `#20BEDA` | `rgb(32, 190, 218)` | `oklch(0.74 0.125 213.9)` | `0.6%` |
| `text` | `#58CF88` | `rgb(88, 207, 136)` | `oklch(0.77 0.149 154.5)` | `0.2%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `32.532 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `2.25`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react';
import { motion } from 'framer-motion';

interface LockScreenProps {
  className?: string;
}

export const LockScreen: React.FC<LockScreenProps> = ({ className }) => {
  const containerVariants = {
    hidden: { opacity: 0, scale: 0.95 },
    visible: {
      opacity: 1,
      scale: 1,
      transition: {
        type: 'spring',
        stiffness: 260,
        damping: 20,
        duration: 0.32532,
      },
    },
  };

  return (
    <motion.div
      variants={containerVariants}
      initial="hidden"
      animate="visible"
      className={
        'relative w-[324px] h-[569px] bg-[#0E0C0D] rounded-[28px] overflow-hidden flex flex-col items-center justify-center ' +
        className
      }
    >
      {/* Antennae dashed lines */}
      <div className="absolute top-[120px] left-[110px] w-[2px] h-[80px] bg-[#20BEDA] opacity-60" />
      <div className="absolute top-[120px] left-[112px] w-[2px] h-[80px] bg-[#20BEDA] opacity-60" />
      <div className="absolute top-[120px] left-[210px] w-[2px] h-[80px] bg-[#20BEDA] opacity-60" />
      <div className="absolute top-[120px] left-[212px] w-[2px] h-[80px] bg-[#20BEDA] opacity-60" />

      {/* Antennae circles */}
      <div className="absolute top-[40px] left-[90px] w-[40px] h-[40px] bg-[#20BEDA] rounded-full shadow-[0_0_15px_rgba(32,190,218,0.6)]" />
      <div className="absolute top-[40px] left-[194px] w-[40px] h-[40px] bg-[#20BEDA] rounded-full shadow-[0_0_15px_rgba(32,190,218,0.6)]" />

      {/* Main green panel */}
      <div className="relative z-10 w-[260px] h-[200px] bg-[#00D97A] roun
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
  late Animation<double> _scaleAnimation;
  late Animation<double> _opacityAnimation;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 325),
    );
    _scaleAnimation = Tween<double>(begin: 0.95, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOut),
    );
    _opacityAnimation = Tween<double>(begin: 0.0, end: 1.0).animate(
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
          opacity: _opacityAnimation.value,
          child: Transform.scale(
            scale: _scaleAnimation.value,
            child: Container(
              width: 324,
              height: 569,
              decoration: BoxDeco
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
