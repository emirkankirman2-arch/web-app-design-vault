---
title: "Button — DcJ42FZu0v6_Video_by_figma_c (00:00.000)"
description: "Button UI component (recon_DcJ42FZu0v6_Video_by_figma_create_s1_01_button) with SSIM 0.994, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_DcJ42FZu0v6_Video_by_figma.create_s1_01_button"
category: "Button"
ssim: 0.994
quality_score: 8.72
tags: [button, ui-design, design-tokens, react, flutter]
---

# Button — DcJ42FZu0v6_Video_by_figma_c (00:00.000)

> **Category:** [[02_Button|Button]] | **SSIM Fidelity:** `0.994` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[01_Card|Card]], [[06_Input|Input]], [[08_Modal|Modal]]

Professional Button reverse-engineered from DcJ42FZu0v6_Video_by_figma.create at 00:00.000. Features FADE_IN_SCALE micro-interaction animation with 8.55:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#000000` | `rgb(0, 0, 0)` | `oklch(0.00 0.000 0.0)` | `69.3%` |
| `surface` | `#77848D` | `rgb(119, 132, 141)` | `oklch(0.61 0.021 238.0)` | `10.5%` |
| `accent` | `#141414` | `rgb(20, 20, 20)` | `oklch(0.19 0.000 89.9)` | `5.0%` |
| `text` | `#E487C3` | `rgb(228, 135, 195)` | `oklch(0.74 0.135 341.7)` | `1.3%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `24.0 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
import React from 'react';
import { motion } from 'framer-motion';

export interface FigmaCreateButtonProps {
  label?: string;
  onClick?: () => void;
  className?: string;
}

export const FigmaCreateButton: React.FC<FigmaCreateButtonProps> = ({
  label = 'Figma.create',
  onClick,
  className,
}) => {
  const variants = {
    initial: { opacity: 0, scale: 0.95 },
    animate: { opacity: 1, scale: 1 },
    hover: { scale: 1.02 },
    tap: { scale: 0.98 },
  };

  return (
    <motion.button
      whileHover="hover"
      whileTap="tap"
      variants={variants}
      initial="initial"
      animate="animate"
      transition={{ type: 'spring', stiffness: 260, damping: 20 }}
      onClick={onClick}
      className={
        'flex items-center justify-center gap-2 w-[167px] h-[42px] rounded-[7px] bg-[#141414] text-[#E487C3] font-medium text-sm tracking-wide shadow-lg shadow-black/40 transition-all duration-200 ' +
        (className ?? '')
      }
      aria-label={label}
    >
      <span className="font-semibold text-base tracking-tight">Figma</span>
      <span className="text-xs text-[#77848D] opacity-70">.create</span>
    </motion.button>
  );
};

// Default export for convenience
export default FigmaCreateButton;
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class FigmaCreateButton extends StatefulWidget {
  final String label;
  final VoidCallback? onPressed;

  const FigmaCreateButton({super.key, this.label = 'Figma.create', this.onPressed});

  @override
  State<FigmaCreateButton> createState() => _FigmaCreateButtonState();
}

class _FigmaCreateButtonState extends State<FigmaCreateButton>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scale;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 240),
    );
    _scale = Tween<double>(begin: 0.95, end: 1.0).animate(
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
    return ScaleTransition(
      scale: _scale,
      child: GestureDetector(
        onTapDown: (_) => _controller.reverse(),
        onTapUp: (_) => _controller.forward(),
        onTap: widget.onPressed,
        child: AnimatedContainer(
          duration: const Duration(milliseconds: 200),
          width: 167,
          height: 42,
          decoration: BoxDecoration(
            color: const Color(0xFF141414),
         
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
