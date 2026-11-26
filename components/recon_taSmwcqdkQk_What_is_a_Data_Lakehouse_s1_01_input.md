---
title: "Input — taSmwcqdkQk_What_is_a_Data_L (00:11.440)"
description: "Input UI component (recon_taSmwcqdkQk_What_is_a_Data_Lakehouse_s1_01_input) with SSIM 0.9873, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_taSmwcqdkQk_What_is_a_Data_Lakehouse_s1_01_input"
category: "Input"
ssim: 0.9873
quality_score: 8.72
tags: [input, ui-design, design-tokens, react, flutter]
---

# Input — taSmwcqdkQk_What_is_a_Data_L (00:11.440)

> **Category:** [[06_Input|Input]] | **SSIM Fidelity:** `0.9873` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[02_Button|Button]], [[08_Modal|Modal]], [[09_SplashAuth|SplashAuth]]

Professional Input reverse-engineered from taSmwcqdkQk_What_is_a_Data_Lakehouse at 00:11.440. Features FADE_IN_SCALE micro-interaction animation with 7.96:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#252525` | `rgb(37, 37, 37)` | `oklch(0.26 0.000 89.9)` | `94.9%` |
| `surface` | `#3B403C` | `rgb(59, 64, 60)` | `oklch(0.37 0.010 151.6)` | `1.7%` |
| `accent` | `#6BC7E3` | `rgb(107, 199, 227)` | `oklch(0.78 0.096 220.0)` | `0.3%` |
| `text` | `#6BC7E3` | `rgb(107, 199, 227)` | `oklch(0.78 0.096 220.0)` | `0.3%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `80.08 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react';
import { motion } from 'framer-motion';

interface InputProps {
  placeholder?: string;
  value?: string;
  onChange?: (e: React.ChangeEvent<HTMLInputElement>) => void;
  className?: string;
}

export const Input: React.FC<InputProps> = ({
  placeholder = 'Enter text...',
  value,
  onChange,
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
        placeholder={placeholder}
        value={value}
        onChange={onChange}
        className={\`w-full h-[38px] bg-[#252525] border-none outline-none text-[#6BC7E3] placeholder:text-[#6BC7E3]/50 text-sm font-medium transition-colors focus:ring-2 focus:ring-[#6BC7E3] \${className}\`}
        aria-label="Input field"
      />
    </motion.div>
  );
};

// Usage example:
// <Input placeholder="Search..." onChange={(e) => console.log(e.target.value)} />
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class InputWidget extends StatefulWidget {
  final String placeholder;
  final String? value;
  final ValueChanged<String>? onChanged;

  const InputWidget({
    Key? key,
    this.placeholder = 'Enter text...',
    this.value,
    this.onChanged,
  }) : super(key: key);

  @override
  State<InputWidget> createState() => _InputWidgetState();
}

class _InputWidgetState extends State<InputWidget>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scaleAnimation;
  late Animation<double> _opacityAnimation;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 800),
    );
    _scaleAnimation = Tween<double>(begin: 0.95, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOutBack),
    );
    _opacityAnimation = Tween<double>(begin: 0.0, end: 1.0).animate(
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
          opacity: _opacityAnimation.value,
     
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
