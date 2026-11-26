---
title: "LockScreen — 0_PuRInJFrc_KIMI_3_5_Design_ (05:30.600)"
description: "LockScreen UI component (recon_0_PuRInJFrc_KIMI_3_5_Design_Tests_for_UI_UX_Logos_s2_02_lockscreen) with SSIM 0.9861, OKLCH design tokens, SLIDE_DOWN motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_0_PuRInJFrc_KIMI_3_-_5_Design_Tests_for_UI_UX_Logos_s2_02_lockscreen"
category: "LockScreen"
ssim: 0.9861
quality_score: 8.72
tags: [lockscreen, ui-design, design-tokens, react, flutter]
---

# LockScreen — 0_PuRInJFrc_KIMI_3_5_Design_ (05:30.600)

> **Category:** [[07_LockScreen|LockScreen]] | **SSIM Fidelity:** `0.9861` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[03_GlassMenu|GlassMenu]], [[09_SplashAuth|SplashAuth]], [[01_Card|Card]]

Professional LockScreen reverse-engineered from 0_PuRInJFrc_KIMI_3_-_5_Design_Tests_for_UI_UX_Logos at 05:30.600. Features SLIDE_DOWN micro-interaction animation with 9.18:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#302522` | `rgb(48, 37, 34)` | `oklch(0.28 0.018 35.7)` | `28.0%` |
| `surface` | `#B98374` | `rgb(185, 131, 116)` | `oklch(0.66 0.071 36.1)` | `3.0%` |
| `accent` | `#080808` | `rgb(8, 8, 8)` | `oklch(0.13 0.000 89.9)` | `5.0%` |
| `text` | `#B3D1D3` | `rgb(179, 209, 211)` | `oklch(0.84 0.032 201.5)` | `8.0%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `SLIDE_DOWN`
- **Measured Duration:** `74.82 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `1.57`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS
// LockScreen component reconstructed from video evidence
// Style: AUTO | Motion: SLIDE_DOWN (IN_VIEW trigger)

import React, { useEffect, useState } from 'react';
import { motion } from 'framer-motion';

interface LockScreenProps {
  className?: string;
  onUnlock?: () => void;
}

const LockScreen: React.FC<LockScreenProps> = ({ className, onUnlock }) => {
  const [isUnlocked, setIsUnlocked] = useState(false);

  useEffect(() => {
    // Animation triggers on mount (IN_VIEW)
    // Duration from design tokens: 74.82s (extremely slow, likely video context)
    // For UI purposes, we use a reasonable duration while preserving easing
  }, []);

  const handleUnlock = () => {
    setIsUnlocked(true);
    onUnlock?.();
  };

  if (isUnlocked) return null;

  return (
    <motion
      div
      initial={{ opacity: 0, y: -15.5 }}
      animate={{ opacity: 1, y: 0 }}
      transition={{ duration: 0.7, ease: [0.16, 1, 0.3, 1] }}
      className={
        'fixed inset-0 z-50 bg-[#302522] text-[#B3D1D3] flex flex-col items-center justify-center ' +
        className
      }
    >
      {/* Screen content area */}
      <div className="relative w-full h-full max-w-md max-h-[478px] rounded-[28px] overflow-hidden shadow-none border border-white/10">
        {/* Decorative top accent bar matching surface color */}
        <div className="absolute top-0 left-0 right-0 h-1 bg-[#B98374]" />

        {/* Main content placeholder */}
        <div className="flex-1 flex flex-col items-center justify-center p-8 text-center">
          <div className="w-20 h-
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class LockScreen extends StatefulWidget {
  final VoidCallback? onUnlock;
  const LockScreen({Key? key, this.onUnlock}) : super(key: key);

  @override
  State<LockScreen> createState() => _LockScreenState();
}

class _LockScreenState extends State<LockScreen>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<Offset> _offsetAnimation;
  late Animation<double> _opacityAnimation;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      duration: const Duration(milliseconds: 700),
      vsync: this,
    );
    _offsetAnimation = Tween<Offset>(
      begin: const Offset(0, -0.155), // -15.5px relative
      end: Offset.zero,
    ).animate(CurvedAnimation(
      parent: _controller,
      curve: Curves.easeInOut, // Approximates cubic-bezier(0.16, 1, 0.3, 1)
    ));
    _opacityAnimation = Tween<double>(begin: 0.0, end: 1.0).animate(_controller);
    _controller.forward();
  }

  @override
  void dispose() {
    _controller.dispose();
    super.dispose();
  }

  @override
  Widget build(BuildContext context) {
    return Material(
      color: Colors.transparent,
      child: Stack(
        children: [
          Container(
            width: double.infinity,
            height: double.infinity,
            color: const Color(0xFF302522),
          ),
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
