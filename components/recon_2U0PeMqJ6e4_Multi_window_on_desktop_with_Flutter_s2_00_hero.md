---
title: "Hero — 2U0PeMqJ6e4_Multi_window_on_ (04:22.888)"
description: "Hero UI component (recon_2U0PeMqJ6e4_Multi_window_on_desktop_with_Flutter_s2_00_hero) with SSIM 0.9916, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_2U0PeMqJ6e4_Multi-window_on_desktop_with_Flutter_s2_00_hero"
category: "Hero"
ssim: 0.9916
quality_score: 8.72
tags: [hero, ui-design, design-tokens, react, flutter]
---

# Hero — 2U0PeMqJ6e4_Multi_window_on_ (04:22.888)

> **Category:** [[05_Hero|Hero]] | **SSIM Fidelity:** `0.9916` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[10_ShaderCanvas|ShaderCanvas]], [[02_Button|Button]], [[04_Navbar|Navbar]]

Professional Hero reverse-engineered from 2U0PeMqJ6e4_Multi-window_on_desktop_with_Flutter at 04:22.888. Features FADE_IN_SCALE micro-interaction animation with 9.87:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#78CBE8` | `rgb(120, 203, 232)` | `oklch(0.80 0.091 222.6)` | `56.5%` |
| `surface` | `#A7E2EF` | `rgb(167, 226, 239)` | `oklch(0.88 0.062 212.8)` | `22.4%` |
| `accent` | `#DB9182` | `rgb(219, 145, 130)` | `oklch(0.73 0.093 32.0)` | `1.5%` |
| `text` | `#1F131A` | `rgb(31, 19, 26)` | `oklch(0.21 0.023 343.5)` | `12.7%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `57.808 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `0.84`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react'
import { motion } from 'framer-motion'

interface HeroSectionProps {
  className?: string
}

const HeroSection: React.FC<HeroSectionProps> = ({ className }) => {
  const heroVariants = {
    initial: { opacity: 0, scale: 0.95 },
    animate: { opacity: 1, scale: 1 },
  }

  const heroTransition = {
    type: 'spring',
    stiffness: 260,
    damping: 20,
  }

  return (
    <section
      className={
        'relative w-full min-h-screen bg-[#78CBE8] text-[#1F131A] overflow-hidden ' +
        className
      }
    >
      <motion.div
        variants={heroVariants}
        initial="initial"
        animate="animate"
        transition={heroTransition}
        className="flex flex-col items-center justify-center h-full px-4 sm:px-6 lg:px-8"
      >
        <div className="relative z-10 max-w-7xl w-full text-center">
          <h1
            className="text-5xl md:text-7xl font-bold tracking-tight mb-6 leading-tight"
          >
            Build beautiful interfaces<br />
            <span className="text-[#DB9182]">with Flutter & React</span>
          </h1>
          <p className="text-lg md:text-xl text-[#1F131A]/80 max-w-2xl mx-auto mb-10">
            Reconstructed from video evidence with precise design tokens,
            accessible markup, and smooth spring animations.
          </p>
          <div className="flex flex-col sm:flex-row gap-4 justify-center items-center">
            <button
              className="inline-flex items-center justify-center px-8 py-4 bg-[#DB9182] text-white font-semibold rounded-lg shadow-lg hover:bg-[#DB9182]/
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class HeroSection extends StatefulWidget {
  const HeroSection({Key? key}) : super(key: key);

  @override
  State<HeroSection> createState() => _HeroSectionState;
}

class _HeroSectionState extends State<HeroSection>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _opacity;
  late Animation<double> _scale;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 800),
    );
    _opacity = Tween<double>(begin: 0.0, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOutCubic),
    );
    _scale = Tween<double>(begin: 0.95, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOutCubic),
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
      backgroundColor: const Color(0xFF78CBE8),
      body: Stack(
        children: [
          // Decorative blobs
          Positioned.fill(
            child: IgnorePointer(
              child: Stack(
                children: [
                  Positioned(
                    top: -MediaQuery.of(context).size.height * 0.1,
                    l
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
