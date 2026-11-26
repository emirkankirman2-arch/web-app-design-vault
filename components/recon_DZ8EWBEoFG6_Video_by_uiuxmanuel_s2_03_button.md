---
title: "Button — DZ8EWBEoFG6_Video_by_uiuxman (00:08.000)"
description: "Button UI component (recon_DZ8EWBEoFG6_Video_by_uiuxmanuel_s2_03_button) with SSIM 0.9903, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_DZ8EWBEoFG6_Video_by_uiuxmanuel_s2_03_button"
category: "Button"
ssim: 0.9903
quality_score: 8.72
tags: [button, ui-design, design-tokens, react, flutter]
---

# Button — DZ8EWBEoFG6_Video_by_uiuxman (00:08.000)

> **Category:** [[02_Button|Button]] | **SSIM Fidelity:** `0.9903` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[01_Card|Card]], [[06_Input|Input]], [[08_Modal|Modal]]

Professional Button reverse-engineered from DZ8EWBEoFG6_Video_by_uiuxmanuel at 00:08.000. Features FADE_IN_SCALE micro-interaction animation with 14.72:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#EEECEF` | `rgb(238, 236, 239)` | `oklch(0.95 0.005 314.8)` | `84.7%` |
| `surface` | `#E3E1E4` | `rgb(227, 225, 228)` | `oklch(0.91 0.005 314.8)` | `7.3%` |
| `accent` | `#7F7D80` | `rgb(127, 125, 128)` | `oklch(0.59 0.005 314.8)` | `5.0%` |
| `text` | `#1C1A1D` | `rgb(28, 26, 29)` | `oklch(0.22 0.006 314.7)` | `1.3%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `18.0 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react'
import { motion } from 'framer-motion'

interface AutoButtonProps {
  children?: React.ReactNode
  className?: string
  onClick?: () => void
  disabled?: boolean
}

export const AutoButton: React.FC<AutoButtonProps> = ({
  children,
  className = '',
  onClick,
  disabled = false,
}) => {
  const buttonVariants = {
    initial: { opacity: 0, scale: 0.95 },
    animate: { opacity: 1, scale: 1 },
    hover: { scale: 1.02 },
    tap: { scale: 0.98 },
  }

  const buttonTransition = {
    type: 'spring',
    stiffness: 260,
    damping: 20,
  }

  return (
    <motion.button
      aria-disabled={disabled}
      disabled={disabled}
      onClick={onClick}
      whileHover={!disabled ? 'hover' : undefined}
      whileTap={!disabled ? 'tap' : undefined}
      variants={buttonVariants}
      initial="initial"
      animate="animate"
      transition={buttonTransition}
      className={
        'inline-flex items-center justify-center whitespace-nowrap rounded-none border-none font-medium text-[1C1A1D] transition-colors duration-200 ' +
        (disabled
          ? 'bg-E3E1E4 text-7F7D80 cursor-not-allowed'
          : 'bg-EEECEF hover:bg-E3E1E4 active:bg-E3E1E4 shadow-sm cursor-pointer') +
        ' ' +
        className
      }
      style={
        {
          minWidth: '103px',
          height: '26px',
          padding: '0 12px',
          ...(disabled && { opacity: 0.6 }),
        } as React.CSSProperties
      }
    >
      {children}
    </motion.button>
  )
}

export default AutoButton
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class AutoButton extends StatefulWidget {
  final Widget? child;
  final VoidCallback? onPressed;
  final bool enabled;
  final String? semanticsLabel;

  const AutoButton({
    super.key,
    this.child,
    this.onPressed,
    this.enabled = true,
    this.semanticsLabel,
  });

  @override
  State<AutoButton> createState() => _AutoButtonState();
}

class _AutoButtonState extends State<AutoButton>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scale;
  late Animation<double> _opacity;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 18000),
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
            
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
