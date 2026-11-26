---
title: "GlassMenu — htYXzucT9ho_GPT_vs_Gemini_Aw (05:09.400)"
description: "GlassMenu UI component (recon_htYXzucT9ho_GPT_vs_Gemini_Award_Winning_Site_in_One_Prompt_s2_02_g) with SSIM 0.994, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_htYXzucT9ho_GPT_vs_Gemini_-_Award_Winning_Site_in_One_Prompt_s2_02_glassmenu"
category: "GlassMenu"
ssim: 0.994
quality_score: 8.72
tags: [glassmenu, ui-design, design-tokens, react, flutter]
---

# GlassMenu — htYXzucT9ho_GPT_vs_Gemini_Aw (05:09.400)

> **Category:** [[03_GlassMenu|GlassMenu]] | **SSIM Fidelity:** `0.994` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[04_Navbar|Navbar]], [[01_Card|Card]], [[10_ShaderCanvas|ShaderCanvas]]

Professional GlassMenu reverse-engineered from htYXzucT9ho_GPT_vs_Gemini_-_Award_Winning_Site_in_One_Prompt at 05:09.400. Features FADE_IN_SCALE micro-interaction animation with 8.89:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#000000` | `rgb(0, 0, 0)` | `oklch(0.00 0.000 0.0)` | `58.7%` |
| `surface` | `#AAA8AA` | `rgb(170, 168, 170)` | `oklch(0.73 0.004 325.6)` | `2.5%` |
| `accent` | `#961C8A` | `rgb(150, 28, 138)` | `oklch(0.48 0.193 332.8)` | `0.3%` |
| `text` | `#AAA8AA` | `rgb(170, 168, 170)` | `oklch(0.73 0.004 325.6)` | `2.5%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `121.8 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.02`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react';
import { motion } from 'framer-motion';

interface GlassMenuProps {
  className?: string;
}

const tabs = [
  { id: 'home', label: 'Home', icon: '🏠' },
  { id: 'likes', label: 'Likes', icon: '❤️' },
  { id: 'create', label: 'Create', icon: '✨' },
  { id: 'profile', label: 'Profile', icon: '👤' },
  { id: 'alerts', label: 'Alerts', icon: '🔔' },
];

export const GlassMenu: React.FC<GlassMenuProps> = ({ className }) => {
  const [activeTab, setActiveTab] = React.useState<string>('home');

  return (
    <nav
      className={
        'fixed bottom-8 left-1/2 -translate-x-1/2 z-50 ' +
        'bg-black/40 backdrop-blur-xl border border-white/10 rounded-full px-4 py-2 flex items-center gap-2 shadow-2xl ' +
        (className || '')
      }
      aria-label="Main navigation"
    >
      <motion.div
        initial={{ opacity: 0, scale: 0.95 }}
        animate={{ opacity: 1, scale: 1 }}
        transition={{ type: 'spring', stiffness: 260, damping: 20 }}
      >
        {tabs.map((tab) => (
          <button
            key={tab.id}
            onClick={() => setActiveTab(tab.id)}
            aria-pressed={activeTab === tab.id}
            aria-label={tab.label}
            className={
              'relative group flex flex-col items-center justify-center w-10 h-10 rounded-full transition-all duration-200 ' +
              (activeTab === tab.id
                ? 'bg-white/10 text-white shadow-[0_0_15px_rgba(150,28,138,0.4)]'
                : 'text-gray-400 hover:text-white hover:bg-white/5')
            }
          >
            <span className="text-lg
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class GlassMenu extends StatefulWidget {
  const GlassMenu({Key? key}) : super(key: key);

  @override
  State<GlassMenu> createState() => _GlassMenuState();
}

class _GlassMenuState extends State<GlassMenu> {
  int _selectedIndex = 0;

  final List<Map<String, dynamic>> _tabs = [
    {'icon': Icons.home, 'label': 'Home'},
    {'icon': Icons.favorite, 'label': 'Likes'},
    {'icon': Icons.add_circle, 'label': 'Create'},
    {'icon': Icons.person, 'label': 'Profile'},
    {'icon': Icons.notifications, 'label': 'Alerts'},
  ];

  @override
  Widget build(BuildContext context) {
    return Positioned(
      bottom: 32,
      left: 0,
      right: 0,
      child: Center(
        child: ClipRRect(
          borderRadius: BorderRadius.circular(30),
          child: BackdropFilter(
            filter: ImageFilter.blur(sigmaX: 12, sigmaY: 12),
            child: Container(
              width: 320,
              height: 56,
              decoration: BoxDecoration(
                color: Colors.black.withOpacity(0.4),
                borderRadius: BorderRadius.circular(30),
                border: Border.all(color: Colors.white.withOpacity(0.1)),
                boxShadow: [
                  BoxShadow(
                    color: Colors.black.withOpacity(0.5),
                    blurRadius: 25,
                    spreadRadius: -12,
            
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
