---
title: "Hero — Dd2upTghZBK_Video_by_wearepi (00:00.000)"
description: "Hero UI component (recon_Dd2upTghZBK_Video_by_wearepixelflow_s1_00_hero) with SSIM 0.9956, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_Dd2upTghZBK_Video_by_wearepixelflow_s1_00_hero"
category: "Hero"
ssim: 0.9956
quality_score: 8.72
tags: [hero, ui-design, design-tokens, react, flutter]
---

# Hero — Dd2upTghZBK_Video_by_wearepi (00:00.000)

> **Category:** [[05_Hero|Hero]] | **SSIM Fidelity:** `0.9956` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[10_ShaderCanvas|ShaderCanvas]], [[02_Button|Button]], [[04_Navbar|Navbar]]

Professional Hero reverse-engineered from Dd2upTghZBK_Video_by_wearepixelflow at 00:00.000. Features FADE_IN_SCALE micro-interaction animation with 12.04:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#000000` | `rgb(0, 0, 0)` | `oklch(0.00 0.000 0.0)` | `52.8%` |
| `surface` | `#5E5E60` | `rgb(94, 94, 96)` | `oklch(0.48 0.003 286.3)` | `0.1%` |
| `accent` | `#C4C4C4` | `rgb(196, 196, 196)` | `oklch(0.82 0.000 89.9)` | `0.0%` |
| `text` | `#C4C4C4` | `rgb(196, 196, 196)` | `oklch(0.82 0.000 89.9)` | `0.0%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `6.0 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
import React from 'react';
import { motion } from 'framer-motion';

export default function HeroConnect() {
  return (
    <div className="fixed inset-0 bg-black text-[#C4C4C4] flex items-center justify-center font-mono antialiased">
      <motion.div
        initial={{ opacity: 0, scale: 0.95 }}
        animate={{ opacity: 1, scale: 1 }}
        transition={{ type: 'spring', stiffness: 260, damping: 20 }}
        className="relative w-full max-w-[405px] h-[720px] flex flex-col items-center justify-center p-6"
      >
        {/* Decorative outer glow ring */}
        <div className="absolute inset-0 rounded-full bg-white/5 blur-[40px] animate-pulse" />

        {/* Main pill container */}
        <div className="relative inline-flex items-center gap-1 px-4 py-2 rounded-full bg-[#111111] border border-white/10 shadow-[0_0_20px_rgba(196,196,196,0.15)]">
          {['C','O','N','N','E','C','T'].map((letter, idx) => (
            <div
              key={idx}
              className="w-8 h-8 rounded-full flex items-center justify-center text-xs font-bold tracking-widest transition-colors duration-300 hover:bg-white/10"
              style={{ color: '#C4C4C4' }}
            >
              {letter}
            </div>
          ))}
        </div>

        {/* Subtle underline accent */}
        <div className="mt-4 w-1/3 h-[1px] bg-white/20 rounded-full" />
      </motion.div>
    </div>
  );
}
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class HeroConnect extends StatefulWidget {
  const HeroConnect({super.key});

  @override
  State<HeroConnect> createState() => _HeroConnectState();
}

class _HeroConnectState extends State<HeroConnect> with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scale;
  late Animation<double> _opacity;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(vsync: this, duration: const Duration(milliseconds: 6000))
      ..forward();
    final curved = CurvedAnimation(parent: _controller, curve: Curves.easeOut);
    _scale = Tween<double>(begin: 0.95, end: 1.0).animate(curved);
    _opacity = Tween<double>(begin: 0.0, end: 1.0).animate(curved);
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
        child: AnimatedBuilder(
          animation: _controller,
          builder: (context, child) {
            return Opacity(
              opacity: _opacity.value,
              child: Transform.scale(
                scale: _scale.value,
                child: SizedBox(
                  width: 405,
                  height: 720,
                  child: Column(
                    mainAxisAli
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
