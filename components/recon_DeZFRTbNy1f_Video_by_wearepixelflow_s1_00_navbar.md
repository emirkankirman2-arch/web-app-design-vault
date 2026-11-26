---
title: "Navbar — DeZFRTbNy1f_Video_by_wearepi (00:00.000)"
description: "Navbar UI component (recon_DeZFRTbNy1f_Video_by_wearepixelflow_s1_00_navbar) with SSIM 0.9921, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_DeZFRTbNy1f_Video_by_wearepixelflow_s1_00_navbar"
category: "Navbar"
ssim: 0.9921
quality_score: 8.72
tags: [navbar, ui-design, design-tokens, react, flutter]
---

# Navbar — DeZFRTbNy1f_Video_by_wearepi (00:00.000)

> **Category:** [[04_Navbar|Navbar]] | **SSIM Fidelity:** `0.9921` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[03_GlassMenu|GlassMenu]], [[02_Button|Button]], [[05_Hero|Hero]]

Professional Navbar reverse-engineered from DeZFRTbNy1f_Video_by_wearepixelflow at 00:00.000. Features FADE_IN_SCALE micro-interaction animation with 20.47:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#000000` | `rgb(0, 0, 0)` | `oklch(0.00 0.000 0.0)` | `55.5%` |
| `surface` | `#373639` | `rgb(55, 54, 57)` | `oklch(0.34 0.005 301.2)` | `0.9%` |
| `accent` | `#4C4C4E` | `rgb(76, 76, 78)` | `oklch(0.42 0.003 286.3)` | `5.0%` |
| `text` | `#FCFCFC` | `rgb(252, 252, 252)` | `oklch(0.99 0.000 89.9)` | `3.6%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `13.533 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
import React from 'react'
import { motion } from 'framer-motion'
import { Home, Heart, PlusCircle, User, Bell } from 'lucide-react'

interface NavItem {
  icon: React.ElementType
  label: string
  active: boolean
}

const NAV_ITEMS: NavItem[] = [
  { icon: Home, label: 'Home', active: true },
  { icon: Heart, label: 'Likes', active: false },
  { icon: PlusCircle, label: 'Create', active: false },
  { icon: User, label: 'Profile', active: false },
  { icon: Bell, label: 'Alerts', active: false },
]

export default function GlassNavbar() {
  return (
    <nav
      className="fixed bottom-0 left-1/2 -translate-x-1/2 mb-6 w-[338px] h-[61px]"
      aria-label="Main navigation"
    >
      <motion.div
        initial={{ opacity: 0, scale: 0.95 }}
        animate={{ opacity: 1, scale: 1 }}
        transition={{ type: 'spring', stiffness: 260, damping: 20 }}
        className="relative flex items-center justify-center gap-1 h-full w-full rounded-full bg-black/80 backdrop-blur-md border border-white/10 shadow-2xl"
      >
        {NAV_ITEMS.map((item, index) => (
          <button
            key={item.label}
            type="button"
            aria-pressed={item.active}
            aria-label={item.label}
            className={
              'relative flex flex-col items-center justify-center w-10 h-10 transition-all duration-200 ease-out'
            }
          >
            <item.icon
              className={
                `w-5 h-5 transition-colors duration-200 ${
                  item.active
                    ? 'text
```

## 4. Flutter / Dart Implementation

```dart
// Flutter StatefulWidget
import 'package:flutter/material.dart';\n\nclass GlassNavbar extends StatefulWidget {\n  const GlassNavbar({Key? key}) : super(key: key);\n\n  @override\n  State<GlassNavbar> createState() => _GlassNavbarState();\n}\n\nclass _GlassNavbarState extends State<GlassNavbar> {\n  int _selectedIndex = 0;\n\n  final List<Map<String, dynamic>> _items = [\n    {'icon': Icons.home, 'label': 'Home'},\n    {'icon': Icons.favorite, 'label': 'Likes'},\n    {'icon': Icons.add_circle, 'label': 'Create'},\n    {'icon': Icons.person, 'label': 'Profile'},\n    {'icon': Icons.notifications, 'label': 'Alerts'},\n  ];\n\n  @override\n  Widget build(BuildContext context) {\n    return Positioned(\n      bottom: 24,\n      left: MediaQuery.of(context).size.width / 2 - 169,\n      child: ClipRRect(\n        borderRadius: BorderRadius.circular(30.5),\n        child: BackdropFilter(\n          filter: ImageFilter.blur(sigmaX: 12, sigmaY: 12),\n          child: Container(\n            width: 338,\n            height: 61,\n            decoration: BoxDecoration(\n              color: Colors.black.withOpacity(0.8),\n              border: Border.all(color: Colors.white.withOpacity(0.1)),\n              borderRadius: BorderRadius.circular(30.5),\n              boxShadow: [\n                BoxShadow(\n                  color: Colors.black.withOpacity(0.5),\n                  blurRadius
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
