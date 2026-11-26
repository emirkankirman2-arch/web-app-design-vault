---
title: "Button — 7uWC417h910_I_Asked_NASA_to_ (04:02.583)"
description: "Button UI component (recon_7uWC417h910_I_Asked_NASA_to_Use_My_App_Redesign_s2_02_button) with SSIM 0.9923, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_7uWC417h910_I_Asked_NASA_to_Use_My_App_Redesign_s2_02_button"
category: "Button"
ssim: 0.9923
quality_score: 8.72
tags: [button, ui-design, design-tokens, react, flutter]
---

# Button — 7uWC417h910_I_Asked_NASA_to_ (04:02.583)

> **Category:** [[02_Button|Button]] | **SSIM Fidelity:** `0.9923` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[01_Card|Card]], [[06_Input|Input]], [[08_Modal|Modal]]

Professional Button reverse-engineered from 7uWC417h910_I_Asked_NASA_to_Use_My_App_Redesign at 04:02.583. Features FADE_IN_SCALE micro-interaction animation with 13.83:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#040404` | `rgb(4, 4, 4)` | `oklch(0.11 0.000 89.9)` | `44.4%` |
| `surface` | `#757C83` | `rgb(117, 124, 131)` | `oklch(0.58 0.014 248.1)` | `8.8%` |
| `accent` | `#040404` | `rgb(4, 4, 4)` | `oklch(0.11 0.000 89.9)` | `5.0%` |
| `text` | `#D4D4D4` | `rgb(212, 212, 212)` | `oklch(0.87 0.000 89.9)` | `0.6%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `50.883 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `1.05`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
import React from 'react';
import { motion } from 'framer-motion';
import MusicNoteIcon from 'lucide-react/MusicNote2';

export interface MusicButtonProps {
  onClick?: () => void;
  className?: string;
}

export const MusicButton: React.FC<MusicButtonProps> = ({ onClick, className }) => {
  const variants = {
    initial: { opacity: 0, scale: 0.95 },
    animate: { opacity: 1, scale: 1 },
    hover: { scale: 1.05 },
    tap: { scale: 0.95 }
  };

  return (
    <motion.button
      asChild={false}
      type="button"
      onClick={onClick}
      whileHover="hover"
      whileTap="tap"
      variants={variants}
      initial="initial"
      animate="animate"
      transition={{ type: 'spring', stiffness: 260, damping: 20 }}
      className={
        'relative flex items-center justify-center w-[110px] h-[69px] rounded-[12px] bg-[#040404] text-[#D4D4D4] shadow-lg transition-all duration-200 ' +
        (className ?? '')
      }
      aria-label="Music"
    >
      <MusicNoteIcon className="w-6 h-6" aria-hidden="true" />
    </motion.button>
  );
};

// Default export for convenience
export default MusicButton;
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class MusicButton extends StatefulWidget {
  final VoidCallback? onPressed;
  const MusicButton({Key? key, this.onPressed}) : super(key: key);

  @override
  State<MusicButton> createState() => _MusicButtonState();
}

class _MusicButtonState extends State<MusicButton>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scale;
  late Animation<double> _opacity;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 500),
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
        return Transform.scale(
          scale: _scale.value,
          child: Opacity(
            opacity: _opacity.value,
            child: GestureDetector(
              onTapDown: (_) => _controller.reverse(),
              onTapUp: (
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
