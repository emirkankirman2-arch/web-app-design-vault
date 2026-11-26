---
title: "Card — h6Bp7DilFTA_Can_we_Make_A_CS (09:37.600)"
description: "Card UI component (recon_h6Bp7DilFTA_Can_we_Make_A_CSS_Only_Logo_Marquee_With_ZERO_Repetiti) with SSIM 0.995, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_h6Bp7DilFTA_Can_we_Make_A_CSS_Only_Logo_Marquee_With_ZERO_Repetition_s2_00_card"
category: "Card"
ssim: 0.995
quality_score: 8.72
tags: [card, ui-design, design-tokens, react, flutter]
---

# Card — h6Bp7DilFTA_Can_we_Make_A_CS (09:37.600)

> **Category:** [[01_Card|Card]] | **SSIM Fidelity:** `0.995` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[02_Button|Button]], [[03_GlassMenu|GlassMenu]], [[05_Hero|Hero]]

Professional Card reverse-engineered from h6Bp7DilFTA_Can_we_Make_A_CSS_Only_Logo_Marquee_With_ZERO_Repetition at 09:37.600. Features FADE_IN_SCALE micro-interaction animation with 17.48:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#121212` | `rgb(18, 18, 18)` | `oklch(0.18 0.000 89.9)` | `59.5%` |
| `surface` | `#4B494B` | `rgb(75, 73, 75)` | `oklch(0.41 0.004 325.7)` | `8.8%` |
| `accent` | `#174D74` | `rgb(23, 77, 116)` | `oklch(0.41 0.086 244.5)` | `0.4%` |
| `text` | `#F7F7F6` | `rgb(247, 247, 246)` | `oklch(0.98 0.001 106.4)` | `1.6%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `158.08 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.12`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
import { motion } from 'framer-motion';

export interface CardProps {
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
        'relative w-[610px] h-[342px] rounded-xl bg-[#4B494B] shadow-lg overflow-hidden ' +
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
  const CardWidget({Key? key}) : super(key: key);

  @override
  State<CardWidget> createState() => _CardWidgetState();
}

class _CardWidgetState extends State<CardWidget> with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scaleAnimation;
  late Animation<double> _opacityAnimation;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 1580),
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
            scale: _scaleAnimation.value,
            child: Container(
              width: 610,
              height: 342,
              decoration: BoxDecorat
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
