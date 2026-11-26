---
title: "Card — ZSNiSdB8Ens_CSS_animations_t (09:59.400)"
description: "Card UI component (recon_ZSNiSdB8Ens_CSS_animations_to_bring_your_site_to_life_s3_08_card) with SSIM 0.9953, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_ZSNiSdB8Ens_CSS_animations_to_bring_your_site_to_life_s3_08_card"
category: "Card"
ssim: 0.9953
quality_score: 8.72
tags: [card, ui-design, design-tokens, react, flutter]
---

# Card — ZSNiSdB8Ens_CSS_animations_t (09:59.400)

> **Category:** [[01_Card|Card]] | **SSIM Fidelity:** `0.9953` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[02_Button|Button]], [[03_GlassMenu|GlassMenu]], [[05_Hero|Hero]]

Professional Card reverse-engineered from ZSNiSdB8Ens_CSS_animations_to_bring_your_site_to_life at 09:59.400. Features FADE_IN_SCALE micro-interaction animation with 12.86:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#131418` | `rgb(19, 20, 24)` | `oklch(0.19 0.008 274.5)` | `44.6%` |
| `surface` | `#38383E` | `rgb(56, 56, 62)` | `oklch(0.34 0.010 285.8)` | `8.6%` |
| `accent` | `#111216` | `rgb(17, 18, 22)` | `oklch(0.18 0.008 274.4)` | `5.0%` |
| `text` | `#DCD6DA` | `rgb(220, 214, 218)` | `oklch(0.88 0.008 337.5)` | `1.6%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `167.733 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.01`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS
// Reverse-engineered from video context: ZSNiSdB8Ens_CSS_animations_to_bring_your_site_to_life.mp4 @ 09:59.400
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
      transition={
        type: 'spring',
        stiffness: 260,
        damping: 20
      }
      className={
        'w-[72px] h-[150px] bg-[#38383E] shadow-lg rounded-none border-none ' +
        (className || '')
      }
    >
      {children}
    </motion.div>
  );
};

// Usage example:
// <Card>
//   <div className="flex h-full items-center justify-center text-[#DCD6DA] text-xs font-medium">
//     Card Content
//   </div>
// </Card>
```

## 4. Flutter / Dart Implementation

```dart
// Flutter StatefulWidget
// Reverse-engineered from video context: ZSNiSdB8Ens_CSS_animations_to_bring_your_site_to_life.mp4 @ 09:59.400
import 'package:flutter/material.dart';

class CardComponent extends StatefulWidget {
  const CardComponent({Key? key}) : super(key: key);

  @override
  State<CardComponent> createState() => _CardComponentState();
}

class _CardComponentState extends State<CardComponent>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scaleAnimation;
  late Animation<double> _opacityAnimation;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 500),
    );
    _scaleAnimation = Tween<double>(begin: 0.95, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOut),
    );
    _opacityAnimation = Tween<double>(begin: 0.0, end: 1.0).animate(
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
          opacity: _opacityAnimation.value,
          child: Transform.scale(
  
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
