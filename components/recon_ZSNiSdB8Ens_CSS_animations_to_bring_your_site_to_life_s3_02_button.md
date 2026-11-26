---
title: "Button — ZSNiSdB8Ens_CSS_animations_t (09:59.400)"
description: "Button UI component (recon_ZSNiSdB8Ens_CSS_animations_to_bring_your_site_to_life_s3_02_button) with SSIM 0.9929, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_ZSNiSdB8Ens_CSS_animations_to_bring_your_site_to_life_s3_02_button"
category: "Button"
ssim: 0.9929
quality_score: 8.72
tags: [button, ui-design, design-tokens, react, flutter]
---

# Button — ZSNiSdB8Ens_CSS_animations_t (09:59.400)

> **Category:** [[02_Button|Button]] | **SSIM Fidelity:** `0.9929` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[01_Card|Card]], [[06_Input|Input]], [[08_Modal|Modal]]

Professional Button reverse-engineered from ZSNiSdB8Ens_CSS_animations_to_bring_your_site_to_life at 09:59.400. Features FADE_IN_SCALE micro-interaction animation with 12.86:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#131418` | `rgb(19, 20, 24)` | `oklch(0.19 0.008 274.5)` | `44.6%` |
| `surface` | `#38383E` | `rgb(56, 56, 62)` | `oklch(0.34 0.010 285.8)` | `8.6%` |
| `accent` | `#111216` | `rgb(17, 18, 22)` | `oklch(0.18 0.008 274.4)` | `5.0%` |
| `text` | `#DCD6DA` | `rgb(220, 214, 218)` | `oklch(0.88 0.008 337.5)` | `1.6%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `167.733 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.01`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
// Reconstructed from video evidence: ZSNiSdB8Ens_CSS_animations_to_bring_your_site_to_life.mp4 @ 09:59.400
import React from 'react'
import { motion, AnimatePresence } from 'framer-motion'

interface GlassMenuDockProps {
  className?: string
}

const navItems = [
  { id: 'home', label: 'Home', icon: 'ð ' },
  { id: 'likes', label: 'Likes', icon: 'â¤ï¸' },
  { id: 'create', label: 'Create', icon: 'â¨' },
  { id: 'profile', label: 'Profile', icon: 'ð¤' },
  { id: 'alerts', label: 'Alerts', icon: 'ð' },
]

export const GlassMenuDock: React.FC<GlassMenuDockProps> = ({ className }) => {
  const [activeId, setActiveId] = React.useState<string>('home')

  return (
    <nav
      className={
        'fixed bottom-6 left-1/2 -translate-x-1/2 z-50 ' +
        'bg-[#131418]/80 backdrop-blur-xl border border-white/10 rounded-full px-4 py-2 shadow-2xl ' +
        'flex items-center gap-3 ' +
        className
      }
      aria-label="Main navigation"
    >
      <AnimatePresence mode="wait">
        {navItems.map((item) => (
          <motion.button
            key={item.id}
            initial={{ opacity: 0, scale: 0.95 }}
            animate={{ opacity: 1, scale: 1 }}
            exit={{ opacity: 0, scale: 0.95 }}
            transition={{ type: 'spring', stiffness: 260, damping: 20 }}
            whileHover={{ scale: 1.1 }}
            whileTap={{ scale: 0.9 }}
            onClick={() => setActiveId(item.id)}
            className={
              'relative flex flex-col items-center justify-center w-16 h-6 rounded-none tr
```

## 4. Flutter / Dart Implementation

```dart
// Flutter StatefulWidget
// Reconstructed from video evidence: ZSNiSdB8Ens_CSS_animations_to_bring_your_site_to_life.mp4 @ 09:59.400
import 'package:flutter/material.dart';

class GlassMenuDock extends StatefulWidget {
  const GlassMenuDock({super.key});

  @override
  State<GlassMenuDock> createState() => _GlassMenuDockState();
}

class _GlassMenuDockState extends State<GlassMenuDock> {
  String _activeId = 'home';

  final List<Map<String, String>> _items = [
    {'id': 'home', 'label': 'Home', 'icon': 'ð '},
    {'id': 'likes', 'label': 'Likes', 'icon': 'â¤ï¸'},
    {'id': 'create', 'label': 'Create', 'icon': 'â¨'},
    {'id': 'profile', 'label': 'Profile', 'icon': 'ð¤'},
    {'id': 'alerts', 'label': 'Alerts', 'icon': 'ð'},
  ];

  @override
  Widget build(BuildContext context) {
    return Positioned(
      bottom: 24,
      left: 0,
      right: 0,
      child: Center(
        child: ClipRRect(
          borderRadius: BorderRadius.circular(999),
          child: BackdropFilter(
            filter: ImageFilter.blur(sigmaX: 12, sigmaY: 12),
            child: Container(
              width: 320,
              height: 40,
              decoration: BoxDecoration(
                color: const Color(0xFF131418).withOpacity(0.8),
                border: Border.all(color: Colors.white.withOpacity(0.1)),
                borderRadius: BorderRadius.circular(999),
        
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
