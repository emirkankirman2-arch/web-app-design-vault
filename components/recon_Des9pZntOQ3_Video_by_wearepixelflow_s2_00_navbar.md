---
title: "Navbar — Des9pZntOQ3_Video_by_wearepi (00:10.000)"
description: "Navbar UI component (recon_Des9pZntOQ3_Video_by_wearepixelflow_s2_00_navbar) with SSIM 0.9906, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_Des9pZntOQ3_Video_by_wearepixelflow_s2_00_navbar"
category: "Navbar"
ssim: 0.9906
quality_score: 8.72
tags: [navbar, ui-design, design-tokens, react, flutter]
---

# Navbar — Des9pZntOQ3_Video_by_wearepi (00:10.000)

> **Category:** [[04_Navbar|Navbar]] | **SSIM Fidelity:** `0.9906` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[03_GlassMenu|GlassMenu]], [[02_Button|Button]], [[05_Hero|Hero]]

Professional Navbar reverse-engineered from Des9pZntOQ3_Video_by_wearepixelflow at 00:10.000. Features FADE_IN_SCALE micro-interaction animation with 20.82:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#000000` | `rgb(0, 0, 0)` | `oklch(0.00 0.000 0.0)` | `61.3%` |
| `surface` | `#808080` | `rgb(128, 128, 128)` | `oklch(0.60 0.000 89.9)` | `1.1%` |
| `accent` | `#412EE9` | `rgb(65, 46, 233)` | `oklch(0.48 0.259 274.7)` | `5.0%` |
| `text` | `#FEFEFE` | `rgb(254, 254, 254)` | `oklch(1.00 0.000 89.9)` | `12.3%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `11.733 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react'
import { motion, AnimatePresence } from 'framer-motion'
import { Home, Heart, PlusCircle, User, Bell } from 'lucide-react'

interface NavItem {
  id: string
  label: string
  icon: React.ElementType
}

const NAV_ITEMS: NavItem[] = [
  { id: 'home', label: 'Home', icon: Home },
  { id: 'likes', label: 'Likes', icon: Heart },
  { id: 'create', label: 'Create', icon: PlusCircle },
  { id: 'profile', label: 'Profile', icon: User },
  { id: 'alerts', label: 'Alerts', icon: Bell },
]

export default function GlassNavbar({ activeId = 'home' }: { activeId?: string }) {
  return (
    <nav className="fixed bottom-6 left-1/2 -translate-x-1/2 z-50">
      <AnimatePresence mode="wait">
        <motion.div
          initial={{ opacity: 0, scale: 0.95 }}
          animate={{ opacity: 1, scale: 1 }}
          exit={{ opacity: 0, scale: 0.95 }}
          transition={{ type: 'spring', stiffness: 260, damping: 20 }}
          className="inline-flex items-center gap-1 px-3 py-2 rounded-full bg-black/60 backdrop-blur-md border border-white/10 shadow-2xl shadow-black/50"
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
                  'relative flex items-center justify-center w-10 h-10 rounded-full transition-colors duration-200 ' +
                 
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class GlassNavbar extends StatefulWidget {
  final String activeId;
  final ValueChanged<String> onItemTap;
  const GlassNavbar({Key? key, this.activeId = 'home', required this.onItemTap}) : super(key: key);

  @override
  _GlassNavbarState createState() => _GlassNavbarState();
}

class _GlassNavbarState extends State<GlassNavbar> with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scale;
  late Animation<double> _opacity;

  final List<Map<String, dynamic>> items = [
    {'id': 'home', 'label': 'Home', 'icon': Icons.home},
    {'id': 'likes', 'label': 'Likes', 'icon': Icons.favorite},
    {'id': 'create', 'label': 'Create', 'icon': Icons.add_circle},
    {'id': 'profile', 'label': 'Profile', 'icon': Icons.person},
    {'id': 'alerts', 'label': 'Alerts', 'icon': Icons.notifications},
  ];

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(vsync: this, duration: const Duration(milliseconds: 800));
    _scale = Tween<double>(begin: 0.95, end: 1.0).animate(CurvedAnimation(parent: _controller, curve: Curves.easeOut));
    _opacity = Tween<double>(begin: 0.0, end: 1.0).animate(CurvedAnimation(parent: _controller, curve: Curves.easeOut));
    _controller.forward();
  }

  @override
  void dispose() {
    _controller.dispose();
    super.dispose();
 
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
