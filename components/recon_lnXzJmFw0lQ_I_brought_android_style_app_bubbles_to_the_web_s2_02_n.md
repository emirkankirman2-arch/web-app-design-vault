---
title: "Navbar — lnXzJmFw0lQ_I_brought_androi (01:12.100)"
description: "Navbar UI component (recon_lnXzJmFw0lQ_I_brought_android_style_app_bubbles_to_the_web_s2_02_n) with SSIM 0.9931, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_lnXzJmFw0lQ_I_brought_android_style_app_bubbles_to_the_web_s2_02_navbar"
category: "Navbar"
ssim: 0.9931
quality_score: 8.72
tags: [navbar, ui-design, design-tokens, react, flutter]
---

# Navbar — lnXzJmFw0lQ_I_brought_androi (01:12.100)

> **Category:** [[04_Navbar|Navbar]] | **SSIM Fidelity:** `0.9931` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[03_GlassMenu|GlassMenu]], [[02_Button|Button]], [[05_Hero|Hero]]

Professional Navbar reverse-engineered from lnXzJmFw0lQ_I_brought_android_style_app_bubbles_to_the_web at 01:12.100. Features FADE_IN_SCALE micro-interaction animation with 18.93:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#000000` | `rgb(0, 0, 0)` | `oklch(0.00 0.000 0.0)` | `91.1%` |
| `surface` | `#424F46` | `rgb(66, 79, 70)` | `oklch(0.41 0.022 155.1)` | `1.2%` |
| `accent` | `#26CA57` | `rgb(38, 202, 87)` | `oklch(0.74 0.203 147.8)` | `0.6%` |
| `text` | `#F3F3F3` | `rgb(243, 243, 243)` | `oklch(0.96 0.000 89.9)` | `2.0%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `24.5 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.04`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
// Reconstructed from video evidence: lnXzJmFw0lQ_I_brought_android_style_app_bubbles_to_the_web.mp4
// DESKTOP view at 01:12.100

import React from 'react'
import { motion } from 'framer-motion'

interface NavItem {
  id: string
  label: string
  icon: React.ReactNode
}

const NAV_ITEMS: NavItem[] = [
  { id: 'home', label: 'Home', icon: <span className="text-[14px]">🏠</span> },
  { id: 'likes', label: 'Likes', icon: <span className="text-[14px]">❤️</span> },
  { id: 'create', label: 'Create', icon: <span className="text-[14px]">✨</span> },
  { id: 'profile', label: 'Profile', icon: <span className="text-[14px]">👤</span> },
  { id: 'alerts', label: 'Alerts', icon: <span className="text-[14px]">🔔</span> },
]

export default function GlassNavbar() {
  const [activeId, setActiveId] = React.useState<string>('home')

  return (
    <nav
      className="fixed bottom-8 left-1/2 -translate-x-1/2 z-50"
      aria-label="Main navigation"
    >
      <motion.div
        initial={{ opacity: 0, scale: 0.95 }}
        animate={{ opacity: 1, scale: 1 }}
        transition={
          type: 'spring',
          stiffness: 260,
          damping: 20
        }
        className="flex items-center justify-center gap-1 px-4 py-2.5 bg-black/80 backdrop-blur-xl backdrop-saturate-150 border border-white/10 rounded-full shadow-2xl shadow-black/50"
        style={{ width: 715, height: 78 }}
      >
        {NAV_ITEMS.map((item) => (
          <button
            key={item.id}
            onClick={() => setActiveId(item.id)}
            aria-presse
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class GlassNavbar extends StatefulWidget {
  const GlassNavbar({super.key});

  @override
  State<GlassNavbar> createState() => _GlassNavbarState;
}

class _GlassNavbarState extends State<GlassNavbar>
    with SingleTickerProviderStateMixin {
  int _activeIndex = 0;
  late AnimationController _controller;
  late Animation<double> _scaleAnim;
  late Animation<double> _opacityAnim;

  final List<Map<String, dynamic>> _items = const [
    {'label': 'Home', 'icon': Icons.home},
    {'label': 'Likes', 'icon': Icons.favorite},
    {'label': 'Create', 'icon': Icons.add_circle},
    {'label': 'Profile', 'icon': Icons.person},
    {'label': 'Alerts', 'icon': Icons.notifications},
  ];

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 24500),
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
    return Positioned(
      bottom: 32,
      left: Medi
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
