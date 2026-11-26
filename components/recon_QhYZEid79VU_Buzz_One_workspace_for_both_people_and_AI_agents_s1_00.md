---
title: "LockScreen — QhYZEid79VU_Buzz_One_workspa (00:00.000)"
description: "LockScreen UI component (recon_QhYZEid79VU_Buzz_One_workspace_for_both_people_and_AI_agents_s1_00) with SSIM 0.9927, OKLCH design tokens, SLIDE_UP motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_QhYZEid79VU_Buzz_-_One_workspace_for_both_people_and_AI_agents_s1_00_lockscreen"
category: "LockScreen"
ssim: 0.9927
quality_score: 8.72
tags: [lockscreen, ui-design, design-tokens, react, flutter]
---

# LockScreen — QhYZEid79VU_Buzz_One_workspa (00:00.000)

> **Category:** [[07_LockScreen|LockScreen]] | **SSIM Fidelity:** `0.9927` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[03_GlassMenu|GlassMenu]], [[09_SplashAuth|SplashAuth]], [[01_Card|Card]]

Professional LockScreen reverse-engineered from QhYZEid79VU_Buzz_-_One_workspace_for_both_people_and_AI_agents at 00:00.000. Features SLIDE_UP micro-interaction animation with 17.08:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#F5F5F8` | `rgb(245, 245, 248)` | `oklch(0.97 0.004 286.3)` | `34.0%` |
| `surface` | `#CAD2C9` | `rgb(202, 210, 201)` | `oklch(0.86 0.015 142.2)` | `6.3%` |
| `accent` | `#716D5C` | `rgb(113, 109, 92)` | `oklch(0.53 0.026 96.2)` | `5.0%` |
| `text` | `#151216` | `rgb(21, 18, 22)` | `oklch(0.19 0.009 317.7)` | `21.0%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `SLIDE_UP`
- **Measured Duration:** `22.96 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `6.46`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS
// LockScreen component reconstructed from video evidence
// Style: AUTO | Motion: SLIDE_UP | Duration: 22.96s

import React, { useEffect } from 'react';
import { motion } from 'framer-motion';

interface LockScreenProps {
  className?: string;
}

const LockScreen: React.FC<LockScreenProps> = ({ className }) => {
  useEffect(() => {
    // Animation is handled by Framer Motion
  }, []);

  return (
    <motion.div
      initial={{ opacity: 0, y: 5.468011856079102 }}
      animate={{ opacity: 1, y: 0 }}
      transition={
        duration: 22.96,
        ease: [0.16, 1, 0.3, 1]
      }
      className={
        'relative w-[284px] h-[453px] rounded-[28px] bg-[#F5F5F8] overflow-hidden shadow-none ' +
        (className || '')
      }
    >
      {/* Background surface layer */}
      <div className="absolute inset-0 bg-[#CAD2C9] opacity-60" />

      {/* Content placeholder - lock screen area */}
      <div className="absolute inset-4 flex flex-col items-center justify-center text-[#151216]">
        <div className="w-12 h-12 rounded-full bg-[#716D5C] mb-4 flex items-center justify-center">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            className="w-6 h-6 text-white"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
          >
            <path
              strokeLinecap="round"
              strokeLinejoin="round"
              strokeWidth={2}
              d="M12 15v2m-6 4h12a2 2 0 002-2v-6a2 2 0 00-2-2H6a2 2 0 00-2 2v6a2 2 0 002 2zm10-10V7a4 4 0 00-8 0v4h8z"
            
```

## 4. Flutter / Dart Implementation

```dart
// Flutter StatefulWidget
// LockScreen component reconstructed from video evidence
// Style: AUTO | Motion: SLIDE_UP | Duration: 22.96s

import 'package:flutter/material.dart';

class LockScreen extends StatefulWidget {
  const LockScreen({Key? key}) : super(key: key);

  @override
  _LockScreenState createState() => _LockScreenState();
}

class _LockScreenState extends State<LockScreen>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _opacityAnimation;
  late Animation<Offset> _slideAnimation;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 22960),
    );
    _opacityAnimation = Tween<double>(begin: 0.0, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeInOut),
    );
    _slideAnimation = Tween<Offset>(begin: const Offset(0, 0.05468), end: Offset.zero).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeInOut),
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
    return FadeTransition(
      opacity: _opacityAnimation,
      child: SlideTransition(
        position: _slideAnimation,
        child: Container(
          width: 284,
       
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
