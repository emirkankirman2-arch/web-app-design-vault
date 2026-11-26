---
title: "Navbar — Des9pZntOQ3_Video_by_wearepi (00:00.000)"
description: "Navbar UI component (recon_Des9pZntOQ3_Video_by_wearepixelflow_s1_00_navbar) with SSIM 0.99, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_Des9pZntOQ3_Video_by_wearepixelflow_s1_00_navbar"
category: "Navbar"
ssim: 0.99
quality_score: 8.72
tags: [navbar, ui-design, design-tokens, react, flutter]
---

# Navbar — Des9pZntOQ3_Video_by_wearepi (00:00.000)

> **Category:** [[04_Navbar|Navbar]] | **SSIM Fidelity:** `0.99` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[03_GlassMenu|GlassMenu]], [[02_Button|Button]], [[05_Hero|Hero]]

Professional Navbar reverse-engineered from Des9pZntOQ3_Video_by_wearepixelflow at 00:00.000. Features FADE_IN_SCALE micro-interaction animation with 20.68:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#000000` | `rgb(0, 0, 0)` | `oklch(0.00 0.000 0.0)` | `61.3%` |
| `surface` | `#808080` | `rgb(128, 128, 128)` | `oklch(0.60 0.000 89.9)` | `1.1%` |
| `accent` | `#402FE6` | `rgb(64, 47, 230)` | `oklch(0.47 0.255 274.6)` | `5.0%` |
| `text` | `#FEFDFD` | `rgb(254, 253, 253)` | `oklch(0.99 0.001 17.2)` | `12.9%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `11.733 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react'
import { motion, AnimatePresence } from 'framer-motion'
import { Home, Heart, Plus, User, Bell } from 'lucide-react'

interface NavItem {
  id: string
  label: string
  icon: React.ElementType
}

const NAV_ITEMS: NavItem[] = [
  { id: 'home', label: 'Home', icon: Home },
  { id: 'likes', label: 'Likes', icon: Heart },
  { id: 'create', label: 'Create', icon: Plus },
  { id: 'profile', label: 'Profile', icon: User },
  { id: 'alerts', label: 'Alerts', icon: Bell },
]

export default function GlassNavbar({ activeId = 'home' }: { activeId?: string }) {
  return (
    <nav className="fixed bottom-0 left-0 right-0 z-50 px-4 pb-6">
      <AnimatePresence mode="wait">
        <motion.div
          initial={{ opacity: 0, scale: 0.95 }}
          animate={{ opacity: 1, scale: 1 }}
          exit={{ opacity: 0, scale: 0.95 }}
          transition={{ type: 'spring', stiffness: 260, damping: 20 }}
          className="mx-auto w-[197px] h-[58px] rounded-full bg-black/60 backdrop-blur-md border border-white/10 flex items-center justify-center gap-1 px-2 py-1 shadow-lg shadow-black/40"
        >
          {NAV_ITEMS.map((item) => {
            const isActive = item.id === activeId
            return (
              <motion.button
                key={item.id}
                whileHover={{ scale: 1.1 }}
                whileTap={{ scale: 0.9 }}
                aria-pressed={isActive}
                aria-label={item.label}
                className={
                  'w-10 h-10 rounded-full flex items-center justify-center transition-all duration-200 ' +
        
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class GlassNavbar extends StatefulWidget {
  final String activeId;
  final ValueChanged<String> onItemTap;
  const GlassNavbar({super.key, this.activeId = 'home', required this.onItemTap});

  @override
  State<GlassNavbar> createState() => _GlassNavbarState;
}

class _GlassNavbarState extends State<GlassNavbar> with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scaleAnim;
  late Animation<double> _opacityAnim;

  final List<Map<String, dynamic>> items = [
    {'id': 'home', 'icon': Icons.home},
    {'id': 'likes', 'icon': Icons.favorite_border},
    {'id': 'create', 'icon': Icons.add},
    {'id': 'profile', 'icon': Icons.person_outline},
    {'id': 'alerts', 'icon': Icons.notifications_outlined},
  ];

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(vsync: this, duration: const Duration(milliseconds: 11733));
    _scaleAnim = Tween<double>(begin: 0.95, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOut),
    );
    _opacityAnim = Tween<double>(begin: 0.0, end: 1.0).animate(
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
  Widget build(BuildContext contex
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
