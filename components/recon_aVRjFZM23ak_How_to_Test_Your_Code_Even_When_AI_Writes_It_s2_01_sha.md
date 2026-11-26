---
title: "ShaderCanvas — aVRjFZM23ak_How_to_Test_Your (02:05.125)"
description: "ShaderCanvas UI component (recon_aVRjFZM23ak_How_to_Test_Your_Code_Even_When_AI_Writes_It_s2_01_sha) with SSIM 0.9909, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_aVRjFZM23ak_How_to_Test_Your_Code_Even_When_AI_Writes_It_s2_01_shadercanvas"
category: "ShaderCanvas"
ssim: 0.9909
quality_score: 8.72
tags: [shadercanvas, ui-design, design-tokens, react, flutter]
---

# ShaderCanvas — aVRjFZM23ak_How_to_Test_Your (02:05.125)

> **Category:** [[10_ShaderCanvas|ShaderCanvas]] | **SSIM Fidelity:** `0.9909` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[05_Hero|Hero]], [[03_GlassMenu|GlassMenu]], [[01_Card|Card]]

Professional ShaderCanvas reverse-engineered from aVRjFZM23ak_How_to_Test_Your_Code_Even_When_AI_Writes_It at 02:05.125. Features FADE_IN_SCALE micro-interaction animation with 13.54:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#202020` | `rgb(32, 32, 32)` | `oklch(0.24 0.000 89.9)` | `58.0%` |
| `surface` | `#6B6B6B` | `rgb(107, 107, 107)` | `oklch(0.53 0.000 89.9)` | `1.3%` |
| `accent` | `#79D234` | `rgb(121, 210, 52)` | `oklch(0.78 0.205 134.9)` | `0.5%` |
| `text` | `#EAEAEA` | `rgb(234, 234, 234)` | `oklch(0.94 0.000 89.9)` | `30.3%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `43.794 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.25`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react'
import { motion } from 'framer-motion'

interface ShaderCanvasProps {
  width?: number
  height?: number
}

export const ShaderCanvas: React.FC<ShaderCanvasProps> = ({ width = 988, height = 508 }) => {
  return (
    <div
      className="relative w-full h-full bg-[#202020] text-[#EAEAEA] overflow-hidden"
      style={{ width, height }}
    >
      {/* Browser chrome header */}
      <div className="absolute top-0 left-0 right-0 h-16 bg-gray-300 flex items-center px-6 gap-4 border-b border-gray-400 z-10">
        <div className="flex gap-2">
          <div className="w-3 h-3 rounded-full bg-red-500" />
          <div className="w-3 h-3 rounded-full bg-yellow-500" />
          <div className="w-3 h-3 rounded-full bg-green-500" />
        </div>
        <div className="flex-1 bg-gray-200 rounded-full px-4 py-1.5 text-gray-900 text-sm font-medium shadow-inner">
          shop.example.
        </div>
      </div>

      {/* Canvas content area */}
      <motion.div
        initial={{ opacity: 0, scale: 0.95 }}
        animate={{ opacity: 1, scale: 1 }}
        transition={{ type: 'spring', stiffness: 260, damping: 20 }}
        className="absolute inset-0 flex flex-col items-center justify-center p-8"
      >
        {/* T-shirt SVG icon */}
        <svg
          className="w-32 h-32 text-[#79D234] drop-shadow-[0_0_12px_rgba(121,210,52,0.6)]"
          viewBox="0 0 24 24"
          fill="none"
          stroke="currentColor"
          strokeWidth="2"
          strokeLinecap="round"
          strokeLinejoin="round"
        >
          <path d="M4 10v4h
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class ShaderCanvas extends StatefulWidget {
  final double width;
  final double height;

  const ShaderCanvas({super.key, this.width = 988, this.height = 508});

  @override
  State<ShaderCanvas> createState() => _ShaderCanvasState();
}

class _ShaderCanvasState extends State<ShaderCanvas> with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scaleAnim;
  late Animation<double> _opacityAnim;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 600),
    );
    _scaleAnim = Tween<double>(begin: 0.95, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOutBack),
    );
    _opacityAnim = Tween<double>(begin: 0.0, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeIn),
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
    return SizedBox(
      width: widget.width,
      height: widget.height,
      child: Stack(
        children: [
          // Browser chrome header
          Positioned(
            top: 0,
            left: 0,
            right: 0,
            child: Container(
              height: 64,
  
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
