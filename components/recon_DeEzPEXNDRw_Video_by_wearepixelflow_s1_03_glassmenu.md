---
title: "GlassMenu — DeEzPEXNDRw_Video_by_wearepi (00:00.000)"
description: "GlassMenu UI component (recon_DeEzPEXNDRw_Video_by_wearepixelflow_s1_03_glassmenu) with SSIM 0.9887, OKLCH design tokens, FADE_AND_SLIDE_UP motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_DeEzPEXNDRw_Video_by_wearepixelflow_s1_03_glassmenu"
category: "GlassMenu"
ssim: 0.9887
quality_score: 8.72
tags: [glassmenu, ui-design, design-tokens, react, flutter]
---

# GlassMenu — DeEzPEXNDRw_Video_by_wearepi (00:00.000)

> **Category:** [[03_GlassMenu|GlassMenu]] | **SSIM Fidelity:** `0.9887` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[04_Navbar|Navbar]], [[01_Card|Card]], [[10_ShaderCanvas|ShaderCanvas]]

Professional GlassMenu reverse-engineered from DeEzPEXNDRw_Video_by_wearepixelflow at 00:00.000. Features FADE_AND_SLIDE_UP micro-interaction animation with 17.57:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#000000` | `rgb(0, 0, 0)` | `oklch(0.00 0.000 0.0)` | `54.2%` |
| `surface` | `#3A2E3D` | `rgb(58, 46, 61)` | `oklch(0.32 0.031 319.5)` | `5.1%` |
| `accent` | `#EFD045` | `rgb(239, 208, 69)` | `oklch(0.86 0.155 96.2)` | `1.1%` |
| `text` | `#ECE9F7` | `rgb(236, 233, 247)` | `oklch(0.94 0.019 295.9)` | `12.0%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_AND_SLIDE_UP`
- **Measured Duration:** `0.45 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `120.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
import React from 'react';
import { motion } from 'framer-motion';
import { Home, Heart, Plus, User, Bell } from 'lucide-react';

interface GlassMenuProps {
  activeTab?: 'home' | 'likes' | 'create' | 'profile' | 'alerts';
  onTabChange?: (tab: string) => void;
}

const tabs = [
  { id: 'home', label: 'Home', icon: Home },
  { id: 'likes', label: 'Likes', icon: Heart },
  { id: 'create', label: 'Create', icon: Plus },
  { id: 'profile', label: 'Profile', icon: User },
  { id: 'alerts', label: 'Alerts', icon: Bell },
] as const;

export default function GlassMenu({ activeTab = 'home', onTabChange }: GlassMenuProps) {
  return (
    <motion.nav
      initial={{ opacity: 0, y: 24 }}
      animate={{ opacity: 1, y: 0 }}
      transition={{ duration: 0.45, ease: [0.16, 1, 0.3, 1] }}
      className="fixed bottom-6 left-1/2 -translate-x-1/2 w-[237px] h-[59px] rounded-[10px] bg-black/40 backdrop-blur-md border border-white/10 flex items-center justify-center gap-1 px-2 py-1 z-50"
      aria-label="Main navigation"
    >
      {tabs.map((tab) => {
        const isActive = activeTab === tab.id;
        const Icon = tab.icon;
        return (
          <motion.button
            key={tab.id}
            whileHover={{ scale: 1.1 }}
            whileTap={{ scale: 0.9 }}
            onClick={() => onTabChange?.(tab.id)}
            className={
              'w-10 h-10 rounded-lg flex items-center justify-center transition-all duration-200 ' +
              (isActive
                ? 'bg-[#EFD045] text-black shadow-[0_0_15px_rgba(239,20
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class GlassMenu extends StatefulWidget {
  final String activeTab;
  final ValueChanged<String> onTabChange;
  const GlassMenu({super.key, this.activeTab = 'home', required this.onTabChange});

  @override
  State<GlassMenu> createState() => _GlassMenuState();
}

class _GlassMenuState extends State<GlassMenu> with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<Offset> _offsetAnimation;
  late Animation<double> _opacityAnimation;

  final List<Map<String, dynamic>> tabs = [
    {'id': 'home', 'icon': Icons.home},
    {'id': 'likes', 'icon': Icons.favorite},
    {'id': 'create', 'icon': Icons.add},
    {'id': 'profile', 'icon': Icons.person},
    {'id': 'alerts', 'icon': Icons.notifications},
  ];

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(vsync: this, duration: const Duration(milliseconds: 450));
    _offsetAnimation = Tween<Offset>(begin: const Offset(0, 0.3), end: Offset.zero).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeInOut),
    );
    _opacityAnimation = Tween<double>(begin: 0.0, end: 1.0).animate(
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
  Widget build(
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
