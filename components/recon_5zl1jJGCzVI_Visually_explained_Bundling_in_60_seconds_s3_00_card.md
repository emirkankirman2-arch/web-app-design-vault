---
title: "Card — 5zl1jJGCzVI_Visually_explain (00:38.000)"
description: "Card UI component (recon_5zl1jJGCzVI_Visually_explained_Bundling_in_60_seconds_s3_00_card) with SSIM 0.9947, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_5zl1jJGCzVI_Visually_explained_-_Bundling_in_60_seconds_s3_00_card"
category: "Card"
ssim: 0.9947
quality_score: 8.72
tags: [card, ui-design, design-tokens, react, flutter]
---

# Card — 5zl1jJGCzVI_Visually_explain (00:38.000)

> **Category:** [[01_Card|Card]] | **SSIM Fidelity:** `0.9947` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[02_Button|Button]], [[03_GlassMenu|GlassMenu]], [[05_Hero|Hero]]

Professional Card reverse-engineered from 5zl1jJGCzVI_Visually_explained_-_Bundling_in_60_seconds at 00:38.000. Features FADE_IN_SCALE micro-interaction animation with 4.65:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#000000` | `rgb(0, 0, 0)` | `oklch(0.00 0.000 0.0)` | `90.7%` |
| `surface` | `#3A3534` | `rgb(58, 53, 52)` | `oklch(0.33 0.007 31.1)` | `1.0%` |
| `accent` | `#030102` | `rgb(3, 1, 2)` | `oklch(0.08 0.013 345.0)` | `5.0%` |
| `text` | `#787676` | `rgb(120, 118, 118)` | `oklch(0.57 0.002 17.2)` | `0.1%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `14.0 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react'
import { motion } from 'framer-motion'

interface CardProps {
  children?: React.ReactNode
  className?: string
}

export const Card: React.FC<CardProps> = ({ children, className }) => {
  return (
    <motion.div
      initial={{ opacity: 0, scale: 0.95 }}
      animate={{ opacity: 1, scale: 1 }}
      transition={{ type: 'spring', stiffness: 260, damping: 20 }}
      className={
        'bg-[#3A3534] text-[#787676] rounded-none shadow-lg w-42 h-7 flex items-center justify-center font-mono text-sm tracking-widest uppercase ' +
        (className || '')
      }
    >
      {children}
    </motion.div>
  )
}

// Usage example:
// <Card>BUNDLES</Card>
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class CardWidget extends StatefulWidget {
  final String text;
  const CardWidget({super.key, this.text = 'BUNDLES'});

  @override
  State<CardWidget> createState() => _CardWidgetState();
}

class _CardWidgetState extends State<CardWidget> with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _opacity;
  late Animation<double> _scale;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 1400),
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
    return AnimatedBuilder(
      animation: _controller,
      builder: (context, child) {
        return Opacity(
          opacity: _opacity.value,
          child: Transform.scale(
            scale: _scale.value,
            child: Container(
              width: 168,
              height: 28,
              decoration: BoxDecoration(
                color: 
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
