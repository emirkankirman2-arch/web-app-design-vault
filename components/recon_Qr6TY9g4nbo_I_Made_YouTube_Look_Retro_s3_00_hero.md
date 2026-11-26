---
title: "Hero — Qr6TY9g4nbo_I_Made_YouTube_L (03:25.100)"
description: "Hero UI component (recon_Qr6TY9g4nbo_I_Made_YouTube_Look_Retro_s3_00_hero) with SSIM 0.9918, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_Qr6TY9g4nbo_I_Made_YouTube_Look_Retro_s3_00_hero"
category: "Hero"
ssim: 0.9918
quality_score: 8.72
tags: [hero, ui-design, design-tokens, react, flutter]
---

# Hero — Qr6TY9g4nbo_I_Made_YouTube_L (03:25.100)

> **Category:** [[05_Hero|Hero]] | **SSIM Fidelity:** `0.9918` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[10_ShaderCanvas|ShaderCanvas]], [[02_Button|Button]], [[04_Navbar|Navbar]]

Professional Hero reverse-engineered from Qr6TY9g4nbo_I_Made_YouTube_Look_Retro at 03:25.100. Features FADE_IN_SCALE micro-interaction animation with 16.14:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#151415` | `rgb(21, 20, 21)` | `oklch(0.19 0.003 325.7)` | `51.1%` |
| `surface` | `#848BA9` | `rgb(132, 139, 169)` | `oklch(0.64 0.046 274.7)` | `2.5%` |
| `accent` | `#E87D79` | `rgb(232, 125, 121)` | `oklch(0.71 0.133 23.2)` | `0.8%` |
| `text` | `#EFF0F4` | `rgb(239, 240, 244)` | `oklch(0.96 0.005 275.0)` | `10.4%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `30.1 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `2.45`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
// Reconstructed Hero component based on video context Qr6TY9g4nbo_I_Made_YouTube_Look_Retro.mp4 at 03:25.100
// Style: AUTO | Motion: FADE_IN_SCALE | Duration: 30100ms | Spring easing

import React from 'react'
import { motion } from 'framer-motion'

interface HeroProps {
  className?: string
}

export const Hero: React.FC<HeroProps> = ({ className }) => {
  const variants = {
    initial: { opacity: 0, scale: 0.95 },
    animate: { opacity: 1, scale: 1 },
  }

  const transition = {
    type: 'spring',
    stiffness: 260,
    damping: 20,
    duration: 30.1, // 30100ms converted to seconds for framer-motion
  }

  return (
    <section
      className={
        'relative w-full h-screen min-h-[720px] bg-[#151415] text-[#EFF0F4] overflow-hidden ' +
        className
      }
    >
      {/* Background video / image placeholder */}
      <div className="absolute inset-0 z-0">
        <video
          autoPlay
          muted
          loop
          playsInline
          className="w-full h-full object-cover"
          poster="https://images.unsplash.com/photo-1536440136628-849c177e76a1?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80"
        >
          <source src="#" type="video/mp4" />
          Your browser does not support the video tag.
        </video>
        <div className="absolute inset-0 bg-black/40" />
      </div>

      {/* Content overlay */}
      <motion.div
        variants={variants}
        initial="initial"
        animate="animate"
        transition={transition}
        className="relative z-10 flex 
```

## 4. Flutter / Dart Implementation

```dart
// Flutter StatefulWidget - Hero Component
// Reconstructed from video context Qr6TY9g4nbo_I_Made_YouTube_Look_Retro.mp4

import 'package:flutter/material.dart';

class HeroWidget extends StatefulWidget {
  const HeroWidget({Key? key}) : super(key: key);

  @override
  _HeroWidgetState createState() => _HeroWidgetState();
}

class _HeroWidgetState extends State<HeroWidget>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _opacity;
  late Animation<double> _scale;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 30100),
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
      backgroundColor: const Color(0xFF151415),
      body: Stack(
        children: [
          // Background video placeholder
          Positioned.fill(
            child: Image.network(
              'https://images.unsplash.com/photo-15364
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
