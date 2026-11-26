---
title: "Input — MUWAbpg1xLo_CPU_vs_GPU_vs_TP (00:08.360)"
description: "Input UI component (recon_MUWAbpg1xLo_CPU_vs_GPU_vs_TPU_s1_02_input) with SSIM 0.9889, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_MUWAbpg1xLo_CPU_vs_GPU_vs_TPU_s1_02_input"
category: "Input"
ssim: 0.9889
quality_score: 8.72
tags: [input, ui-design, design-tokens, react, flutter]
---

# Input — MUWAbpg1xLo_CPU_vs_GPU_vs_TP (00:08.360)

> **Category:** [[06_Input|Input]] | **SSIM Fidelity:** `0.9889` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[02_Button|Button]], [[08_Modal|Modal]], [[09_SplashAuth|SplashAuth]]

Professional Input reverse-engineered from MUWAbpg1xLo_CPU_vs_GPU_vs_TPU at 00:08.360. Features FADE_IN_SCALE micro-interaction animation with 8.81:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#252525` | `rgb(37, 37, 37)` | `oklch(0.26 0.000 89.9)` | `86.5%` |
| `surface` | `#374C48` | `rgb(55, 76, 72)` | `oklch(0.40 0.027 181.9)` | `5.6%` |
| `accent` | `#DCC52C` | `rgb(220, 197, 44)` | `oklch(0.82 0.159 100.1)` | `0.9%` |
| `text` | `#DCC52C` | `rgb(220, 197, 44)` | `oklch(0.82 0.159 100.1)` | `0.9%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `51.68 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react'
import { motion } from 'framer-motion'

interface InputProps {
  value?: string
  onChange?: (e: React.ChangeEvent<HTMLInputElement>) => void
  placeholder?: string
  className?: string
}

export const Input: React.FC<InputProps> = ({
  value,
  onChange,
  placeholder,
  className,
}) => {
  return (
    <motion.div
      initial={{ opacity: 0, scale: 0.95 }}
      animate={{ opacity: 1, scale: 1 }}
      transition={{ type: 'spring', stiffness: 260, damping: 20 }}
      className={\`relative w-full \${className}\`}
    >
      <input
        type="text"
        value={value}
        onChange={onChange}
        placeholder={placeholder}
        className={\`w-full h-8 bg-[#252525] border-none text-[#DCC52C] placeholder-gray-500 text-sm font-mono outline-none focus:ring-0 disabled:opacity-50 \${className}\`}
        autoComplete="off"
        spellCheck={false}
      />
    </motion.div>
  )
}

// Usage example:
// <Input placeholder="CPU vs GPU vs TPU" className="w-[314px]" />
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class InputWidget extends StatefulWidget {
  final String? value;
  final ValueChanged<String>? onChanged;
  final String? placeholder;

  const InputWidget({Key? key, this.value, this.onChanged, this.placeholder}) : super(key: key);

  @override
  State<InputWidget> createState() => _InputWidgetState();
}

class _InputWidgetState extends State<InputWidget> with SingleTickerProviderStateMixin {
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
            scal
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
