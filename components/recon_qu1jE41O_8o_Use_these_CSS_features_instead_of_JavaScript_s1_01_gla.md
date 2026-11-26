---
title: "GlassMenu — qu1jE41O_8o_Use_these_CSS_fe (00:00.000)"
description: "GlassMenu UI component (recon_qu1jE41O_8o_Use_these_CSS_features_instead_of_JavaScript_s1_01_gla) with SSIM 0.9889, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_qu1jE41O_8o_Use_these_CSS_features_instead_of_JavaScript_s1_01_glassmenu"
category: "GlassMenu"
ssim: 0.9889
quality_score: 8.72
tags: [glassmenu, ui-design, design-tokens, react, flutter]
---

# GlassMenu — qu1jE41O_8o_Use_these_CSS_fe (00:00.000)

> **Category:** [[03_GlassMenu|GlassMenu]] | **SSIM Fidelity:** `0.9889` | **Quality Score:** `8.72 / 10`  
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
    <nav
      aria-label="Main navigation"
      className="fixed bottom-8 left-1/2 -translate-x-1/2 z-50"
    >
      <motion.div
        initial={{ opacity: 0, scale: 0.95 }}
        animate={{ opacity: 1, scale: 1 }}
        transition={{ type: 'spring', stiffness: 260, damping: 20 }}
        className="flex items-center gap-1 px-3 py-2 rounded-full bg-[#140F15]/80 backdrop-blur-xl border border-white/10 shadow-2xl"
      >
        {tabs.map((tab) => (
          <button
            key={tab.id}
            onClick={() => onTabChange?.(tab.id)}
            aria-pressed={activeTab === tab.id}
            aria-label={tab.label}
            className={
              'flex flex-col items-center justify-center w-10 h-10 rounded-xl transition-all duration-200 ease-out ' +
              (activeTab === tab.id
                ? 'bg-[#5C4152] text-[#339EF0] shadow-[0_0_15px_rgba(51,158,240,0.4)]'
                : 'text-[#5C4152] hover:bg-white/10 hover:text-white')
            }
          >
            <span className="text-lg">{tab.icon}</span>
            <span className="
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class GlassMenu extends StatefulWidget {
  const GlassMenu({Key? key}) : super(key: key);

  @override
  State<GlassMenu> createState() => _GlassMenuState;
}

class _GlassMenuState extends State<GlassMenu> {
  String _activeTab = 'home';

  final List<Map<String, String>> _tabs = [
    {'id': 'home', 'label': 'Home', 'icon': '🏠'},
    {'id': 'likes', 'label': 'Likes', 'icon': '❤️'},
    {'id': 'create', 'label': 'Create', 'icon': '✨'},
    {'id': 'profile', 'label': 'Profile', 'icon': '👤'},
    {'id': 'alerts', 'label': 'Alerts', 'icon': '🔔'},
  ];

  @override
  Widget build(BuildContext context) {
    return Positioned(
      bottom: 32,
      left: MediaQuery.of(context).size.width / 2 - 72.5,
      child: ClipRRect(
        borderRadius: BorderRadius.circular(30),
        child: BackdropFilter(
          filter: ImageFilter.blur(sigmaX: 12, sigmaY: 12),
          child: Container(
            width: 145,
            height: 59,
            decoration: BoxDecoration(
              color: const Color(0x140F15).withOpacity(0.8),
              borderRadius: BorderRadius.circular(30),
              border: Border.all(color: Colors.white.withOpacity(0.1)),
              boxShadow: [
                BoxShadow(
                  color: Colors.black.withOpacity(0.5),
                  blurRadius: 25,
                  spreadRadius: -12,
     
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
