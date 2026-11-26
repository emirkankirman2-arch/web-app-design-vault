---
title: "Card — SglP_F5FWhY_Convince_the_top (00:02.933)"
description: "Card UI component (recon_SglP_F5FWhY_Convince_the_top_3_LLMs_why_your_comment_should_win_s1) with SSIM 0.9956, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_SglP-F5FWhY_Convince_the_top_3_LLMs_why_your_comment_should_win_s1_01_card"
category: "Card"
ssim: 0.9956
quality_score: 8.72
tags: [card, ui-design, design-tokens, react, flutter]
---

# Card — SglP_F5FWhY_Convince_the_top (00:02.933)

> **Category:** [[01_Card|Card]] | **SSIM Fidelity:** `0.9956` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[02_Button|Button]], [[03_GlassMenu|GlassMenu]], [[05_Hero|Hero]]

Professional Card reverse-engineered from SglP-F5FWhY_Convince_the_top_3_LLMs_why_your_comment_should_win at 00:02.933. Features FADE_IN_SCALE micro-interaction animation with 18.76:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#000000` | `rgb(0, 0, 0)` | `oklch(0.00 0.000 0.0)` | `73.0%` |
| `surface` | `#8E8E8E` | `rgb(142, 142, 142)` | `oklch(0.65 0.000 89.9)` | `2.4%` |
| `accent` | `#B2B2B2` | `rgb(178, 178, 178)` | `oklch(0.76 0.000 89.9)` | `2.1%` |
| `text` | `#F2F2F2` | `rgb(242, 242, 242)` | `oklch(0.96 0.000 89.9)` | `2.7%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `42.533 s`
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
  const variants = {
    initial: { opacity: 0, scale: 0.95 },
    animate: { opacity: 1, scale: 1 },
  };

  const transition = {
    type: 'spring',
    stiffness: 260,
    damping: 20,
  };

  return (
    <motion.div
      initial="initial"
      animate="animate"
      transition={transition}
      className={
        'relative rounded-2xl bg-gray-800 p-6 shadow-xl border border-gray-700 ' +
        (className ?? '')
      }
    >
      {children}
    </motion.div>
  );
};

export default Card;
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
              width: 620,
              height: 211,
              decoration: BoxDecoration(
                color: const Color(0xFF8E8E8E),
                
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
