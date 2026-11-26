---
title: "ShaderCanvas — Dddv7P_k60o_Top_5_AI_Buildin (02:37.657)"
description: "ShaderCanvas UI component (recon_Dddv7P_k60o_Top_5_AI_Building_Blocks_Every_Engineer_Should_Know_s2) with SSIM 0.9831, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_Dddv7P_k60o_Top_5_AI_Building_Blocks_Every_Engineer_Should_Know_s2_01_shadercanvas"
category: "ShaderCanvas"
ssim: 0.9831
quality_score: 8.72
tags: [shadercanvas, ui-design, design-tokens, react, flutter]
---

# ShaderCanvas — Dddv7P_k60o_Top_5_AI_Buildin (02:37.657)

> **Category:** [[10_ShaderCanvas|ShaderCanvas]] | **SSIM Fidelity:** `0.9831` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[05_Hero|Hero]], [[03_GlassMenu|GlassMenu]], [[01_Card|Card]]

Professional ShaderCanvas reverse-engineered from Dddv7P_k60o_Top_5_AI_Building_Blocks_Every_Engineer_Should_Know at 02:37.657. Features FADE_IN_SCALE micro-interaction animation with 6.64:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#202020` | `rgb(32, 32, 32)` | `oklch(0.24 0.000 89.9)` | `64.7%` |
| `surface` | `#666666` | `rgb(102, 102, 102)` | `oklch(0.51 0.000 89.9)` | `24.3%` |
| `accent` | `#8C864A` | `rgb(140, 134, 74)` | `oklch(0.61 0.081 103.5)` | `1.1%` |
| `text` | `#A5A6A0` | `rgb(165, 166, 160)` | `oklch(0.72 0.009 114.3)` | `0.4%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `52.552 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `0.7`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
// Reverse-engineered ShaderCanvas component
// Source: Video Dddv7P_k60o_Top_5_AI_Building_Blocks_Every_Engineer_Should_Know.mp4 @ 02:37.657

import React from 'react'
import { motion } from 'framer-motion'

interface ShaderCanvasProps {
  className?: string
}

export const ShaderCanvas: React.FC<ShaderCanvasProps> = ({ className }) => {
  const framerMotionProps = {
    initial: { opacity: 0, scale: 0.95 },
    animate: { opacity: 1, scale: 1 },
    transition: { type: 'spring', stiffness: 260, damping: 20 }
  }

  return (
    <motion.div
      {...framerMotionProps}
      className={
        'relative w-full h-full rounded-2xl overflow-hidden bg-gray-900 shadow-2xl ' +
        className
      }
    >
      {/* Background layer matching #202020 */}
      <div className="absolute inset-0 bg-[#202020]" />

      {/* Surface card layer matching #666666 */}
      <div className="absolute inset-4 bg-[#666666] rounded-xl opacity-90" />

      {/* Google logo (blurred, desaturated) */}
      <div className="absolute inset-0 flex items-center justify-center p-8">
        <div className="text-9xl font-bold text-transparent bg-clip-text blur-2xl opacity-30">
          Google
        </div>
      </div>

      {/* NotebookLM text */}
      <div className="absolute bottom-16 left-1/2 -translate-x-1/2">
        <div className="flex items-center gap-4">
          <div className="w-12 h-12 bg-[#666666] rounded-full flex items-center justify-center">
            <svg
              className="w-6 h-6 text-white"
              fill="none"
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';
import 'dart:async';

class ShaderCanvas extends StatefulWidget {
  final double width;
  final double height;

  const ShaderCanvas({Key? key, this.width = 946, this.height = 404}) : super(key: key);

  @override
  _ShaderCanvasState createState() => _ShaderCanvasState();
}

class _ShaderCanvasState extends State<ShaderCanvas>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _opacityAnim;
  late Animation<double> _scaleAnim;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 5255),
    );
    _opacityAnim = Tween<double>(begin: 0.0, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOut),
    );
    _scaleAnim = Tween<double>(begin: 0.95, end: 1.0).animate(
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
          opacity: _opacityAnim.value,
          child: Transform.scale(
            scale: _scaleAnim.value,
            child: Container(

```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
