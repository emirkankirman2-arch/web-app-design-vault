---
title: "Navbar — DeVKbIFOOy0_Video_by_viewcci (00:10.200)"
description: "Navbar UI component (recon_DeVKbIFOOy0_Video_by_viewcci_s3_02_navbar) with SSIM 0.9899, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_DeVKbIFOOy0_Video_by_viewcci_s3_02_navbar"
category: "Navbar"
ssim: 0.9899
quality_score: 8.72
tags: [navbar, ui-design, design-tokens, react, flutter]
---

# Navbar — DeVKbIFOOy0_Video_by_viewcci (00:10.200)

> **Category:** [[04_Navbar|Navbar]] | **SSIM Fidelity:** `0.9899` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[03_GlassMenu|GlassMenu]], [[02_Button|Button]], [[05_Hero|Hero]]

Professional Navbar reverse-engineered from DeVKbIFOOy0_Video_by_viewcci at 00:10.200. Features FADE_IN_SCALE micro-interaction animation with 12.94:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#020102` | `rgb(2, 1, 2)` | `oklch(0.07 0.010 326.5)` | `23.7%` |
| `surface` | `#6E5951` | `rgb(110, 89, 81)` | `oklch(0.48 0.031 41.9)` | `17.0%` |
| `accent` | `#81744F` | `rgb(129, 116, 79)` | `oklch(0.56 0.055 90.9)` | `5.0%` |
| `text` | `#DAC9BA` | `rgb(218, 201, 186)` | `oklch(0.85 0.028 63.9)` | `4.5%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `10.2 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.05`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
// Reconstructed from video evidence: Vanguard Glass Navbar
// Style: AUTO | Animation: FADE_IN_SCALE | Theme: Dark

import React from 'react'
import { motion } from 'framer-motion'

interface NavItem {
  id: string
  label: string
  icon: React.ReactNode
}

const NAV_ITEMS: NavItem[] = [
  { id: 'home', label: 'Home', icon: <span className="sr-only">Home</span> }, // Icons would be SVG in production
  { id: 'likes', label: 'Likes', icon: <span className="sr-only">Likes</span> },
  { id: 'create', label: 'Create', icon: <span className="sr-only">Create</span> },
  { id: 'profile', label: 'Profile', icon: <span className="sr-only">Profile</span> },
  { id: 'alerts', label: 'Alerts', icon: <span className="sr-only">Alerts</span> },
]

export default function VanguardGlassNavbar({ activeId = 'home' }: { activeId?: string } = {}) {
  return (
    <nav
      className="fixed bottom-6 left-1/2 -translate-x-1/2 z-50"
      aria-label="Main navigation"
    >
      <motion.div
        initial={{ opacity: 0, scale: 0.95 }}
        animate={{ opacity: 1, scale: 1 }}
        transition={{ type: 'spring', stiffness: 260, damping: 20 }}
        className="flex items-center gap-2 px-4 py-2.5 rounded-full bg-black/60 backdrop-blur-md border border-white/10 shadow-2xl"
      >
        {NAV_ITEMS.map((item) => (
          <button
            key={item.id}
            onClick={() => {}}
            aria-pressed={activeId === item.id}
            className={
              'relative flex flex-col items-center justify-center w-10 h-10 rounded-lg
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class VanguardGlassNavbar extends StatefulWidget {
  final String activeId;
  final ValueChanged<String> onItemTap;

  const VanguardGlassNavbar({super.key, this.activeId = 'home', required this.onItemTap});

  @override
  State<VanguardGlassNavbar> createState() => _VanguardGlassNavbarState;
}

class _VanguardGlassNavbarState extends State<VanguardGlassNavbar>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scaleAnim;
  late Animation<double> _opacityAnim;

  final List<Map<String, String>> items = const [
    {'id': 'home', 'label': 'Home'},
    {'id': 'likes', 'label': 'Likes'},
    {'id': 'create', 'label': 'Create'},
    {'id': 'profile', 'label': 'Profile'},
    {'id': 'alerts', 'label': 'Alerts'},
  ];

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(vsync: this, duration: const Duration(milliseconds: 10200));
    _scaleAnim = Tween<double>(begin: 0.95, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.elasticOut),
    );
    _opacityAnim = Tween<double>(begin: 0.0, end: 1.0).animate(_controller);
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
      animat
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
