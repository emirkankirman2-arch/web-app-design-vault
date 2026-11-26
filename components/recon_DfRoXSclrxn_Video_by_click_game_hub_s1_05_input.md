---
title: "Input — DfRoXSclrxn_Video_by_click_g (00:00.000)"
description: "Input UI component (recon_DfRoXSclrxn_Video_by_click_game_hub_s1_05_input) with SSIM 0.9895, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_DfRoXSclrxn_Video_by_click.game.hub_s1_05_input"
category: "Input"
ssim: 0.9895
quality_score: 8.72
tags: [input, ui-design, design-tokens, react, flutter]
---

# Input — DfRoXSclrxn_Video_by_click_g (00:00.000)

> **Category:** [[06_Input|Input]] | **SSIM Fidelity:** `0.9895` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[02_Button|Button]], [[08_Modal|Modal]], [[09_SplashAuth|SplashAuth]]

Professional Input reverse-engineered from DfRoXSclrxn_Video_by_click.game.hub at 00:00.000. Features FADE_IN_SCALE micro-interaction animation with 13.37:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#17141A` | `rgb(23, 20, 26)` | `oklch(0.20 0.013 307.7)` | `59.0%` |
| `surface` | `#665F5F` | `rgb(102, 95, 95)` | `oklch(0.49 0.009 17.5)` | `2.5%` |
| `accent` | `#C45D2B` | `rgb(196, 93, 43)` | `oklch(0.60 0.146 44.1)` | `5.0%` |
| `text` | `#E0DCD8` | `rgb(224, 220, 216)` | `oklch(0.90 0.007 67.7)` | `4.8%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `5.067 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `18.48`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS
// Reconstructed from video evidence: Input component (Style: AUTO)
import React from 'react'
import { motion } from 'framer-motion'

interface InputProps {
  label?: string
  value?: string | number
  onChange?: (value: string) => void
  className?: string
}

export const Input: React.FC<InputProps> = ({
  label = 'COMMON',
  value = 50,
  onChange,
  className = '',
}) => {
  return (
    <motion.div
      initial={{ opacity: 0, scale: 0.95 }}
      animate={{ opacity: 1, scale: 1 }}
      transition={{ type: 'spring', stiffness: 260, damping: 20 }}
      className={
        'flex items-center gap-3 rounded-full border border-white/20 bg-[#17141A] px-4 py-2 text-sm font-mono text-[#E0DCD8] ' +
        className
      }
    >
      <span className="font-bold tracking-tight">{label}</span>
      <div className="w-3 h-3 rounded-full bg-[#C45D2B] shadow-[0_0_8px_rgba(196,93,43,0.6)]" />
      <span>{value}</span>
    </motion.div>
  )
}

// Usage example:
// <Input label="COMMON" value={50} />
```

## 4. Flutter / Dart Implementation

```dart
// Flutter StatefulWidget
import 'package:flutter/material.dart';

class InputWidget extends StatefulWidget {
  final String label;
  final int value;
  const InputWidget({super.key, this.label = 'COMMON', this.value = 50});

  @override
  State<InputWidget> createState() => _InputWidgetState();
}

class _InputWidgetState extends State<InputWidget>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scale;
  late Animation<double> _opacity;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 5066),
    );
    _scale = Tween<double>(begin: 0.95, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOut),
    );
    _opacity = Tween<double>(begin: 0.0, end: 1.0).animate(
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
              width: 143,
              hei
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
