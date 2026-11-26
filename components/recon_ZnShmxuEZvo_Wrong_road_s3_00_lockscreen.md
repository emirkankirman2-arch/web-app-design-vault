---
title: "LockScreen — ZnShmxuEZvo_Wrong_road (01:30.617)"
description: "LockScreen UI component (recon_ZnShmxuEZvo_Wrong_road_s3_00_lockscreen) with SSIM 0.9904, OKLCH design tokens, SLIDE_DOWN motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_ZnShmxuEZvo_Wrong_road_s3_00_lockscreen"
category: "LockScreen"
ssim: 0.9904
quality_score: 8.72
tags: [lockscreen, ui-design, design-tokens, react, flutter]
---

# LockScreen — ZnShmxuEZvo_Wrong_road (01:30.617)

> **Category:** [[07_LockScreen|LockScreen]] | **SSIM Fidelity:** `0.9904` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[03_GlassMenu|GlassMenu]], [[09_SplashAuth|SplashAuth]], [[01_Card|Card]]

Professional LockScreen reverse-engineered from ZnShmxuEZvo_Wrong_road at 01:30.617. Features SLIDE_DOWN micro-interaction animation with 5.45:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#000000` | `rgb(0, 0, 0)` | `oklch(0.00 0.000 0.0)` | `38.9%` |
| `surface` | `#848183` | `rgb(132, 129, 131)` | `oklch(0.61 0.005 337.4)` | `16.3%` |
| `accent` | `#160D19` | `rgb(22, 13, 25)` | `oklch(0.18 0.028 317.5)` | `3.5%` |
| `text` | `#848183` | `rgb(132, 129, 131)` | `oklch(0.61 0.005 337.4)` | `16.3%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `SLIDE_DOWN`
- **Measured Duration:** `10.425 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `10.11`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS
// LockScreen component reconstructed from video evidence
// Source: ZnShmxuEZvo_Wrong_road.mp4, TABLET_LANDSCAPE view at 01:30.617

import React, { useEffect, useState } from 'react'
import { motion } from 'framer-motion'

interface LockScreenProps {
  className?: string
  onUnlock?: () => void
}

const LockScreen: React.FC<LockScreenProps> = ({ className, onUnlock }) => {
  const [isUnlocked, setIsUnlocked] = useState(false)

  useEffect(() => {
    // Auto slide down animation triggered on mount
    // Duration: 10.43s, easing: cubic-bezier(0.16, 1, 0.3, 1)
  }, [])

  const handleUnlock = () => {
    setIsUnlocked(true)
    onUnlock?.()
  }

  return (
    <div
      className={
        'relative w-full h-full bg-black overflow-hidden ' + className
      }
    >
      {/* Background layer - black base */}
      <div className="absolute inset-0 bg-black" />

      {/* Surface layer - gray card/panel */}
      <motion.div
        initial={{ opacity: 0, y: -5.6 }}
        animate={{ opacity: 1, y: 0 }}
        transition={
          duration: 10.43,
          ease: [0.16, 1, 0.3, 1]
        }
        className={
          'absolute inset-0 bg-[#848183] rounded-[21px] ' +
          'flex flex-col items-center justify-center ' +
          'transition-all duration-300 ease-in-out'
        }
      >
        {/* Lock icon placeholder */}
        <div className="w-16 h-16 bg-[#160D19] rounded-full flex items-center justify-center mb-8 opacity-50">
          <svg
            className="w-8 h-8 text-white"
            fill="none"
            stro
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';
import 'dart:async';

class LockScreen extends StatefulWidget {
  final VoidCallback? onUnlock;
  const LockScreen({Key? key, this.onUnlock}) : super(key: key);

  @override
  State<LockScreen> createState() => _LockScreenState;
}

class _LockScreenState extends State<LockScreen>
    with SingleTickerProviderStateMixin {
  bool _isUnlocked = false;
  late AnimationController _controller;
  late Animation<Offset> _offsetAnimation;
  late Animation<double> _opacityAnimation;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      duration: const Duration(milliseconds: 10425),
      vsync: this,
    );
    _offsetAnimation = Tween<Offset>(
      begin: const Offset(0, -0.025), // approx -5.6px relative
      end: Offset.zero,
    ).animate(CurvedAnimation(
      parent: _controller,
      curve: Curves.easeInOut, // cubic-bezier(0.16, 1, 0.3, 1)
    ));
    _opacityAnimation = Tween<double>(begin: 0.0, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeInOut),
    );
    _controller.forward();
  }

  @override
  void dispose() {
    _controller.dispose();
    super.dispose();
  }

  void _handleUnlock() {
    setState(() => _isUnlocked = true);
    widget.onUnlock?.call();
  }

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundCol
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
