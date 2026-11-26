---
title: "ShaderCanvas — mMEgcEqc46g_I_Made_Reddit_Lo (03:46.933)"
description: "ShaderCanvas UI component (recon_mMEgcEqc46g_I_Made_Reddit_Look_Retro_s3_00_shadercanvas) with SSIM 0.9806, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_mMEgcEqc46g_I_Made_Reddit_Look_Retro_s3_00_shadercanvas"
category: "ShaderCanvas"
ssim: 0.9806
quality_score: 8.72
tags: [shadercanvas, ui-design, design-tokens, react, flutter]
---

# ShaderCanvas — mMEgcEqc46g_I_Made_Reddit_Lo (03:46.933)

> **Category:** [[10_ShaderCanvas|ShaderCanvas]] | **SSIM Fidelity:** `0.9806` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[05_Hero|Hero]], [[03_GlassMenu|GlassMenu]], [[01_Card|Card]]

Professional ShaderCanvas reverse-engineered from mMEgcEqc46g_I_Made_Reddit_Look_Retro at 03:46.933. Features FADE_IN_SCALE micro-interaction animation with 16.23:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#000000` | `rgb(0, 0, 0)` | `oklch(0.00 0.000 0.0)` | `71.7%` |
| `surface` | `#A19F9A` | `rgb(161, 159, 154)` | `oklch(0.70 0.008 88.7)` | `1.8%` |
| `accent` | `#C6C2BA` | `rgb(198, 194, 186)` | `oklch(0.82 0.012 84.6)` | `5.7%` |
| `text` | `#E5E2DB` | `rgb(229, 226, 219)` | `oklch(0.91 0.010 87.5)` | `10.1%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `23.767 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.84`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react';
import { motion } from 'framer-motion';

interface ShaderCanvasProps {
  width?: number;
  height?: number;
  className?: string;
}

export const ShaderCanvas: React.FC<ShaderCanvasProps> = ({
  width = 906,
  height = 381,
  className = '',
}) => {
  return (
    <motion.div
      initial={{ opacity: 0, scale: 0.95 }}
      animate={{ opacity: 1, scale: 1 }}
      transition={{ type: 'spring', stiffness: 260, damping: 20 }}
      className={
        'relative w-full h-full bg-black overflow-hidden rounded-none ' + className
      }
      style={{ width, height }}
    >
      {/* Canvas placeholder for shader rendering */}
      <canvas
        className='absolute inset-0 w-full h-full block'
        width={width}
        height={height}
      />
      {/* Surface overlay matching design tokens */}
      <div className='absolute inset-0 bg-[#A19F9A]/10 backdrop-blur-sm pointer-events-none' />
      {/* Accent glow */}
      <div className='absolute inset-0 bg-[#C6C2BA]/5 mix-blend-overlay pointer-events-none' />
    </motion.div>
  );
};

// Demo wrapper showing usage with text overlay from screenshot
interface ShaderCanvasDemoProps {}

export const ShaderCanvasDemo: React.FC<ShaderCanvasDemoProps> = () => {
  return (
    <div className='fixed inset-0 bg-black flex items-center justify-center text-[#E5E2DB] font-mono'>
      <ShaderCanvas width={906} height={381} />
      <div className='absolute inset-0 p-8 flex flex-col justify-between pointer-events-none'>
        <div className='flex items-center gap-4'>
          <div className='w-10 h-10 ro
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class ShaderCanvas extends StatefulWidget {
  final double width;
  final double height;
  const ShaderCanvas({super.key, this.width = 906, this.height = 381});

  @override
  State<ShaderCanvas> createState() => _ShaderCanvasState();
}

class _ShaderCanvasState extends State<ShaderCanvas>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _opacity;
  late Animation<double> _scale;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 2377),
    );
    _opacity = Tween<double>(begin: 0.0, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOut),
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
    return AnimatedBuilder(
      animation: _controller,
      builder: (context, child) {
        return Opacity(
          opacity: _opacity.value,
          child: Transform.scale(
            scale: _scale.value,
            child: SizedBox(
              width: widget.width,
              height: widget
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
