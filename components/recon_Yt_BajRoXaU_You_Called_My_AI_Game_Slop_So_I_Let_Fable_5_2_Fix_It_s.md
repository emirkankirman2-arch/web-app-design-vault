---
title: "GlassMenu — Yt_BajRoXaU_You_Called_My_AI (00:00.000)"
description: "GlassMenu UI component (recon_Yt_BajRoXaU_You_Called_My_AI_Game_Slop_So_I_Let_Fable_5_2_Fix_It_s) with SSIM 0.9887, OKLCH design tokens, SLIDE_DOWN motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_Yt-BajRoXaU_You_Called_My_AI_Game_Slop_So_I_Let_Fable_5.2_Fix_It_s1_02_glassmenu"
category: "GlassMenu"
ssim: 0.9887
quality_score: 8.72
tags: [glassmenu, ui-design, design-tokens, react, flutter]
---

# GlassMenu — Yt_BajRoXaU_You_Called_My_AI (00:00.000)

> **Category:** [[03_GlassMenu|GlassMenu]] | **SSIM Fidelity:** `0.9887` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[04_Navbar|Navbar]], [[01_Card|Card]], [[10_ShaderCanvas|ShaderCanvas]]

Professional GlassMenu reverse-engineered from Yt-BajRoXaU_You_Called_My_AI_Game_Slop_So_I_Let_Fable_5.2_Fix_It at 00:00.000. Features SLIDE_DOWN micro-interaction animation with 13.4:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#121214` | `rgb(18, 18, 20)` | `oklch(0.18 0.004 286.0)` | `28.6%` |
| `surface` | `#43443F` | `rgb(67, 68, 63)` | `oklch(0.38 0.008 116.0)` | `13.9%` |
| `accent` | `#0A0B12` | `rgb(10, 11, 18)` | `oklch(0.15 0.015 278.1)` | `5.0%` |
| `text` | `#DEDACF` | `rgb(222, 218, 207)` | `oklch(0.89 0.015 90.2)` | `4.5%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `SLIDE_DOWN`
- **Measured Duration:** `96.667 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `0.64`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
// GlassMenu - 5-tab frosted glass navigation bar
// Reconstructed from video evidence: Yt-BajRoXaU_You_Called_My_AI_Game_Slop_So_I_Let_Fable_5.2_Fix_It.mp4

import React, { useState } from 'react'
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

export default function GlassMenu() {
  const [activeId, setActiveId] = useState<string>('home')

  return (
    <nav
      className="fixed bottom-6 left-1/2 -translate-x-1/2 z-50"
      aria-label="Main navigation"
    >
      <AnimatePresence mode="wait">
        <motion.div
          initial={{ opacity: 0, y: -6.97 }}
          animate={{ opacity: 1, y: 0 }}
          exit={{ opacity: 0, y: 6 }}
          transition {{
            duration: 0.9,
            ease: [0.16, 1, 0.3, 1],
          }}
          className="inline-flex items-center gap-1 px-3 py-2 rounded-full bg-white/10 backdrop-blur-md border border-white/5 shadow-lg"
        >
          {NAV_ITEMS.map((item) => (
            <button
              key={item.id}
              onClick={() => setActiveId(item.id)}
              aria-pressed={activeId === item.id}
              aria-label={item
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class GlassMenu extends StatefulWidget {
  const GlassMenu({super.key});

  @override
  State<GlassMenu> createState() => _GlassMenuState;
}

class _GlassMenuState extends State<GlassMenu> {
  int _selectedIndex = 0;

  final List<Map<String, dynamic>> _items = [
    {'icon': Icons.home, 'label': 'Home'},
    {'icon': Icons.favorite, 'label': 'Likes'},
    {'icon': Icons.add_circle, 'label': 'Create'},
    {'icon': Icons.person, 'label': 'Profile'},
    {'icon': Icons.notifications, 'label': 'Alerts'},
  ];

  @override
  Widget build(BuildContext context) {
    return Positioned(
      bottom: 24,
      left: 0,
      right: 0,
      child: Center(
        child: ClipRRect(
          borderRadius: BorderRadius.circular(20),
          child: BackdropFilter(
            filter: ImageFilter.blur(sigmaX: 12, sigmaY: 12),
            child: Container(
              width: 171,
              height: 64,
              decoration: BoxDecoration(
                color: Colors.white.withOpacity(0.1),
                borderRadius: BorderRadius.circular(20),
                border: Border.all(color: Colors.white.withOpacity(0.05)),
                boxShadow: [
                  BoxShadow(
                    color: Colors.black.withOpacity(0.5),
                    blurRadius: 30,
                    offset: Offset(0, 10),
                  ),
    
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
