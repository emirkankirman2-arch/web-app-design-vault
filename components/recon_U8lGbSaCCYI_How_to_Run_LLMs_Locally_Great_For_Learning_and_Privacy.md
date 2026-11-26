---
title: "Button — U8lGbSaCCYI_How_to_Run_LLMs_ (03:24.329)"
description: "Button UI component (recon_U8lGbSaCCYI_How_to_Run_LLMs_Locally_Great_For_Learning_and_Privacy) with SSIM 0.9944, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_U8lGbSaCCYI_How_to_Run_LLMs_Locally_Great_For_Learning_and_Privacy_s2_04_button"
category: "Button"
ssim: 0.9944
quality_score: 8.72
tags: [button, ui-design, design-tokens, react, flutter]
---

# Button — U8lGbSaCCYI_How_to_Run_LLMs_ (03:24.329)

> **Category:** [[02_Button|Button]] | **SSIM Fidelity:** `0.9944` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[01_Card|Card]], [[06_Input|Input]], [[08_Modal|Modal]]

Professional Button reverse-engineered from U8lGbSaCCYI_How_to_Run_LLMs_Locally_Great_For_Learning_and_Privacy at 03:24.329. Features FADE_IN_SCALE micro-interaction animation with 8.55:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#202020` | `rgb(32, 32, 32)` | `oklch(0.24 0.000 89.9)` | `87.3%` |
| `surface` | `#727373` | `rgb(114, 115, 115)` | `oklch(0.55 0.001 197.1)` | `3.3%` |
| `accent` | `#BE505B` | `rgb(190, 80, 91)` | `oklch(0.58 0.142 16.6)` | `5.0%` |
| `text` | `#44D575` | `rgb(68, 213, 117)` | `oklch(0.77 0.182 150.6)` | `1.7%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `71.947 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.17`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react'
import { motion } from 'framer-motion'

interface AutoButtonProps {
  children?: React.ReactNode
  onClick?: () => void
  className?: string
}

export const AutoButton: React.FC<AutoButtonProps> = ({
  children,
  onClick,
  className = '',
}) => {
  const variants = {
    initial: { opacity: 0, scale: 0.95 },
    animate: { opacity: 1, scale: 1 },
  }

  const transition = {
    type: 'spring',
    stiffness: 260,
    damping: 20,
  }

  return (
    <motion.button
      variants={variants}
      initial="initial"
      animate="animate"
      transition={transition}
      onClick={onClick}
      className={
        'relative inline-flex items-center justify-center w-[151px] h-[68px] rounded-none bg-[#BE505B] text-white font-medium shadow-lg shadow-black/50 focus:outline-none focus:ring-2 focus:ring-[#BE505B] focus:ring-offset-2 focus:ring-offset-[#202020] active:scale-95 transition-transform duration-200 disabled:opacity-50 disabled:pointer-events-none ' +
        className
      }
    >
      {children}
    </motion.button>
  )
}

// Usage example:
// <AutoButton onClick={handleClick}>Run LLMs Locally</AutoButton>

// Export default for convenience
export default AutoButton
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class AutoButton extends StatefulWidget {
  final VoidCallback? onPressed;
  final Widget? child;

  const AutoButton({Key? key, this.onPressed, this.child}) : super(key: key);

  @override
  State<AutoButton> createState() => _AutoButtonState();
}

class _AutoButtonState extends State<AutoButton>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scaleAnimation;
  late Animation<double> _opacityAnimation;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 700),
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
            child: SizedBox(
  
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
