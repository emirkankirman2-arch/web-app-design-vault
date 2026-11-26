---
title: "Card — DcYlO_rhejc_Video_by_dreator (00:04.000)"
description: "Card UI component (recon_DcYlO_rhejc_Video_by_dreators1_s1_00_card) with SSIM 0.9938, OKLCH design tokens, FADE_AND_SLIDE_UP motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_DcYlO-rhejc_Video_by_dreators1_s1_00_card"
category: "Card"
ssim: 0.9938
quality_score: 8.72
tags: [card, ui-design, design-tokens, react, flutter]
---

# Card — DcYlO_rhejc_Video_by_dreator (00:04.000)

> **Category:** [[01_Card|Card]] | **SSIM Fidelity:** `0.9938` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[02_Button|Button]], [[03_GlassMenu|GlassMenu]], [[05_Hero|Hero]]

Professional Card reverse-engineered from DcYlO-rhejc_Video_by_dreators1 at 00:04.000. Features FADE_AND_SLIDE_UP micro-interaction animation with 18.76:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#000000` | `rgb(0, 0, 0)` | `oklch(0.00 0.000 0.0)` | `54.5%` |
| `surface` | `#3D3A43` | `rgb(61, 58, 67)` | `oklch(0.35 0.016 300.8)` | `0.6%` |
| `accent` | `#E6E5E6` | `rgb(230, 229, 230)` | `oklch(0.92 0.002 325.6)` | `5.0%` |
| `text` | `#F2F2F2` | `rgb(242, 242, 242)` | `oklch(0.96 0.000 89.9)` | `0.7%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_AND_SLIDE_UP`
- **Measured Duration:** `0.45 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `120.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
import React from 'react';
import { motion } from 'framer-motion';

export interface OTPAnimationCardProps {
  title?: string;
  className?: string;
}

export const OTPAnimationCard: React.FC<OTPAnimationCardProps> = ({
  title = 'OTP Animation V1',
  className,
}) => {
  return (
    <motion.div
      initial={{ opacity: 0, y: 24 }}
      animate={{ opacity: 1, y: 0 }}
      transition={
        duration: 0.45,
        ease: [0.16, 1, 0.3, 1]
      }
      className={
        'w-[220px] h-[26px] bg-black text-[#F2F2F2] flex items-center justify-center font-mono text-sm tracking-wide overflow-hidden ' +
        (className ?? '')
      }
      role="region"
      aria-label={title}
    >
      <span className="text-[#E6E5E6] font-semibold">{title}</span>
    </motion.div>
  );
};

export default OTPAnimationCard;
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class OTPAnimationCard extends StatefulWidget {
  final String title;
  const OTPAnimationCard({super.key, this.title = 'OTP Animation V1'});

  @override
  State<OTPAnimationCard> createState() => _OTPAnimationCardState();
}

class _OTPAnimationCardState extends State<OTPAnimationCard>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _opacity;
  late Animation<Offset> _offset;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 450),
    );
    _opacity = Tween<double>(begin: 0.0, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeInOut),
    );
    _offset = Tween<Offset>(begin: const Offset(0, 0.5), end: Offset.zero).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeInOut),
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
    return SlideTransition(
      position: _offset,
      child: FadeTransition(
        opacity: _opacity,
        child: SizedBox(
          width: 220,
          height: 26,
          child: Center(
            child: Text(
              widget.title,
              style: const T
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
