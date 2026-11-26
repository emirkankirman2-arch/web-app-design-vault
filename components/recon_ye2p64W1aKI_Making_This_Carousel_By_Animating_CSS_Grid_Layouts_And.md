---
title: "Button — ye2p64W1aKI_Making_This_Caro (08:35.100)"
description: "Button UI component (recon_ye2p64W1aKI_Making_This_Carousel_By_Animating_CSS_Grid_Layouts_And) with SSIM 0.9914, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_ye2p64W1aKI_Making_This_Carousel_By_Animating_CSS_Grid_Layouts_And_Using_s3_14_button"
category: "Button"
ssim: 0.9914
quality_score: 8.72
tags: [button, ui-design, design-tokens, react, flutter]
---

# Button — ye2p64W1aKI_Making_This_Caro (08:35.100)

> **Category:** [[02_Button|Button]] | **SSIM Fidelity:** `0.9914` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[01_Card|Card]], [[06_Input|Input]], [[08_Modal|Modal]]

Professional Button reverse-engineered from ye2p64W1aKI_Making_This_Carousel_By_Animating_CSS_Grid_Layouts_And_Using at 08:35.100. Features FADE_IN_SCALE micro-interaction animation with 7.58:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#17161D` | `rgb(23, 22, 29)` | `oklch(0.20 0.014 291.7)` | `84.5%` |
| `surface` | `#35373F` | `rgb(53, 55, 63)` | `oklch(0.34 0.014 274.5)` | `2.6%` |
| `accent` | `#17161E` | `rgb(23, 22, 30)` | `oklch(0.21 0.016 290.7)` | `5.0%` |
| `text` | `#C1A294` | `rgb(193, 162, 148)` | `oklch(0.74 0.042 45.7)` | `0.3%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `76.5 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `0.79`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react'
import { motion } from 'framer-motion'

interface GlassMenuButtonProps {
  icon: React.ReactNode
  label?: string
  isActive?: boolean
  onClick?: () => void
}

export const GlassMenuButton: React.FC<GlassMenuButtonProps> = ({
  icon,
  label,
  isActive = false,
  onClick,
}) => {
  return (
    <motion.button
      aria-label={label || 'menu button'}
      onClick={onClick}
      className={
        'relative flex flex-col items-center justify-center w-[85px] h-[53px] rounded-[9px] transition-all duration-200 ease-out'
      }
      whileHover={{ scale: 1.05 }}
      whileTap={{ scale: 0.95 }}
      style={
        isActive
          ? {
              backgroundColor: '#35373F',
              boxShadow: '0 4px 12px rgba(0, 0, 0, 0.5)',
            }
          : {
              backgroundColor: 'transparent',
              boxShadow: 'none',
            }
      }
    >
      <div className="relative z-10 text-center">
        <span className="text-[14px] font-medium text-[#C1A294] opacity-80 transition-opacity duration-200">
          {icon}
        </span>
        {label && (
          <span className="mt-[2px] text-[10px] font-medium text-[#C1A294] opacity-60 transition-opacity duration-200">
            {label}
          </span>
        )}
      </div>
      {/* Accent glow ring for active state */}
      {isActive && (
        <motion.div
          className="absolute inset-0 rounded-[9px] border border-[#17161E] opacity-0"
          animate={{ opacity: 1 }}
          transition={{ duration: 0.2 }}
        />
      )}
    </motion.button>
  )

```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class GlassMenuButton extends StatefulWidget {
  final IconData icon;
  final String? label;
  final bool isActive;
  final VoidCallback? onTap;

  const GlassMenuButton({
    Key? key,
    required this.icon,
    this.label,
    this.isActive = false,
    this.onTap,
  }) : super(key: key);

  @override
  State<GlassMenuButton> createState() => _GlassMenuButtonState;
}

class _GlassMenuButtonState extends State<GlassMenuButton>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scaleAnimation;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      duration: const Duration(milliseconds: 200),
      vsync: this,
    );
    _scaleAnimation = Tween<double>(begin: 1.0, end: 0.95).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOut),
    );
  }

  @override
  void dispose() {
    _controller.dispose();
    super.dispose();
  }

  void _onTapDown(TapDownDetails details) => _controller.forward();
  void _onTapUp(TapUpDetails details) => _controller.reverse();

  @override
  Widget build(BuildContext context) {
    return GestureDetector(
      onTapDown: _onTapDown,
      onTapUp: _onTapUp,
      onTapCancel: () => _controller.reverse(),
      onTap: widget.onTap,
      child: AnimatedScale(
        scale: _scaleAnimatio
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
