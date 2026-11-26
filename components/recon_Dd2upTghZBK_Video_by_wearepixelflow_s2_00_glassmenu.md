---
title: "GlassMenu — Dd2upTghZBK_Video_by_wearepi (00:04.000)"
description: "GlassMenu UI component (recon_Dd2upTghZBK_Video_by_wearepixelflow_s2_00_glassmenu) with SSIM 0.9899, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_Dd2upTghZBK_Video_by_wearepixelflow_s2_00_glassmenu"
category: "GlassMenu"
ssim: 0.9899
quality_score: 8.72
tags: [glassmenu, ui-design, design-tokens, react, flutter]
---

# GlassMenu — Dd2upTghZBK_Video_by_wearepi (00:04.000)

> **Category:** [[03_GlassMenu|GlassMenu]] | **SSIM Fidelity:** `0.9899` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[04_Navbar|Navbar]], [[01_Card|Card]], [[10_ShaderCanvas|ShaderCanvas]]

Professional GlassMenu reverse-engineered from Dd2upTghZBK_Video_by_wearepixelflow at 00:04.000. Features FADE_IN_SCALE micro-interaction animation with 17.94:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#000000` | `rgb(0, 0, 0)` | `oklch(0.00 0.000 0.0)` | `50.8%` |
| `surface` | `#323233` | `rgb(50, 50, 51)` | `oklch(0.32 0.002 286.3)` | `0.4%` |
| `accent` | `#B3B3B4` | `rgb(179, 179, 180)` | `oklch(0.77 0.001 286.4)` | `0.3%` |
| `text` | `#EDEDED` | `rgb(237, 237, 237)` | `oklch(0.95 0.000 89.9)` | `0.1%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `6.0 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
import React from 'react'
import { motion } from 'framer-motion'
import { Home, Heart, PlusCircle, User, Bell } from 'lucide-react'

interface GlassMenuProps {
  className?: string
}

const tabs = [
  { id: 'home', label: 'Home', icon: Home },
  { id: 'likes', label: 'Likes', icon: Heart },
  { id: 'create', label: 'Create', icon: PlusCircle },
  { id: 'profile', label: 'Profile', icon: User },
  { id: 'alerts', label: 'Alerts', icon: Bell },
]

export const GlassMenu: React.FC<GlassMenuProps> = ({ className }) => {
  return (
    <motion.nav
      initial={{ opacity: 0, scale: 0.95 }}
      animate={{ opacity: 1, scale: 1 }}
      transition={{ type: 'spring', stiffness: 260, damping: 20 }}
      className={
        'fixed bottom-6 left-1/2 -translate-x-1/2 z-50 ' +
        'w-[317px] h-[58px] rounded-[10px] bg-black/60 backdrop-blur-md border border-white/10 ' +
        'flex items-center justify-center gap-2 px-3 py-2 ' +
        className
      }
      aria-label="Main navigation"
    >
      {tabs.map((tab) => (
        <button
          key={tab.id}
          type="button"
          aria-label={tab.label}
          className={
            'w-10 h-10 rounded-lg flex items-center justify-center ' +
            'transition-all duration-200 ease-out ' +
            'hover:bg-white/10 hover:scale-110 ' +
            'text-gray-400 hover:text-white'
          }
        >
          <tab.icon className="w-5 h-5" />
        </button>
      ))}
    </motion.nav>
  )
}
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class GlassMenu extends StatefulWidget {
  const GlassMenu({Key? key}) : super(key: key);

  @override
  State<GlassMenu> createState() => _GlassMenuState;
}

class _GlassMenuState extends State<GlassMenu> with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scale;
  late Animation<double> _opacity;

  final List<Map<String, dynamic>> tabs = [
    {'icon': Icons.home, 'label': 'Home'},
    {'icon': Icons.favorite, 'label': 'Likes'},
    {'icon': Icons.add_circle, 'label': 'Create'},
    {'icon': Icons.person, 'label': 'Profile'},
    {'icon': Icons.notifications, 'label': 'Alerts'},
  ];

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 6000),
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
        retur
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
