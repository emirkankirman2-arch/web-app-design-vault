---
title: "Button — DfQiYCBMdDN_Video_by_lnunesd (00:10.200)"
description: "Button UI component (recon_DfQiYCBMdDN_Video_by_lnunesdesigns_s3_01_button) with SSIM 0.9909, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_DfQiYCBMdDN_Video_by_lnunesdesigns_s3_01_button"
category: "Button"
ssim: 0.9909
quality_score: 8.72
tags: [button, ui-design, design-tokens, react, flutter]
---

# Button — DfQiYCBMdDN_Video_by_lnunesd (00:10.200)

> **Category:** [[02_Button|Button]] | **SSIM Fidelity:** `0.9909` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[01_Card|Card]], [[06_Input|Input]], [[08_Modal|Modal]]

Professional Button reverse-engineered from DfQiYCBMdDN_Video_by_lnunesdesigns at 00:10.200. Features FADE_IN_SCALE micro-interaction animation with 8.09:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#564A42` | `rgb(86, 74, 66)` | `oklch(0.42 0.021 55.7)` | `25.2%` |
| `surface` | `#AC8E84` | `rgb(172, 142, 132)` | `oklch(0.67 0.039 39.3)` | `15.0%` |
| `accent` | `#0A060C` | `rgb(10, 6, 12)` | `oklch(0.13 0.016 315.5)` | `5.0%` |
| `text` | `#FAF8F9` | `rgb(250, 248, 249)` | `oklch(0.98 0.002 345.2)` | `2.1%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `7.6 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `9.97`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react'
import { motion } from 'framer-motion'

interface GlassDockButtonProps {
  icon: React.ReactNode
  label?: string
  isActive?: boolean
  onClick?: () => void
  className?: string
}

export const GlassDockButton: React.FC<GlassDockButtonProps> = ({
  icon,
  label,
  isActive = false,
  onClick,
  className,
}) => {
  const variants = {
    initial: { opacity: 0, scale: 0.95 },
    animate: { opacity: 1, scale: 1 },
    hover: { scale: 1.05 },
    tap: { scale: 0.95 },
  }

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
        'relative flex items-center justify-center w-10 h-11 rounded-lg transition-all duration-300 ' +
        (isActive
          ? 'bg-[#AC8E84] shadow-[0_4px_12px_rgba(10,6,12,0.4)]'
          : 'bg-[#564A42]/80 backdrop-blur-md border border-white/10 shadow-[0_2px_8px_rgba(10,6,12,0.3)] hover:bg-[#564A42]') +
        ' ' +
        (className || '')
      }
    >
      <span className="text-[#FAF8F9] text-sm font-medium leading-none">{icon}</span>
      {label && (
        <span
          className={
            'absolute -bottom-6 left-1/2 -translate-x-1/2 px-2 py-1 rounded text-[10px] font-medium whitespace-nowrap opacity-0 group-hover:opacity-100 transition-opacity duration-200 ' +
            'bg-[#0A060C] text-[#FAF8F9] shadow-lg'
          }
        >
          {label}
        </span>
      
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class GlassDockButton extends StatefulWidget {
  final IconData icon;
  final String? label;
  final bool isActive;
  final VoidCallback? onTap;

  const GlassDockButton({
    Key? key,
    required this.icon,
    this.label,
    this.isActive = false,
    this.onTap,
  }) : super(key: key);

  @override
  State<GlassDockButton> createState() => _GlassDockButtonState;
}

class _GlassDockButtonState extends State<GlassDockButton>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scale;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 150),
    );
    _scale = Tween<double>(begin: 1.0, end: 0.95).animate(
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
    return GestureDetector(
      onTapDown: (_) => _controller.forward(),
      onTapUp: (_) => _controller.reverse(),
      onTapCancel: () => _controller.reverse(),
      onTap: widget.onTap,
      child: ScaleTransition(
        scale: _scale,
        child: Container(
          width: 46,
          height: 43,
          decoration: BoxDecoration(
         
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
