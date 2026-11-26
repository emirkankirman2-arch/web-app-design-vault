---
title: "LockScreen — DfQiYCBMdDN_Video_by_lnunesd (00:06.200)"
description: "LockScreen UI component (recon_DfQiYCBMdDN_Video_by_lnunesdesigns_s2_00_lockscreen) with SSIM 0.9864, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_DfQiYCBMdDN_Video_by_lnunesdesigns_s2_00_lockscreen"
category: "LockScreen"
ssim: 0.9864
quality_score: 8.72
tags: [lockscreen, ui-design, design-tokens, react, flutter]
---

# LockScreen — DfQiYCBMdDN_Video_by_lnunesd (00:06.200)

> **Category:** [[07_LockScreen|LockScreen]] | **SSIM Fidelity:** `0.9864` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[03_GlassMenu|GlassMenu]], [[09_SplashAuth|SplashAuth]], [[01_Card|Card]]

Professional LockScreen reverse-engineered from DfQiYCBMdDN_Video_by_lnunesdesigns at 00:06.200. Features FADE_IN_SCALE micro-interaction animation with 8.01:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#53483F` | `rgb(83, 72, 63)` | `oklch(0.41 0.021 61.5)` | `28.1%` |
| `surface` | `#A58B80` | `rgb(165, 139, 128)` | `oklch(0.66 0.036 44.2)` | `13.9%` |
| `accent` | `#C5F236` | `rgb(197, 242, 54)` | `oklch(0.90 0.205 122.9)` | `4.9%` |
| `text` | `#F3F4EB` | `rgb(243, 244, 235)` | `oklch(0.96 0.012 111.8)` | `4.9%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `7.6 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `9.97`

## 3. React + TypeScript + Tailwind Implementation

```tsx
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
    duration: 7.6,
  };

  return (
    <motion.div
      variants={variants}
      initial="initial"
      animate="animate"
      transition={transition}
      className={
        'relative w-full h-full bg-[#53483F] text-[#F3F4EB] overflow-hidden ' +
        className
      }
    >
      {/* Background surface card */}
      <div className="absolute inset-0 bg-[#A58B80]/10 blur-[40px] rounded-full" />

      {/* Content area */}
      <div className="absolute inset-0 flex flex-col items-center justify-center p-6 z-10">
        <div className="w-full max-w-md space-y-8">
          {/* Time */}
          <div className="text-6xl font-light tracking-tight">
            12:00
          </div>

          {/* Date */}
          <div className="text-xl font-medium tracking-widest uppercase">
            MONDAY, JANUARY 1
          </div>

          {/* Notifications preview */}
          <div className="space-y-3">
            <div className="flex items-center gap-3 px-4 py-2 rounded-lg bg-white/10">
              <div className="w-8 h-8 rounded-full bg-[#C5F236] flex items-center justify-center text-[#53483F] font-bold text-xs">
                J
              </div>
              <div className="flex
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
      duration: const Duration(milliseconds: 7600),
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
      backgroundColor: const Color(0xFF53483F),
      body: Stack(
        children: [
          // Background surface blur
          Positioned.fill(
            child: Container(
              decoration: BoxDecoration(
                color: const Color(0xFFA58B80).withOpacity(0.1),
                shape: BoxShape.circle,
              ),
            ),
       
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
