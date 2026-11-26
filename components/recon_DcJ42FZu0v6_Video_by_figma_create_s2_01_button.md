---
title: "Button — DcJ42FZu0v6_Video_by_figma_c (00:16.000)"
description: "Button UI component (recon_DcJ42FZu0v6_Video_by_figma_create_s2_01_button) with SSIM 0.9939, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_DcJ42FZu0v6_Video_by_figma.create_s2_01_button"
category: "Button"
ssim: 0.9939
quality_score: 8.72
tags: [button, ui-design, design-tokens, react, flutter]
---

# Button — DcJ42FZu0v6_Video_by_figma_c (00:16.000)

> **Category:** [[02_Button|Button]] | **SSIM Fidelity:** `0.9939` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[01_Card|Card]], [[06_Input|Input]], [[08_Modal|Modal]]

Professional Button reverse-engineered from DcJ42FZu0v6_Video_by_figma.create at 00:16.000. Features FADE_IN_SCALE micro-interaction animation with 18.11:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#000000` | `rgb(0, 0, 0)` | `oklch(0.00 0.000 0.0)` | `69.3%` |
| `surface` | `#878379` | `rgb(135, 131, 121)` | `oklch(0.61 0.016 88.7)` | `10.9%` |
| `accent` | `#151515` | `rgb(21, 21, 21)` | `oklch(0.20 0.000 89.9)` | `5.0%` |
| `text` | `#F1F2B5` | `rgb(241, 242, 181)` | `oklch(0.95 0.078 108.6)` | `2.6%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `24.0 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
import { motion } from 'framer-motion';
import React from 'react';

export interface FigmaCreateButtonProps {
  onClick?: () => void;
  className?: string;
}

export const FigmaCreateButton: React.FC<FigmaCreateButtonProps> = ({
  onClick,
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
    <motion.button
      variants={variants}
      initial="initial"
      animate="animate"
      transition={transition}
      onClick={onClick}
      className={
        'flex items-center justify-center w-[167px] h-[42px] rounded-[7px] bg-[#151515] text-[#F1F2B5] font-medium text-sm shadow-lg shadow-black/40 transition-all duration-200 hover:bg-[#2a2a2a] focus:outline-none focus:ring-2 focus:ring-[#F1F2B5]/30 active:scale-95 disabled:opacity-50 disabled:pointer-events-none ' +
        (className ?? '')
      }
    >
      Figma.create
    </motion.button>
  );
};

// Default export for convenience
export default FigmaCreateButton;
```

## 4. Flutter / Dart Implementation

```dart
// Flutter StatefulWidget
import 'package:flutter/material.dart';

class FigmaCreateButton extends StatefulWidget {
  final VoidCallback? onPressed;
  const FigmaCreateButton({Key? key, this.onPressed}) : super(key: key);

  @override
  State<FigmaCreateButton> createState() => _FigmaCreateButtonState();
}

class _FigmaCreateButtonState extends State<FigmaCreateButton>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scale;
  late Animation<double> _opacity;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 2400),
    );
    _scale = Tween<double>(begin: 0.95, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOutCubic),
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
            child: SizedBox(
              widt
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
