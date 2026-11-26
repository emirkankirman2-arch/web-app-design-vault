---
title: "Hero — k_5BGYydqz4_Linear_app_card_ (00:44.767)"
description: "Hero UI component (recon_k_5BGYydqz4_Linear_app_card_animation_with_CSS_Blending_s3_00_hero) with SSIM 0.9927, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_k-5BGYydqz4_Linear.app_card_animation_with_CSS_Blending_s3_00_hero"
category: "Hero"
ssim: 0.9927
quality_score: 8.72
tags: [hero, ui-design, design-tokens, react, flutter]
---

# Hero — k_5BGYydqz4_Linear_app_card_ (00:44.767)

> **Category:** [[05_Hero|Hero]] | **SSIM Fidelity:** `0.9927` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[10_ShaderCanvas|ShaderCanvas]], [[02_Button|Button]], [[04_Navbar|Navbar]]

Professional Hero reverse-engineered from k-5BGYydqz4_Linear.app_card_animation_with_CSS_Blending at 00:44.767. Features FADE_IN_SCALE micro-interaction animation with 19.43:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#FDFDFD` | `rgb(253, 253, 253)` | `oklch(0.99 0.000 89.9)` | `56.7%` |
| `surface` | `#141518` | `rgb(20, 21, 24)` | `oklch(0.20 0.006 271.1)` | `17.8%` |
| `accent` | `#03042F` | `rgb(3, 4, 47)` | `oklch(0.15 0.085 269.4)` | `12.2%` |
| `text` | `#03042F` | `rgb(3, 4, 47)` | `oklch(0.15 0.085 269.4)` | `12.2%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `6.267 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.41`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
// Reconstructed from video evidence: Linear.app card animation with CSS Blending
// Source: k-5BGYydqz4_Linear.app_card_animation_with_CSS_Blending.mp4 @ 00:44.767

import React from 'react'
import { motion } from 'framer-motion'

interface HeroCardAnimationProps {
  className?: string
}

export const HeroCardAnimation: React.FC<HeroCardAnimationProps> = ({ className }) => {
  return (
    <section className={\`relative flex flex-col items-center justify-center min-h-screen bg-[#FDFDFD] p-8 text-center \${className}\`}>
      {/* Heading */}
      <motion.h1
        initial={{ opacity: 0, y: 20 }}
        animate={{ opacity: 1, y: 0 }}
        transition={{ duration: 0.6, ease: 'easeOut' }}
        className="text-5xl font-bold text-[#03042F] tracking-tight mb-12"
      >
        Lets mix-blend it again!
      </motion.h1>

      {/* Card Container */}
      <motion.div
        initial={{ opacity: 0, scale: 0.95 }}
        animate={{ opacity: 1, scale: 1 }}
        transition={
          type: 'spring',
          stiffness: 260,
          damping: 20,
          duration: 6.266
        }
        className="relative w-[720px] h-[720px] rounded-[12px] overflow-hidden shadow-2xl bg-[#141518]"
      >
        {/* Background gradient with blend mode simulation */}
        <div
          className="absolute inset-0 bg-gradient-to-br from-[#03042F] via-[#141518] to-[#03042F]"
        />
        {/* Blend overlay - simulating color-dodge effect */}
        <div
          className="absolute inset-0 bg-gradient-to-tr from-blue-900/4
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class HeroCardAnimation extends StatefulWidget {
  const HeroCardAnimation({super.key});

  @override
  State<HeroCardAnimation> createState() => _HeroCardAnimationState();
}

class _HeroCardAnimationState extends State<HeroCardAnimation>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scaleAnim;
  late Animation<double> _opacityAnim;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 6266),
    );
    _scaleAnim = Tween<double>(begin: 0.95, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOutBack),
    );
    _opacityAnim = Tween<double>(begin: 0.0, end: 1.0).animate(
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
      backgroundColor: const Color(0xFFFDFCFD),
      body: Center(
        child: Column(
          mainAxisAlignment: MainAxisAlignment.center,
          children: [
            const Text(
              "Lets mix-blend it again!",
              style: TextStyle(
                fontSize: 40,
                fontWeigh
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
