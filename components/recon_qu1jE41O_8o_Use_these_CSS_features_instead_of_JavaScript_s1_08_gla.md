---
title: "GlassMenu — qu1jE41O_8o_Use_these_CSS_fe (00:00.000)"
description: "GlassMenu UI component (recon_qu1jE41O_8o_Use_these_CSS_features_instead_of_JavaScript_s1_08_gla) with SSIM 0.9891, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_qu1jE41O_8o_Use_these_CSS_features_instead_of_JavaScript_s1_08_glassmenu"
category: "GlassMenu"
ssim: 0.9891
quality_score: 8.72
tags: [glassmenu, ui-design, design-tokens, react, flutter]
---

# GlassMenu — qu1jE41O_8o_Use_these_CSS_fe (00:00.000)

> **Category:** [[03_GlassMenu|GlassMenu]] | **SSIM Fidelity:** `0.9891` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[04_Navbar|Navbar]], [[01_Card|Card]], [[10_ShaderCanvas|ShaderCanvas]]

Professional GlassMenu reverse-engineered from qu1jE41O_8o_Use_these_CSS_features_instead_of_JavaScript at 00:00.000. Features FADE_IN_SCALE micro-interaction animation with 6.57:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#140F15` | `rgb(20, 15, 21)` | `oklch(0.18 0.015 320.7)` | `32.5%` |
| `surface` | `#5C4152` | `rgb(92, 65, 82)` | `oklch(0.41 0.045 341.1)` | `15.2%` |
| `accent` | `#0B242C` | `rgb(11, 36, 44)` | `oklch(0.24 0.034 221.9)` | `5.0%` |
| `text` | `#339EF0` | `rgb(51, 158, 240)` | `oklch(0.68 0.154 246.4)` | `9.0%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `130.333 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.94`

## 3. React + TypeScript + Tailwind Implementation

```tsx
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

export const GlassMenu: React.FC<GlassMenuProps> = ({ activeTab = 'home', onTabChange }) => {
  return (
    <motion.div
      initial={{ opacity: 0, scale: 0.95 }}
      animate={{ opacity: 1, scale: 1 }}
      transition={{ type: 'spring', stiffness: 260, damping: 20 }}
      className="fixed bottom-8 left-1/2 -translate-x-1/2 z-50"
    >
      <div className="relative">
        {/* Frosted glass background */}
        <div className="absolute inset-0 bg-[#140F15]/60 backdrop-blur-md rounded-full border border-white/10 shadow-2xl"></div>

        {/* Navigation items */}
        <div className="relative flex items-center justify-center gap-2 px-4 py-2 h-14 w-72 rounded-full">
          {tabs.map((tab) => (
            <button
              key={tab.id}
              onClick={() => onTabChange?.(tab.id)}
              className={
                'relative flex flex-col items-center justify-center w-8 h-8 rounded-full transition-all duration-200 ' +
                (activeTab === tab.id
                  ? 'bg-[#339EF0]/20 text-[#339EF0] shadow-[0_0_15px_rgba(51,158,240,0.4)]'
                  : 'text-[#5C4152] hover:text-[#339EF0] hover:bg-white/10')
              }
   
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class GlassMenu extends StatefulWidget {
  final String activeTab;
  final ValueChanged<String> onTabChange;
  const GlassMenu({super.key, this.activeTab = 'home', required this.onTabChange});

  @override
  State<GlassMenu> createState() => _GlassMenuState;
}

class _GlassMenuState extends State<GlassMenu> with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scale;
  late Animation<double> _opacity;

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
    _controller = AnimationController(vsync: this, duration: const Duration(milliseconds: 800));
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

```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
