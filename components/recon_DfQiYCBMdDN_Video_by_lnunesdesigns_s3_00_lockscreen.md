---
title: "LockScreen — DfQiYCBMdDN_Video_by_lnunesd (00:10.200)"
description: "LockScreen UI component (recon_DfQiYCBMdDN_Video_by_lnunesdesigns_s3_00_lockscreen) with SSIM 0.986, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_DfQiYCBMdDN_Video_by_lnunesdesigns_s3_00_lockscreen"
category: "LockScreen"
ssim: 0.986
quality_score: 8.72
tags: [lockscreen, ui-design, design-tokens, react, flutter]
---

# LockScreen — DfQiYCBMdDN_Video_by_lnunesd (00:10.200)

> **Category:** [[07_LockScreen|LockScreen]] | **SSIM Fidelity:** `0.986` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[03_GlassMenu|GlassMenu]], [[09_SplashAuth|SplashAuth]], [[01_Card|Card]]

Professional LockScreen reverse-engineered from DfQiYCBMdDN_Video_by_lnunesdesigns at 00:10.200. Features FADE_IN_SCALE micro-interaction animation with 8.09:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#564A42` | `rgb(86, 74, 66)` | `oklch(0.42 0.021 55.7)` | `25.2%` |
| `surface` | `#AC8E84` | `rgb(172, 142, 132)` | `oklch(0.67 0.039 39.3)` | `15.0%` |
| `accent` | `#0A060C` | `rgb(10, 6, 12)` | `oklch(0.13 0.016 315.5)` | `5.0%` |
| `text` | `#FAF8F9` | `rgb(250, 248, 249)` | `oklch(0.98 0.002 345.2)` | `2.1%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `7.6 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `9.97`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react'
import { motion } from 'framer-motion'

interface LockScreenProps {
  className?: string
}

const LockScreen: React.FC<LockScreenProps> = ({ className }) => {
  const variants = {
    initial: { opacity: 0, scale: 0.95 },
    animate: { opacity: 1, scale: 1 },
  }

  const transition = {
    type: 'spring',
    stiffness: 260,
    damping: 20,
  }

  return (
    <motion.div
      variants={variants}
      initial="initial"
      animate="animate"
      transition={transition}
      className={
        'relative w-full h-full bg-[#564A42] text-[#FAF8F9] overflow-hidden ' +
        className
      }
    >
      {/* Deep Black Card */}
      <div className="absolute top-1/4 left-1/2 -translate-x-1/2 w-[94px] h-[219px] bg-[#0A060C] rounded-xl shadow-lg border border-white/10">
        <div className="absolute bottom-4 left-4 right-4">
          <h3 className="text-lg font-semibold text-[#FAF8F9] tracking-tight">Deep Black</h3>
          <div className="w-16 h-px bg-[#FAF8F9]/30 mt-1 mb-2"></div>
          <p className="text-xs text-[#FAF8F9]/70 font-mono">#0A060C</p>
        </div>
      </div>

      {/* Bright White Card */}
      <div className="absolute top-2/4 left-1/2 -translate-x-1/2 w-[94px] h-[219px] bg-[#FAF8F9] rounded-xl shadow-lg border border-black/10">
        <div className="absolute bottom-4 left-4 right-4">
          <h3 className="text-lg font-semibold text-[#0A060C] tracking-tight">Bright White</h3>
          <div className="w-16 h-px bg-[#0A060C]/30 mt-1 mb-2"></div>
          <p className="text-xs text-[#0A060C]/70 font-mono">#FA
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

  Widget _buildCard({
    required Color bgColor,
    required Color textColor,
    required String title,
    required String hex,
    required double top,
  }) {
    return Positioned(
      top: top,
      left: 0,
      right: 0,
      child: AnimatedBuilder(
        animation: _controller,
        builder: (context, child) {
          return Opacity(
            opacity: _opacity.value,
            child: Transform.scale(
       
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
