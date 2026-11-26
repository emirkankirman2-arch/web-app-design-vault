---
title: "Input — MUWAbpg1xLo_CPU_vs_GPU_vs_TP (02:38.840)"
description: "Input UI component (recon_MUWAbpg1xLo_CPU_vs_GPU_vs_TPU_s2_00_input) with SSIM 0.9895, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_MUWAbpg1xLo_CPU_vs_GPU_vs_TPU_s2_00_input"
category: "Input"
ssim: 0.9895
quality_score: 8.72
tags: [input, ui-design, design-tokens, react, flutter]
---

# Input — MUWAbpg1xLo_CPU_vs_GPU_vs_TP (02:38.840)

> **Category:** [[06_Input|Input]] | **SSIM Fidelity:** `0.9895` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[02_Button|Button]], [[08_Modal|Modal]], [[09_SplashAuth|SplashAuth]]

Professional Input reverse-engineered from MUWAbpg1xLo_CPU_vs_GPU_vs_TPU at 02:38.840. Features FADE_IN_SCALE micro-interaction animation with 15.07:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#252525` | `rgb(37, 37, 37)` | `oklch(0.26 0.000 89.9)` | `72.3%` |
| `surface` | `#4A4C4C` | `rgb(74, 76, 76)` | `oklch(0.41 0.003 197.1)` | `4.2%` |
| `accent` | `#3BCFE4` | `rgb(59, 207, 228)` | `oklch(0.79 0.123 209.1)` | `0.4%` |
| `text` | `#FDFDFD` | `rgb(253, 253, 253)` | `oklch(0.99 0.000 89.9)` | `12.2%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `51.68 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
// Reconstructed from video evidence: MUWAbpg1xLo_CPU_vs_GPU_vs_TPU.mp4 @ 02:38.840
import React from 'react'
import { motion } from 'framer-motion'

interface ByteByteGoInputProps {
  placeholder?: string
  value?: string
  onChange?: (e: React.ChangeEvent<HTMLInputElement>) => void
  className?: string
}

export const ByteByteGoInput: React.FC<ByteByteGoInputProps> = ({
  placeholder = 'Search...',
  value,
  onChange,
  className,
}) => {
  return (
    <motion.div
      initial={{ opacity: 0, scale: 0.95 }}
      animate={{ opacity: 1, scale: 1.0 }}
      transition={{ type: 'spring', stiffness: 260, damping: 20 }}
      className={
        'relative w-[234px] h-[41px] ' + (className || '')
      }
    >
      <input
        type="text"
        placeholder={placeholder}
        value={value}
        onChange={onChange}
        className={
          'w-full h-full bg-[#252525] border-none text-[#FDFDFD] ' +
          'placeholder-[#4A4C4C]/60 focus:outline-none focus:ring-2 focus:ring-[#3BCFE4] ' +
          'text-sm font-sans leading-none ' +
          'transition-colors duration-200 ease-in-out'
        }
        aria-label="Search input"
        autoComplete="off"
        spellCheck={false}
      />
    </motion.div>
  )
}

// Usage example:
// <ByteByteGoInput placeholder="Search ByteByteGo..." />
```

## 4. Flutter / Dart Implementation

```dart
// Flutter StatefulWidget
// Reconstructed from video evidence: MUWAbpg1xLo_CPU_vs_GPU_vs_TPU.mp4 @ 02:38.840
import 'package:flutter/material.dart';

class ByteByteGoInput extends StatefulWidget {
  final String placeholder;
  final String? value;
  final ValueChanged<String>? onChanged;

  const ByteByteGoInput({
    Key? key,
    this.placeholder = 'Search...',
    this.value,
    this.onChanged,
  }) : super(key: key);

  @override
  State<ByteByteGoInput> createState() => _ByteByteGoInputState();
}

class _ByteByteGoInputState extends State<ByteByteGoInput>
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
      anim
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
