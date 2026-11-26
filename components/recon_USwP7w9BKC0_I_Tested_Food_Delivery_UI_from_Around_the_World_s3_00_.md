---
title: "GlassMenu — USwP7w9BKC0_I_Tested_Food_De (11:41.233)"
description: "GlassMenu UI component (recon_USwP7w9BKC0_I_Tested_Food_Delivery_UI_from_Around_the_World_s3_00_) with SSIM 0.991, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_USwP7w9BKC0_I_Tested_Food_Delivery_UI_from_Around_the_World_s3_00_glassmenu"
category: "GlassMenu"
ssim: 0.991
quality_score: 8.72
tags: [glassmenu, ui-design, design-tokens, react, flutter]
---

# GlassMenu — USwP7w9BKC0_I_Tested_Food_De (11:41.233)

> **Category:** [[03_GlassMenu|GlassMenu]] | **SSIM Fidelity:** `0.991` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[04_Navbar|Navbar]], [[01_Card|Card]], [[10_ShaderCanvas|ShaderCanvas]]

Professional GlassMenu reverse-engineered from USwP7w9BKC0_I_Tested_Food_Delivery_UI_from_Around_the_World at 11:41.233. Features FADE_IN_SCALE micro-interaction animation with 12.94:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#CBCBCB` | `rgb(203, 203, 203)` | `oklch(0.84 0.000 89.9)` | `39.6%` |
| `surface` | `#C1C4C4` | `rgb(193, 196, 196)` | `oklch(0.82 0.003 197.1)` | `21.0%` |
| `accent` | `#545454` | `rgb(84, 84, 84)` | `oklch(0.45 0.000 89.9)` | `5.0%` |
| `text` | `#000000` | `rgb(0, 0, 0)` | `oklch(0.00 0.000 0.0)` | `33.5%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `70.767 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.51`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
// GlassMenu - 5-tab frosted glass navigation bar
// Reconstructed from video evidence: USwP7w9BKC0_I_Tested_Food_Delivery_UI_from_Around_the_World.mp4 @ 11:41.233

import React from 'react'
import { motion, AnimatePresence } from 'framer-motion'

interface GlassMenuProps {
  className?: string
}

const tabs = [
  { id: 'home', label: 'Home', icon: '🏠' },
  { id: 'likes', label: 'Likes', icon: '❤️' },
  { id: 'create', label: 'Create', icon: '✨' },
  { id: 'profile', label: 'Profile', icon: '👤' },
  { id: 'alerts', label: 'Alerts', icon: '🔔' },
]

export const GlassMenu: React.FC<GlassMenuProps> = ({ className }) => {
  const [activeTab, setActiveTab] = React.useState<string>('home')

  return (
    <motion.nav
      initial={{ opacity: 0, scale: 0.95 }}
      animate={{ opacity: 1, scale: 1 }}
      transition={{ type: 'spring', stiffness: 260, damping: 20 }}
      className={
        'relative flex items-center justify-center gap-2 px-4 py-2 rounded-[14px] bg-white/60 backdrop-blur-md border border-white/40 shadow-none ' +
        (className || '')
      }
      aria-label="Main navigation"
    >
      {tabs.map((tab) => (
        <button
          key={tab.id}
          onClick={() => setActiveTab(tab.id)}
          aria-pressed={activeTab === tab.id}
          aria-label={tab.label}
          className={
            'flex flex-col items-center justify-center w-10 h-10 rounded-full transition-all duration-200 ' +
            (activeTab === tab.id
              ? 'bg-[#545454] text-white shadow-lg'
              : 'bg-tra
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class GlassMenu extends StatefulWidget {
  const GlassMenu({Key? key}) : super(key: key);

  @override
  State<GlassMenu> createState() => _GlassMenuState();
}

class _GlassMenuState extends State<GlassMenu>
    with SingleTickerProviderStateMixin {
  int _activeIndex = 0;
  late AnimationController _controller;
  late Animation<double> _scaleAnim;
  late Animation<double> _opacityAnim;

  final List<Map<String, String>> _tabs = [
    {'label': 'Home', 'icon': '🏠'},
    {'label': 'Likes', 'icon': '❤️'},
    {'label': 'Create', 'icon': '✨'},
    {'label': 'Profile', 'icon': '👤'},
    {'label': 'Alerts', 'icon': '🔔'},
  ];

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 700),
    );
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
  Widget build(BuildContext context) {
    return AnimatedBuilder(
      animation: _controller,
      builder: (context, child) {
        return Opacity(
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
