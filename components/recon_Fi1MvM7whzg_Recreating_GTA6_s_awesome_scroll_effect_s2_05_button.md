---
title: "Button — Fi1MvM7whzg_Recreating_GTA6_ (13:44.100)"
description: "Button UI component (recon_Fi1MvM7whzg_Recreating_GTA6_s_awesome_scroll_effect_s2_05_button) with SSIM 0.9906, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_Fi1MvM7whzg_Recreating_GTA6_s_awesome_scroll_effect_s2_05_button"
category: "Button"
ssim: 0.9906
quality_score: 8.72
tags: [button, ui-design, design-tokens, react, flutter]
---

# Button — Fi1MvM7whzg_Recreating_GTA6_ (13:44.100)

> **Category:** [[02_Button|Button]] | **SSIM Fidelity:** `0.9906` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[01_Card|Card]], [[06_Input|Input]], [[08_Modal|Modal]]

Professional Button reverse-engineered from Fi1MvM7whzg_Recreating_GTA6_s_awesome_scroll_effect at 13:44.100. Features FADE_IN_SCALE micro-interaction animation with 5.8:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#121217` | `rgb(18, 18, 23)` | `oklch(0.18 0.010 285.4)` | `38.9%` |
| `surface` | `#785765` | `rgb(120, 87, 101)` | `oklch(0.50 0.048 351.8)` | `11.4%` |
| `accent` | `#7E5655` | `rgb(126, 86, 85)` | `oklch(0.50 0.054 20.8)` | `5.0%` |
| `text` | `#3394E6` | `rgb(51, 148, 230)` | `oklch(0.65 0.151 248.4)` | `4.0%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `164.0 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `0.48`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react';
import { motion } from 'framer-motion';

type GlassMenuButtonProps = {
  icon: React.ReactNode;
  label: string;
  isActive?: boolean;
  onClick?: () => void;
};

export const GlassMenuButton: React.FC<GlassMenuButtonProps> = ({
  icon,
  label,
  isActive = false,
  onClick,
}) => {
  const variants = {
    initial: { opacity: 0, scale: 0.95 },
    animate: { opacity: 1, scale: 1 },
    hover: { scale: 1.05 },
    tap: { scale: 0.95 },
  };

  return (
    <motion.button
      aria-label={label}
      onClick={onClick}
      whileHover="hover"
      whileTap="tap"
      variants={variants}
      initial="initial"
      animate="animate"
      transition={{ type: 'spring', stiffness: 260, damping: 20 }}
      className={
        'relative flex flex-col items-center justify-center w-28 h-18 rounded-2xl transition-all duration-200 ' +
        (isActive
          ? 'bg-[#785765]/80 backdrop-blur-md text-[#3394E6] shadow-[0_0_20px_rgba(126,86,85,0.4)]'
          : 'bg-[#121217]/60 backdrop-blur-sm text-[#785765]/60 hover:bg-[#785765]/40 hover:text-[#3394E6] border border-transparent hover:border-[#7E5655]/30')
      }
    >
      <div className="absolute inset-0 rounded-2xl opacity-0 transition-opacity duration-200 " +
            (isActive ? 'bg-[#7E5655]/20' : '') +
            '" />
      <span className="relative z-10 mb-1 text-xs font-medium tracking-wide">
        {icon}
      </span>
      <span className="relative z-10 text-[10px] font-semibold uppercase tracking-widest opacity-80">
        {label}
      </span>
    </motion.button>
  );
};

e
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class GlassMenuButton extends StatefulWidget {
  final IconData icon;
  final String label;
  final bool isActive;
  final VoidCallback? onTap;

  const GlassMenuButton({
    super.key,
    required this.icon,
    required this.label,
    this.isActive = false,
    this.onTap,
  });

  @override
  State<GlassMenuButton> createState() => _GlassMenuButtonState();
}

class _GlassMenuButtonState extends State<GlassMenuButton>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scale;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 164),
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
      child: AnimatedContainer(
        duration: const Duration(milliseconds: 200),
        width: 109,
        height: 69,
        decoration: BoxDecoration(
          color: widget.isActive
              ? const Color(0xFF785765).withOpacity(0.8)
              : const Color(0xFF121217).withOp
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
