---
title: "LockScreen — DfQiYCBMdDN_Video_by_lnunesd (00:00.000)"
description: "LockScreen UI component (recon_DfQiYCBMdDN_Video_by_lnunesdesigns_s1_00_lockscreen) with SSIM 0.9851, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_DfQiYCBMdDN_Video_by_lnunesdesigns_s1_00_lockscreen"
category: "LockScreen"
ssim: 0.9851
quality_score: 8.72
tags: [lockscreen, ui-design, design-tokens, react, flutter]
---

# LockScreen — DfQiYCBMdDN_Video_by_lnunesd (00:00.000)

> **Category:** [[07_LockScreen|LockScreen]] | **SSIM Fidelity:** `0.9851` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[03_GlassMenu|GlassMenu]], [[09_SplashAuth|SplashAuth]], [[01_Card|Card]]

Professional LockScreen reverse-engineered from DfQiYCBMdDN_Video_by_lnunesdesigns at 00:00.000. Features FADE_IN_SCALE micro-interaction animation with 5.96:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#4C433B` | `rgb(76, 67, 59)` | `oklch(0.39 0.018 63.9)` | `20.8%` |
| `surface` | `#625547` | `rgb(98, 85, 71)` | `oklch(0.46 0.028 69.1)` | `16.1%` |
| `accent` | `#DE9E87` | `rgb(222, 158, 135)` | `oklch(0.76 0.084 40.6)` | `7.8%` |
| `text` | `#E6C5AD` | `rgb(230, 197, 173)` | `oklch(0.85 0.050 58.0)` | `10.2%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `7.6 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `9.97`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS
// LockScreen component reconstructed from video evidence
// Style: AUTO | Motion: FADE_IN_SCALE | Duration: 7600ms

import React from 'react'
import { motion } from 'framer-motion'

interface LockScreenProps {
  className?: string
  onUnlock?: () => void
}

const LockScreen: React.FC<LockScreenProps> = ({ className, onUnlock }) => {
  return (
    <motion.div
      initial={{ opacity: 0, scale: 0.95 }}
      animate={{ opacity: 1, scale: 1 }}
      transition={
        type: 'spring',
        stiffness: 260,
        damping: 20
      }
      className={
        'fixed inset-0 z-50 bg-[#4C433B] flex items-center justify-center ' +
        className
      }
    >
      <motion.div
        initial={{ opacity: 0, y: 20 }}
        animate={{ opacity: 1, y: 0 }}
        transition={{ delay: 0.2, duration: 0.5 }}
        className={
          'w-[101px] h-[159px] rounded-[19px] bg-[#625547] ' +
          'flex flex-col items-center justify-center p-6 ' +
          'shadow-lg relative overflow-hidden'
        }
      >
        {/* Decorative accent ring */}
        <div className="absolute inset-0 border-2 border-[#DE9E87]/30 rounded-[19px] pointer-events-none" />

        {/* Lock icon */}
        <div className="w-12 h-12 bg-[#DE9E87] rounded-full flex items-center justify-center mb-4 shadow-[0_4px_6px_rgba(0,0,0,0.3)]">
          <svg
            className="w-6 h-6 text-[#4C433B]
            fill-current
            "
            viewBox="0 0 24 24"
            aria-hidden="true"
          >
            <path d="M12 17a5 5 0 01-5-5v-5a2 2 0 01
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class LockScreen extends StatefulWidget {
  final VoidCallback? onUnlock;
  const LockScreen({Key? key, this.onUnlock}) : super(key: key);

  @override
  State<LockScreen> createState() => _LockScreenState;
}

class _LockScreenState extends State<LockScreen>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scaleAnim;
  late Animation<double> _opacityAnim;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 7600),
    );
    _scaleAnim = Tween<double>(begin: 0.95, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.elasticOut),
    );
    _opacityAnim = Tween<double>(begin: 0.0, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeIn),
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
      backgroundColor: const Color(0xFF4C433B),
      body: Center(
        child: AnimatedBuilder(
          animation: _controller,
          builder: (context, child) {
            return Opacity(
              opacity: _opacityAnim.value,
              child: Transform.scale(
                scale:
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
