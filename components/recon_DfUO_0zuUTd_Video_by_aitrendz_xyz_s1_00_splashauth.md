---
title: "SplashAuth — DfUO_0zuUTd_Video_by_aitrend (00:00.000)"
description: "SplashAuth UI component (recon_DfUO_0zuUTd_Video_by_aitrendz_xyz_s1_00_splashauth) with SSIM 0.9794, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_DfUO-0zuUTd_Video_by_aitrendz.xyz_s1_00_splashauth"
category: "SplashAuth"
ssim: 0.9794
quality_score: 8.72
tags: [splashauth, ui-design, design-tokens, react, flutter]
---

# SplashAuth — DfUO_0zuUTd_Video_by_aitrend (00:00.000)

> **Category:** [[09_SplashAuth|SplashAuth]] | **SSIM Fidelity:** `0.9794` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[06_Input|Input]], [[07_LockScreen|LockScreen]], [[05_Hero|Hero]]

Professional SplashAuth reverse-engineered from DfUO-0zuUTd_Video_by_aitrendz.xyz at 00:00.000. Features FADE_IN_SCALE micro-interaction animation with 11.48:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#10121E` | `rgb(16, 18, 30)` | `oklch(0.19 0.025 276.4)` | `19.9%` |
| `surface` | `#9B8976` | `rgb(155, 137, 118)` | `oklch(0.64 0.035 68.7)` | `13.4%` |
| `accent` | `#DD956E` | `rgb(221, 149, 110)` | `oklch(0.73 0.102 49.1)` | `11.2%` |
| `text` | `#E3C5B7` | `rgb(227, 197, 183)` | `oklch(0.85 0.039 46.6)` | `3.6%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `5.967 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `2.31`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react';
import { motion } from 'framer-motion';
import { Home, Heart, Plus, User, Bell } from 'lucide-react';

interface SplashAuthProps {
  className?: string;
}

export const SplashAuth: React.FC<SplashAuthProps> = ({ className }) => {
  const navItems = [
    { icon: <Home size={20} />, label: 'Home', active: true },
    { icon: <Heart size={20} />, label: 'Likes', active: false },
    { icon: <Plus size={20} />, label: 'Create', active: false },
    { icon: <User size={20} />, label: 'Profile', active: false },
    { icon: <Bell size={20} />, label: 'Alerts', active: false },
  ];

  return (
    <motion.div
      initial={{ opacity: 0, scale: 0.95 }}
      animate={{ opacity: 1, scale: 1 }}
      transition={{ type: 'spring', stiffness: 260, damping: 20 }}
      className={
        'fixed bottom-8 left-1/2 -translate-x-1/2 w-[294px] h-[275px] rounded-[28px] bg-[#10121E] p-6 shadow-none flex flex-col items-center justify-center z-50 ' +
        (className || '')
      }
    >
      <nav className="w-full h-full flex flex-col items-center justify-center gap-4">
        <div className="w-full flex justify-between px-4">
          {navItems.map((item, index) => (
            <button
              key={index}
              className={
                'flex flex-col items-center justify-center gap-1.5 p-2 rounded-full transition-all duration-200 ' +
                (item.active
                  ? 'bg-[#9B8976] text-[#DD956E] shadow-[0_0_15px_rgba(221,149,110,0.4)]'
                  : 'text-[#E3C5B7] hover:bg-[#1A1D2E] hover:text-[#DD956E]')
             
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class SplashAuth extends StatefulWidget {
  const SplashAuth({Key? key}) : super(key: key);

  @override
  State<SplashAuth> createState() => _SplashAuthState;
}

class _SplashAuthState extends State<SplashAuth> with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scaleAnimation;
  late Animation<double> _opacityAnimation;

  int _selectedIndex = 0;

  final List<Map<String, dynamic>> _navItems = [
    {'icon': Icons.home, 'label': 'Home'},
    {'icon': Icons.favorite, 'label': 'Likes'},
    {'icon': Icons.add, 'label': 'Create'},
    {'icon': Icons.person, 'label': 'Profile'},
    {'icon': Icons.notifications, 'label': 'Alerts'},
  ];

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 5966),
    );
    _scaleAnimation = Tween<double>(begin: 0.95, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOut),
    );
    _opacityAnimation = Tween<double>(begin: 0.0, end: 1.0).animate(
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
      anim
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
