---
title: "GlassMenu — USwP7w9BKC0_I_Tested_Food_De (11:41.233)"
description: "GlassMenu UI component (recon_USwP7w9BKC0_I_Tested_Food_Delivery_UI_from_Around_the_World_s3_03_) with SSIM 0.9893, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_USwP7w9BKC0_I_Tested_Food_Delivery_UI_from_Around_the_World_s3_03_glassmenu"
category: "GlassMenu"
ssim: 0.9893
quality_score: 8.72
tags: [glassmenu, ui-design, design-tokens, react, flutter]
---

# GlassMenu — USwP7w9BKC0_I_Tested_Food_De (11:41.233)

> **Category:** [[03_GlassMenu|GlassMenu]] | **SSIM Fidelity:** `0.9893` | **Quality Score:** `8.72 / 10`  
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
import { motion } from 'framer-motion'

interface GlassMenuProps {
  activeTab?: string
  onTabChange?: (tab: string) => void
}

const tabs = [
  { id: 'home', label: 'Home', icon: '🏠' },
  { id: 'likes', label: 'Likes', icon: '❤️' },
  { id: 'create', label: 'Create', icon: '✨' },
  { id: 'profile', label: 'Profile', icon: '👤' },
  { id: 'alerts', label: 'Alerts', icon: '🔔' },
]

export const GlassMenu: React.FC<GlassMenuProps> = ({
  activeTab = 'home',
  onTabChange,
}) => {
  const containerVariants = {
    hidden: { opacity: 0, scale: 0.95 },
    visible: {
      opacity: 1,
      scale: 1,
      transition: {
        type: 'spring',
        stiffness: 260,
        damping: 20,
      },
    },
  }

  const itemVariants = {
    hidden: { opacity: 0, y: 10 },
    visible: {
      opacity: 1,
      y: 0,
      transition: { duration: 0.3 },
    },
  }

  return (
    <motion.div
      initial="hidden"
      animate="visible"
      variants={containerVariants}
      className="fixed bottom-8 left-1/2 -translate-x-1/2 w-[442px] h-[133px] rounded-[23px] bg-white/60 backdrop-blur-xl border border-white/40 shadow-none flex items-center justify-center gap-2 p-2"
    >
      {tabs.map((tab) => (
        <motion.div
          key={tab.id}
          initial="hidden"
          animate="visible"
          variants={itemVariants}
          whileH
```

## 4. Flutter / Dart Implementation

```dart
// Flutter StatefulWidget - GlassMenu
// Reconstructed from video evidence

import 'package:flutter/material.dart';

class GlassMenu extends StatefulWidget {
  const GlassMenu({Key? key}) : super(key: key);

  @override
  State<GlassMenu> createState() => _GlassMenuState();
}

class _GlassMenuState extends State<GlassMenu>
    with SingleTickerProviderStateMixin {
  String activeTab = 'home';
  late AnimationController _controller;
  late Animation<double> _scaleAnimation;
  late Animation<double> _opacityAnimation;

  final List<Map<String, String>> tabs = [
    {'id': 'home', 'label': 'Home', 'icon': '🏠'},
    {'id': 'likes', 'label': 'Likes', 'icon': '❤️'},
    {'id': 'create', 'label': 'Create', 'icon': '✨'},
    {'id': 'profile', 'label': 'Profile', 'icon': '👤'},
    {'id': 'alerts', 'label': 'Alerts', 'icon': '🔔'},
  ];

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 700),
    );
    _scaleAnimation = Tween<double>(begin: 0.95, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOutBack),
    );
    _opacityAnimation = Tween<double>(begin: 0.0, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeIn),
    );
    _controller.forward();
  }

  @override
  void dispose() {
    _controller.dispose();
    super.d
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
