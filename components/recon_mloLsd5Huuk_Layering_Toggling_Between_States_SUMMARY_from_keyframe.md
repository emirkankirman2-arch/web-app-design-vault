---
title: "Card — mloLsd5Huuk_Layering_Togglin (03:23.637)"
description: "Card UI component (recon_mloLsd5Huuk_Layering_Toggling_Between_States_SUMMARY_from_keyframe) with SSIM 0.9947, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_mloLsd5Huuk_Layering_Toggling_Between_States_SUMMARY_from_@keyframers_3._s3_00_card"
category: "Card"
ssim: 0.9947
quality_score: 8.72
tags: [card, ui-design, design-tokens, react, flutter]
---

# Card — mloLsd5Huuk_Layering_Togglin (03:23.637)

> **Category:** [[01_Card|Card]] | **SSIM Fidelity:** `0.9947` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[02_Button|Button]], [[03_GlassMenu|GlassMenu]], [[05_Hero|Hero]]

Professional Card reverse-engineered from mloLsd5Huuk_Layering_Toggling_Between_States_SUMMARY_from_@keyframers_3. at 03:23.637. Features FADE_IN_SCALE micro-interaction animation with 8.14:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#EEB414` | `rgb(238, 180, 20)` | `oklch(0.80 0.161 84.6)` | `64.4%` |
| `surface` | `#24252A` | `rgb(36, 37, 42)` | `oklch(0.27 0.009 276.7)` | `30.8%` |
| `accent` | `#D1A21F` | `rgb(209, 162, 31)` | `oklch(0.74 0.143 86.4)` | `0.6%` |
| `text` | `#24252A` | `rgb(36, 37, 42)` | `oklch(0.27 0.009 276.7)` | `30.8%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `144.077 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react';
import { motion } from 'framer-motion';

interface CardProps {
  children?: React.ReactNode;
  className?: string;
}

export const Card: React.FC<CardProps> = ({ children, className }) => {
  return (
    <motion.div
      initial={{ opacity: 0, scale: 0.95 }}
      animate={{ opacity: 1, scale: 1 }}
      transition={{ type: 'spring', stiffness: 260, damping: 20 }}
      className={
        'relative w-[318px] h-[319px] rounded-[28px] bg-[#EEB414] shadow-lg overflow-hidden ' +
        (className ?? '')
      }
    >
      {children}
    </motion.div>
  );
};

// Example usage:
// <Card>
//   <div className="absolute inset-0 flex items-center justify-center">
//     <span className="text-9xl font-black text-[#24252A]">K</span>
//   </div>
// </Card>
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class CardWidget extends StatefulWidget {
  const CardWidget({super.key});

  @override
  State<CardWidget> createState() => _CardWidgetState();
}

class _CardWidgetState extends State<CardWidget> with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scale;
  late Animation<double> _opacity;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 800),
    );
    _scale = Tween<double>(begin: 0.95, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOutBack),
    );
    _opacity = Tween<double>(begin: 0.0, end: 1.0).animate(_controller);
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
              width: 318,
              height: 319,
              decoration: BoxDecoration(
                color: const Color(0xFFEEB414),
                borderRadius: BorderRadius.circular(28),
                box
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
