---
title: "Button — 7uWC417h910_I_Asked_NASA_to_ (04:02.583)"
description: "Button UI component (recon_7uWC417h910_I_Asked_NASA_to_Use_My_App_Redesign_s2_01_button) with SSIM 0.9919, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_7uWC417h910_I_Asked_NASA_to_Use_My_App_Redesign_s2_01_button"
category: "Button"
ssim: 0.9919
quality_score: 8.72
tags: [button, ui-design, design-tokens, react, flutter]
---

# Button — 7uWC417h910_I_Asked_NASA_to_ (04:02.583)

> **Category:** [[02_Button|Button]] | **SSIM Fidelity:** `0.9919` | **Quality Score:** `8.72 / 10`  
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
// runnable React TypeScript code
import React from 'react';
import { motion } from 'framer-motion';
import { Search } from 'lucide-react';

export interface SearchButtonProps {
  onClick?: () => void;
  className?: string;
  size?: 'sm' | 'md' | 'lg';
}

export const SearchButton: React.FC<SearchButtonProps> = ({
  onClick,
  className,
  size = 'md',
}) => {
  const sizeConfig = {
    sm: { w: 10, h: 10, icon: 16 },
    md: { w: 12, h: 12, icon: 20 },
    lg: { w: 14, h: 14, icon: 24 },
  };

  const { w, h, icon } = sizeConfig[size];

  return (
    <motion.button
      onClick={onClick}
      className={
        'relative flex items-center justify-center overflow-hidden group ' +
        'bg-[#040404] text-[#D4D4D4] ' +
        `w-${w} h-${h} rounded-[12px] ` +
        'shadow-[0_4px_6px_-1px_rgba(0,0,0,0.5),0_2px_4px_-1px_rgba(0,0,0,0.3)] ' +
        'transition-all duration-200 ease-in-out ' +
        'hover:bg-[#757C83] hover:text-[#040404] ' +
        'focus:outline-none focus:ring-2 focus:ring-[#757C83] focus:ring-offset-2 focus:ring-offset-[#040404] ' +
        'active:scale-95 disabled:opacity-50 disabled:pointer-events-none ' +
        (className || '')
      }
      aria-label="Search"
      initial={{ opacity: 0, scale: 0.95 }}
      animate={{ opacity: 1, scale: 1 }}
      transition={{ type: 'spring', stiffness: 260, damping: 20 }}
    >
      <Search size={icon} strokeWidth={2} className="fill-current" />
      <span className="absolute inset-0 bg-white/10 opacity-0 group-hover:opacity-100 transition-opacity duration-200" />
    </motion.button>
  );
};

ex
```

## 4. Flutter / Dart Implementation

```dart
// runnable Flutter StatefulWidget
import 'package:flutter/material.dart';

class SearchButton extends StatefulWidget {
  final VoidCallback? onPressed;
  final double size;
  final Color backgroundColor;
  final Color iconColor;
  final Color hoverColor;
  final Color hoverIconColor;

  const SearchButton({
    Key? key,
    this.onPressed,
    this.size = 48.0,
    this.backgroundColor = const Color(0xFF040404),
    this.iconColor = const Color(0xFFD4D4D4),
    this.hoverColor = const Color(0xFF757C83),
    this.hoverIconColor = const Color(0xFF040404),
  }) : super(key: key);

  @override
  State<SearchButton> createState() => _SearchButtonState();
}

class _SearchButtonState extends State<SearchButton>
    with SingleTickerProviderStateMixin {
  bool _isHovered = false;
  late AnimationController _controller;
  late Animation<double> _scaleAnimation;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 200),
    );
    _scaleAnimation = Tween<double>(begin: 1.0, end: 0.95).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeInOut),
    );
  }

  @override
  void dispose() {
    _controller.dispose();
    super.dispose();
  }

  @override
  Widget build(BuildContext context) {
    return MouseRegion(
      onEnter: (_) => setState(() => _isHovered = tr
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
