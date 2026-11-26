---
title: "Card — panArZuRR0I_Sealed_classes_T (00:44.000)"
description: "Card UI component (recon_panArZuRR0I_Sealed_classes_Technique_of_the_Week_s2_01_card) with SSIM 0.995, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_panArZuRR0I_Sealed_classes_Technique_of_the_Week_s2_01_card"
category: "Card"
ssim: 0.995
quality_score: 8.72
tags: [card, ui-design, design-tokens, react, flutter]
---

# Card — panArZuRR0I_Sealed_classes_T (00:44.000)

> **Category:** [[01_Card|Card]] | **SSIM Fidelity:** `0.995` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[02_Button|Button]], [[03_GlassMenu|GlassMenu]], [[05_Hero|Hero]]

Professional Card reverse-engineered from panArZuRR0I_Sealed_classes_Technique_of_the_Week at 00:44.000. Features FADE_IN_SCALE micro-interaction animation with 10.11:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#0A2C58` | `rgb(10, 44, 88)` | `oklch(0.30 0.088 256.8)` | `28.5%` |
| `surface` | `#4A6377` | `rgb(74, 99, 119)` | `oklch(0.49 0.044 242.9)` | `2.8%` |
| `accent` | `#214064` | `rgb(33, 64, 100)` | `oklch(0.37 0.073 253.4)` | `5.8%` |
| `text` | `#C9E0E8` | `rgb(201, 224, 232)` | `oklch(0.89 0.027 220.7)` | `19.0%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `14.0 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react';
import { motion } from 'framer-motion';

interface CodeCardProps {
  filename?: string;
  code?: string;
  className?: string;
}

export const CodeCard: React.FC<CodeCardProps> = ({
  filename = 'offline_support.dart',
  code = 'class Offline extends AppState {\n}',
  className,
}) => {
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
      initial={variants.initial}
      animate={variants.animate}
      transition={transition}
      className={
        'relative w-full max-w-[625px] h-[407px] rounded-[28px] bg-[#0A2C58] shadow-2xl shadow-blue-900/20 overflow-hidden border border-[#214064]/30 ' +
        (className ?? '')
      }
    >
      {/* Tab bar */}
      <div className="absolute top-0 left-0 right-0 h-10 rounded-t-[28px] bg-[#4A6377]/20 flex items-center px-4 border-b border-[#214064]/30">
        <div className="flex items-center gap-2 text-xs text-[#C9E0E8]/80 font-mono">
          <span className="w-2 h-2 rounded-full bg-red-500/60"></span>
          <span className="w-2 h-2 rounded-full bg-yellow-500/60"></span>
          <span className="w-2 h-2 rounded-full bg-green-500/60"></span>
          <span className="ml-2">{filename}</span>
        </div>
      </div>

      {/* Code content */}
      <div className="absolute inset-0 p-8 flex items-center justify-center font-mono text-lg leading-relaxed text-[#C9E0E8]">
        <span className="text-[#4CAF50]">class </spa
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';
import 'package:google_fonts/google_fonts.dart';

class CodeCard extends StatefulWidget {
  final String filename;
  final String code;

  const CodeCard({
    Key? key,
    this.filename = 'offline_support.dart',
    this.code = 'class Offline extends AppState {\n}',
  }) : super(key: key);

  @override
  State<CodeCard> createState() => _CodeCardState();
}

class _CodeCardState extends State<CodeCard>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scale;
  late Animation<double> _opacity;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 1400),
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
       
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
