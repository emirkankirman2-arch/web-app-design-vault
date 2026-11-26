---
title: "Card — z5OguvQdoks_Parallax_with_CS (03:39.820)"
description: "Card UI component (recon_z5OguvQdoks_Parallax_with_CSS_Variables_SUMMARY_from_iOS_Button_Ho) with SSIM 0.9943, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_z5OguvQdoks_Parallax_with_CSS_Variables_SUMMARY_from_iOS_Button_Hover_@k_s3_02_card"
category: "Card"
ssim: 0.9943
quality_score: 8.72
tags: [card, ui-design, design-tokens, react, flutter]
---

# Card — z5OguvQdoks_Parallax_with_CS (03:39.820)

> **Category:** [[01_Card|Card]] | **SSIM Fidelity:** `0.9943` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[02_Button|Button]], [[03_GlassMenu|GlassMenu]], [[05_Hero|Hero]]

Professional Card reverse-engineered from z5OguvQdoks_Parallax_with_CSS_Variables_SUMMARY_from_iOS_Button_Hover_@k at 03:39.820. Features FADE_IN_SCALE micro-interaction animation with 8.06:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#F4B00D` | `rgb(244, 176, 13)` | `oklch(0.80 0.164 80.2)` | `95.6%` |
| `surface` | `#24252A` | `rgb(36, 37, 42)` | `oklch(0.27 0.009 276.7)` | `3.3%` |
| `accent` | `#F4B00D` | `rgb(244, 176, 13)` | `oklch(0.80 0.164 80.2)` | `5.0%` |
| `text` | `#24252A` | `rgb(36, 37, 42)` | `oklch(0.27 0.009 276.7)` | `3.3%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `119.519 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react'
import { motion } from 'framer-motion'

interface AutoCardProps {
  children?: React.ReactNode
  className?: string
}

export const AutoCard: React.FC<AutoCardProps> = ({ children, className }) => {
  const cardVariants = {
    initial: { opacity: 0, scale: 0.95 },
    animate: { opacity: 1, scale: 1 },
  }

  const cardTransition = {
    type: 'spring',
    stiffness: 260,
    damping: 20,
  }

  return (
    <motion.div
      variants={cardVariants}
      initial="initial"
      animate="animate"
      transition={cardTransition}
      className={
        'relative w-[298px] h-[248px] rounded-[28px] bg-[#F4B00D] shadow-lg overflow-hidden ' +
        (className || '')
      }
    >
      {children}
    </motion.div>
  )
}
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class AutoCard extends StatefulWidget {
  const AutoCard({Key? key}) : super(key: key);

  @override
  State<AutoCard> createState() => _AutoCardState();
}

class _AutoCardState extends State<AutoCard>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scale;
  late Animation<double> _opacity;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 1200),
    );
    _scale = Tween<double>(begin: 0.95, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOutBack),
    );
    _opacity = Tween<double>(begin: 0.0, end: 1.0).animate(
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
    return AnimatedBuilder(
      animation: _controller,
      builder: (context, child) {
        return Opacity(
          opacity: _opacity.value,
          child: Transform.scale(
            scale: _scale.value,
            child: Container(
              width: 298,
              height: 248,
              decoration: BoxDecoration(
                color: const Color(0xFFF4B00D),
      
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
