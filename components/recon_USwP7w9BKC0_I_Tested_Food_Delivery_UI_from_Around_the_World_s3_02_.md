---
title: "GlassMenu — USwP7w9BKC0_I_Tested_Food_De (11:41.233)"
description: "GlassMenu UI component (recon_USwP7w9BKC0_I_Tested_Food_Delivery_UI_from_Around_the_World_s3_02_) with SSIM 0.9939, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_USwP7w9BKC0_I_Tested_Food_Delivery_UI_from_Around_the_World_s3_02_glassmenu"
category: "GlassMenu"
ssim: 0.9939
quality_score: 8.72
tags: [glassmenu, ui-design, design-tokens, react, flutter]
---

# GlassMenu — USwP7w9BKC0_I_Tested_Food_De (11:41.233)

> **Category:** [[03_GlassMenu|GlassMenu]] | **SSIM Fidelity:** `0.9939` | **Quality Score:** `8.72 / 10`  
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
// React TypeScript + Tailwind CSS
// GlassMenu - 5-tab frosted glass navigation bar
// Reverse engineered from video USwP7w9BKC0_I_Tested_Food_Delivery_UI_from_Around_the_World.mp4 @ 11:41.233

import React from 'react'
import { motion, AnimatePresence } from 'framer-motion'
import { Home, Heart, PlusCircle, User, Bell } from 'lucide-react'

interface GlassMenuProps {
  className?: string
  activeTab?: 'home' | 'likes' | 'create' | 'profile' | 'alerts'
  onTabChange?: (tab: string) => void
}

const tabs = [
  { id: 'home', label: 'Home', icon: Home },
  { id: 'likes', label: 'Likes', icon: Heart },
  { id: 'create', label: 'Create', icon: PlusCircle },
  { id: 'profile', label: 'Profile', icon: User },
  { id: 'alerts', label: 'Alerts', icon: Bell },
]

export const GlassMenu: React.FC<GlassMenuProps> = ({
  className = '',
  activeTab = 'home',
  onTabChange,
}) => {
  return (
    <AnimatePresence>
      <motion.nav
        initial={{ opacity: 0, scale: 0.95 }}
        animate={{ opacity: 1, scale: 1 }}
        exit={{ opacity: 0, scale: 0.95 }}
        transition={
          type: 'spring',
          stiffness: 260,
          damping: 20
        }
        className={
          'fixed bottom-8 left-1/2 -translate-x-1/2 z-50 ' +
          'bg-white/60 backdrop-blur-md border border-white/40 ' +
          'rounded-full px-4 py-2.5 shadow-lg ' +
          className
        }
      >
        <div className="flex items-center gap-3">
          {tabs.map((tab) => {
            const isActive = activeTab === tab.id
            const Icon = tab.icon
            return (
        
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';
import 'package:flutter/semantics.dart';

class GlassMenu extends StatefulWidget {
  final ValueChanged<String>? onTabChange;
  final String initialTab;

  const GlassMenu({Key? key, this.onTabChange, this.initialTab = 'home'}) : super(key: key);

  @override
  _GlassMenuState createState() => _GlassMenuState();
}

class _GlassMenuState extends State<GlassMenu> with SingleTickerProviderStateMixin {
  late String _activeTab;
  late AnimationController _controller;
  late Animation<double> _scaleAnim;
  late Animation<double> _opacityAnim;

  final List<Map<String, dynamic>> _tabs = [
    {'id': 'home', 'label': 'Home', 'icon': Icons.home},
    {'id': 'likes', 'label': 'Likes', 'icon': Icons.favorite},
    {'id': 'create', 'label': 'Create', 'icon': Icons.add_circle},
    {'id': 'profile', 'label': 'Profile', 'icon': Icons.person},
    {'id': 'alerts', 'label': 'Alerts', 'icon': Icons.notifications},
  ];

  @override
  void initState() {
    super.initState();
    _activeTab = widget.initialTab;
    _controller = AnimationController(vsync: this, duration: const Duration(milliseconds: 700));
    _scaleAnim = Tween<double>(begin: 0.95, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOutCubic),
    );
    _opacityAnim = Tween<double>(begin: 0.0, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curv
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
