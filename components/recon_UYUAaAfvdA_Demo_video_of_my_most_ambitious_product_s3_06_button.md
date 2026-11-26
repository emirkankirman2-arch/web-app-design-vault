---
title: "Button — UYUAaAfvdA_Demo_video_of_my_ (11:08.434)"
description: "Button UI component (recon_UYUAaAfvdA_Demo_video_of_my_most_ambitious_product_s3_06_button) with SSIM 0.9906, OKLCH design tokens, SLIDE_UP motion spec, React/Tailwind & Flutter implementations."
component_id: "recon__UYUAaAfvdA_Demo_video_of_my_most_ambitious_product_s3_06_button"
category: "Button"
ssim: 0.9906
quality_score: 8.72
tags: [button, ui-design, design-tokens, react, flutter]
---

# Button — UYUAaAfvdA_Demo_video_of_my_ (11:08.434)

> **Category:** [[02_Button|Button]] | **SSIM Fidelity:** `0.9906` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[01_Card|Card]], [[06_Input|Input]], [[08_Modal|Modal]]

Professional Button reverse-engineered from _UYUAaAfvdA_Demo_video_of_my_most_ambitious_product at 11:08.434. Features SLIDE_UP micro-interaction animation with 10.16:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#110E18` | `rgb(17, 14, 24)` | `oklch(0.17 0.021 297.9)` | `48.6%` |
| `surface` | `#726B75` | `rgb(114, 107, 117)` | `oklch(0.54 0.018 315.9)` | `5.4%` |
| `accent` | `#0D1043` | `rgb(13, 16, 67)` | `oklch(0.21 0.094 272.6)` | `5.0%` |
| `text` | `#B6BEC7` | `rgb(182, 190, 199)` | `oklch(0.80 0.016 251.2)` | `4.0%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `SLIDE_UP`
- **Measured Duration:** `67.067 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `0.31`

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

export default function GlassNavigationBar({ activeId = 'home' }: { activeId?: string }) {
  return (
    <nav className="fixed bottom-6 left-1/2 -translate-x-1/2 z-50">
      <div className="flex items-center gap-3 px-4 py-2.5 bg-[#110E18]/80 backdrop-blur-xl border border-white/10 rounded-full shadow-2xl shadow-black/50">
        {NAV_ITEMS.map((item) => {
          const isActive = item.id === activeId
          return (
            <motion.button
              key={item.id}
              onClick={() => {}}
              aria-pressed={isActive}
              aria-label={item.label}
              className="relative flex flex-col items-center justify-center w-10 h-10 rounded-lg transition-colors duration-200 hover:bg-white/5 focus:outline-none focus:ring-2 focus:ring-[#0D1043] focus:ring-offset-2 focus:ring-offset-[#110E18]"
              whileHover={{ scale: 1.1 }}
              whileTap={{ scale: 0.9 }}
            >
              <item.icon className={`w-5 h-5 ${isActive ? 'text-[#B6BEC7]' : 'text-[#726B75]'}`} />
              <span className={`absolute -top-8 left-1/2 -translate
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class GlassNavigationBar extends StatefulWidget {
  const GlassNavigationBar({Key? key}) : super(key: key);

  @override
  State<GlassNavigationBar> createState() => _GlassNavigationBarState;
}

class _GlassNavigationBarState extends State<GlassNavigationBar> {
  int _selectedIndex = 0;

  final List<_NavItem> _items = [
    _NavItem(icon: Icons.home, label: 'Home'),
    _NavItem(icon: Icons.favorite, label: 'Likes'),
    _NavItem(icon: Icons.add, label: 'Create'),
    _NavItem(icon: Icons.person, label: 'Profile'),
    _NavItem(icon: Icons.notifications, label: 'Alerts'),
  ];

  @override
  Widget build(BuildContext context) {
    return Positioned(
      bottom: 24,
      left: 0,
      right: 0,
      child: Center(
        child: ClipRRect(
          borderRadius: BorderRadius.circular(30),
          child: BackdropFilter(
            filter: ImageFilter.blur(sigmaX: 10, sigmaY: 10),
            child: Container(
              width: 320,
              height: 56,
              decoration: BoxDecoration(
                color: const Color(0xFF110E18).withOpacity(0.8),
                borderRadius: BorderRadius.circular(30),
                border: Border.all(color: Colors.white.withOpacity(0.1)),
                boxShadow: [
                  BoxShadow(
                    color: Colors.black.withOpacity(0.5),
                    bl
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
