---
title: "Navbar — lnXzJmFw0lQ_I_brought_androi (00:02.800)"
description: "Navbar UI component (recon_lnXzJmFw0lQ_I_brought_android_style_app_bubbles_to_the_web_s1_00_n) with SSIM 0.996, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_lnXzJmFw0lQ_I_brought_android_style_app_bubbles_to_the_web_s1_00_navbar"
category: "Navbar"
ssim: 0.996
quality_score: 8.72
tags: [navbar, ui-design, design-tokens, react, flutter]
---

# Navbar — lnXzJmFw0lQ_I_brought_androi (00:02.800)

> **Category:** [[04_Navbar|Navbar]] | **SSIM Fidelity:** `0.996` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[03_GlassMenu|GlassMenu]], [[02_Button|Button]], [[05_Hero|Hero]]

Professional Navbar reverse-engineered from lnXzJmFw0lQ_I_brought_android_style_app_bubbles_to_the_web at 00:02.800. Features FADE_IN_SCALE micro-interaction animation with 20.47:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#000000` | `rgb(0, 0, 0)` | `oklch(0.00 0.000 0.0)` | `65.6%` |
| `surface` | `#7B7D7F` | `rgb(123, 125, 127)` | `oklch(0.59 0.004 247.9)` | `2.4%` |
| `accent` | `#2164A1` | `rgb(33, 100, 161)` | `oklch(0.49 0.118 249.9)` | `0.2%` |
| `text` | `#FCFCFC` | `rgb(252, 252, 252)` | `oklch(0.99 0.000 89.9)` | `22.6%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `24.5 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.04`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
import React from 'react';
import { motion } from 'framer-motion';
import { Home, Heart, PlusCircle, User, Bell } from 'lucide-react';

interface NavItem {
  icon: React.ElementType;
  label: string;
  active: boolean;
}

const NAV_ITEMS: NavItem[] = [
  { icon: Home, label: 'Home', active: true },
  { icon: Heart, label: 'Likes', active: false },
  { icon: PlusCircle, label: 'Create', active: false },
  { icon: User, label: 'Profile', active: false },
  { icon: Bell, label: 'Alerts', active: false },
];

export default function GlassNavbar() {
  return (
    <nav className="fixed bottom-0 left-1/2 -translate-x-1/2 mb-6 z-50">
      <motion.div
        initial={{ opacity: 0, scale: 0.95 }}
        animate={{ opacity: 1, scale: 1 }}
        transition={{ type: 'spring', stiffness: 260, damping: 20 }}
        className="flex items-center justify-center gap-6 px-6 py-3 rounded-full bg-black/60 backdrop-blur-xl border border-white/10 shadow-2xl"
      >
        {NAV_ITEMS.map((item, index) => (
          <button
            key={item.label}
            aria-label={item.label}
            className="relative group"
          >
            <div className="flex flex-col items-center justify-center w-10 h-10 rounded-full transition-all duration-300"
                 style={{ backgroundColor: item.active ? 'rgba(33, 100, 161, 0.2)' : 'transparent' }}
            >
              <item.icon
                className={`w-5 h-5 transition-colors duration-300 ${item.active ? 'text-blue-400' : 'text-gray-400 group-hover:text-white'}`}
   
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class GlassNavbar extends StatefulWidget {
  const GlassNavbar({super.key});

  @override
  State<GlassNavbar> createState() => _GlassNavbarState;
}

class _GlassNavbarState extends State<GlassNavbar> {
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
          borderRadius: BorderRadius.circular(30),
          child: BackdropFilter(
            filter: ImageFilter.blur(sigmaX: 12, sigmaY: 12),
            child: Container(
              margin: const EdgeInsets.symmetric(horizontal: 24),
              padding: const EdgeInsets.symmetric(vertical: 12, horizontal: 24),
              decoration: BoxDecoration(
                color: Colors.black.withOpacity(0.6),
                borderRadius: BorderRadius.circular(30),
                border: Border.all(color: Colors.white.withOpacity(0.1)),
                boxShadow: [
                  BoxShadow(
                    color: Colors.black.withOpacity(0.5)
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
