---
title: "Button — 8soK_4_USDo_Making_a_Realist (11:31.380)"
description: "Button UI component (recon_8soK_4_USDo_Making_a_Realistic_Folding_Animation_With_Framer_Motio) with SSIM 0.991, OKLCH design tokens, SLIDE_UP motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_8soK-4_USDo_Making_a_Realistic_Folding_Animation_With_Framer_Motion_s2_05_button"
category: "Button"
ssim: 0.991
quality_score: 8.72
tags: [button, ui-design, design-tokens, react, flutter]
---

# Button — 8soK_4_USDo_Making_a_Realist (11:31.380)

> **Category:** [[02_Button|Button]] | **SSIM Fidelity:** `0.991` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[01_Card|Card]], [[06_Input|Input]], [[08_Modal|Modal]]

Professional Button reverse-engineered from 8soK-4_USDo_Making_a_Realistic_Folding_Animation_With_Framer_Motion at 11:31.380. Features SLIDE_UP micro-interaction animation with 13.66:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#1A1F2A` | `rgb(26, 31, 42)` | `oklch(0.24 0.022 265.7)` | `83.3%` |
| `surface` | `#59403D` | `rgb(89, 64, 61)` | `oklch(0.40 0.036 26.5)` | `2.6%` |
| `accent` | `#171B26` | `rgb(23, 27, 38)` | `oklch(0.22 0.022 269.0)` | `5.0%` |
| `text` | `#F8E7D6` | `rgb(248, 231, 214)` | `oklch(0.94 0.029 67.5)` | `0.4%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `SLIDE_UP`
- **Measured Duration:** `126.92 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `0.4`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react';
import { motion } from 'framer-motion';

interface AutoButtonProps {
  label?: string;
  onClick?: () => void;
  className?: string;
}

export const AutoButton: React.FC<AutoButtonProps> = ({
  label = '3',
  onClick,
  className,
}) => {
  return (
    <motion.button
      className={
        'inline-flex items-center justify-center w-20 h-7 rounded-none bg-[#171B26] text-[#F8E7D6] text-sm font-medium shadow-sm transition-colors duration-200 hover:bg-[#242A38] focus:outline-none focus:ring-2 focus:ring-[#59403D] focus:ring-offset-2 focus:ring-offset-[#1A1F2A] disabled:opacity-50 disabled:pointer-events-none ' +
        (className || '')
      }
      onClick={onClick}
      initial={{ opacity: 0, y: 6.759289741516113 }}
      animate={{ opacity: 1, y: 0 }}
      transition={{ duration: 126.92, ease: [0.16, 1, 0.3, 1] }}
      aria-label={label}
    >
      {label}
    </motion.button>
  );
};

// Usage example:
// <AutoButton label="3" onClick={() => console.log('clicked')} />
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class AutoButton extends StatefulWidget {
  final String label;
  final VoidCallback? onPressed;

  const AutoButton({Key? key, this.label = '3', this.onPressed}) : super(key: key);

  @override
  State<AutoButton> createState() => _AutoButtonState();
}

class _AutoButtonState extends State<AutoButton> with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<Offset> _offsetAnimation;
  late Animation<double> _opacityAnimation;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 126920),
    );
    _offsetAnimation = Tween<Offset>(
      begin: const Offset(0, 6.759289741516113),
      end: Offset.zero,
    ).animate(CurvedAnimation(parent: _controller, curve: Curves.easeInOutCubic));
    _opacityAnimation = Tween<double>(begin: 0.0, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeInOutCubic),
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
    return SlideTransition(
      position: _offsetAnimation,
      child: FadeTransition(
        opacity: _opacityAnimation,
        child: Material(
          color: Colors.transparent,
          chil
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
