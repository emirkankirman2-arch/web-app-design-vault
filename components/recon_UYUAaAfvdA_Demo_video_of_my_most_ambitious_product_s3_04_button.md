---
title: "Button — UYUAaAfvdA_Demo_video_of_my_ (11:08.434)"
description: "Button UI component (recon_UYUAaAfvdA_Demo_video_of_my_most_ambitious_product_s3_04_button) with SSIM 0.9925, OKLCH design tokens, SLIDE_UP motion spec, React/Tailwind & Flutter implementations."
component_id: "recon__UYUAaAfvdA_Demo_video_of_my_most_ambitious_product_s3_04_button"
category: "Button"
ssim: 0.9925
quality_score: 8.72
tags: [button, ui-design, design-tokens, react, flutter]
---

# Button — UYUAaAfvdA_Demo_video_of_my_ (11:08.434)

> **Category:** [[02_Button|Button]] | **SSIM Fidelity:** `0.9925` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[01_Card|Card]], [[06_Input|Input]], [[08_Modal|Modal]]

Professional Button reverse-engineered from _UYUAaAfvdA_Demo_video_of_my_most_ambitious_product at 11:08.434. Features SLIDE_UP micro-interaction animation with 10.16:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#110E18` | `rgb(17, 14, 24)` | `oklch(0.17 0.021 297.9)` | `48.6%` |
| `surface` | `#726B75` | `rgb(114, 107, 117)` | `oklch(0.54 0.018 315.9)` | `5.4%` |
| `accent` | `#0D1043` | `rgb(13, 16, 67)` | `oklch(0.21 0.094 272.6)` | `5.0%` |
| `text` | `#B6BEC7` | `rgb(182, 190, 199)` | `oklch(0.80 0.016 251.2)` | `4.0%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `SLIDE_UP`
- **Measured Duration:** `67.067 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `0.31`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react'
import { motion } from 'framer-motion'

type AutoButtonProps = {
  children: React.ReactNode
  onClick?: () => void
  className?: string
  disabled?: boolean
}

export const AutoButton: React.FC<AutoButtonProps> = ({
  children,
  onClick,
  className,
  disabled = false
}) => {
  return (
    <motion.button
      className={
        'relative inline-flex items-center justify-center w-20 h-10.5 rounded-lg bg-[#110E18] px-4 py-2 text-sm font-medium text-[#B6BEC7] shadow-lg transition-all duration-200 ease-out disabled:opacity-50 disabled:pointer-events-none ' +
        (className ?? '')
      }
      onClick={disabled ? undefined : onClick}
      disabled={disabled}
      whileHover={{ scale: 1.02, boxShadow: '0 0 20px rgba(13, 16, 67, 0.4)' }}
      whileTap={{ scale: 0.98 }}
      initial={{ opacity: 0, y: 9.85 }}
      animate={{ opacity: 1, y: 0 }}
      transition={{ duration: 67.07, ease: [0.16, 1, 0.3, 1] }}
    >
      {children}
    </motion.button>
  )
}

// Usage example:
// <AutoButton onClick={() => console.log('clicked')}>Click Me</AutoButton>
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class AutoButton extends StatefulWidget {
  final Widget child;
  final VoidCallback? onPressed;
  final bool enabled;

  const AutoButton({
    super.key,
    required this.child,
    this.onPressed,
    this.enabled = true,
  });

  @override
  State<AutoButton> createState() => _AutoButtonState();
}

class _AutoButtonState extends State<AutoButton>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scale;
  late Animation<Offset> _offset;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 67067),
    );
    _scale = Tween<double>(begin: 0.98, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOut),
    );
    _offset = Tween<Offset>(begin: const Offset(0, 0.1), end: Offset.zero).animate(
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
        return Transform.translate(
          offset: Offset(0, _offset.value.dy * 9.85),
          child: Transform.scale(
       
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
