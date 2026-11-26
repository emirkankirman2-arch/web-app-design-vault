---
title: "Navbar — lnXzJmFw0lQ_I_brought_androi (01:12.100)"
description: "Navbar UI component (recon_lnXzJmFw0lQ_I_brought_android_style_app_bubbles_to_the_web_s2_01_n) with SSIM 0.9907, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_lnXzJmFw0lQ_I_brought_android_style_app_bubbles_to_the_web_s2_01_navbar"
category: "Navbar"
ssim: 0.9907
quality_score: 8.72
tags: [navbar, ui-design, design-tokens, react, flutter]
---

# Navbar — lnXzJmFw0lQ_I_brought_androi (01:12.100)

> **Category:** [[04_Navbar|Navbar]] | **SSIM Fidelity:** `0.9907` | **Quality Score:** `8.72 / 10`  
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
import React from 'react';
import { motion } from 'framer-motion';
import { Home, Heart, Plus, User, Bell } from 'lucide-react';

interface NavItem {
  icon: React.ElementType;
  label: string;
  active: boolean;
}

const NAV_ITEMS: NavItem[] = [
  { icon: Home, label: 'Home', active: true },
  { icon: Heart, label: 'Likes', active: false },
  { icon: Plus, label: 'Create', active: false },
  { icon: User, label: 'Profile', active: false },
  { icon: Bell, label: 'Alerts', active: false },
];

export default function GlassNavbar() {
  return (
    <nav className="fixed bottom-8 left-1/2 -translate-x-1/2 z-50">
      <motion.div
        initial={{ opacity: 0, scale: 0.95 }}
        animate={{ opacity: 1, scale: 1 }}
        transition={{ type: 'spring', stiffness: 260, damping: 20 }}
        className="flex items-center gap-2 px-6 py-3 rounded-full bg-black/60 backdrop-blur-xl border border-white/10 shadow-2xl"
        aria-label="Main navigation"
      >
        {NAV_ITEMS.map((item, index) => (
          <button
            key={item.label}
            className={
              'relative flex flex-col items-center justify-center w-10 h-10 rounded-full transition-all duration-300 ' +
              (item.active
                ? 'bg-white/10 text-white shadow-[0_0_15px_rgba(38,202,87,0.4)]'
                : 'text-gray-400 hover:text-white hover:bg-white/5')
            }
            aria-pressed={item.active}
            aria-label={item.label}
          >
            <item.icon className="w-5 h-5" />
            <span clas
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

  final List<_NavItem> _items = const [
    _NavItem(icon: Icons.home, label: 'Home'),
    _NavItem(icon: Icons.favorite, label: 'Likes'),
    _NavItem(icon: Icons.add, label: 'Create'),
    _NavItem(icon: Icons.person, label: 'Profile'),
    _NavItem(icon: Icons.notifications, label: 'Alerts'),
  ];

  @override
  Widget build(BuildContext context) {
    return Positioned(
      bottom: 32,
      left: 0,
      right: 0,
      child: Center(
        child: ClipRRect(
          borderRadius: BorderRadius.circular(28),
          child: BackdropFilter(
            filter: ImageFilter.blur(sigmaX: 12, sigmaY: 12),
            child: Container(
              width: 979,
              height: 72,
              decoration: BoxDecoration(
                color: Colors.black.withOpacity(0.6),
                borderRadius: BorderRadius.circular(28),
                border: Border.all(color: Colors.white.withOpacity(0.1)),
                boxShadow: [
                  BoxShadow(
                    color: Colors.black.withOpacity(0.5),
                    blurRadius: 25,
                    spreadRadius: -12,
           
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
