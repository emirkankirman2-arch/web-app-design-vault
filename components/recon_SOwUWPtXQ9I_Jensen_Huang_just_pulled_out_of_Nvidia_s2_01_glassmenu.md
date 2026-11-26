---
title: "GlassMenu — SOwUWPtXQ9I_Jensen_Huang_jus (02:42.500)"
description: "GlassMenu UI component (recon_SOwUWPtXQ9I_Jensen_Huang_just_pulled_out_of_Nvidia_s2_01_glassmenu) with SSIM 0.993, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_SOwUWPtXQ9I_Jensen_Huang_just_pulled_out_of_Nvidia..._s2_01_glassmenu"
category: "GlassMenu"
ssim: 0.993
quality_score: 8.72
tags: [glassmenu, ui-design, design-tokens, react, flutter]
---

# GlassMenu — SOwUWPtXQ9I_Jensen_Huang_jus (02:42.500)

> **Category:** [[03_GlassMenu|GlassMenu]] | **SSIM Fidelity:** `0.993` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[04_Navbar|Navbar]], [[01_Card|Card]], [[10_ShaderCanvas|ShaderCanvas]]

Professional GlassMenu reverse-engineered from SOwUWPtXQ9I_Jensen_Huang_just_pulled_out_of_Nvidia... at 02:42.500. Features FADE_IN_SCALE micro-interaction animation with 19.46:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#FEFEFE` | `rgb(254, 254, 254)` | `oklch(1.00 0.000 89.9)` | `49.1%` |
| `surface` | `#DCDADA` | `rgb(220, 218, 218)` | `oklch(0.89 0.002 17.2)` | `6.6%` |
| `accent` | `#E55807` | `rgb(229, 88, 7)` | `oklch(0.64 0.190 42.1)` | `1.8%` |
| `text` | `#0B0C07` | `rgb(11, 12, 7)` | `oklch(0.15 0.011 116.4)` | `32.5%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `25.833 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `2.26`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React, { useState } from 'react';
import { motion } from 'framer-motion';

// Icons: Home, Likes, Create, Profile, Alerts
const TABS = [
  { id: 'home', label: 'Home', icon: 'M3 9l9-7 9 7v11a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z' },
  { id: 'likes', label: 'Likes', icon: 'M20.84 4.61a5.5 5.5 0 0 0-7.78 0L12 5.67l-1.06-1.06a5.5 5.5 0 0 0-7.78 7.78l1.06 1.06L12 21.23l7.78-7.78 1.06-1.06a5.5 5.5 0 0 0 0-7.78z' },
  { id: 'create', label: 'Create', isRaised: true },
  { id: 'profile', label: 'Profile', icon: 'M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2 M12 3a4 4 0 1 0 0 8 4 4 0 0 0 0-8z' },
  { id: 'alerts', label: 'Alerts', icon: 'M18 8A6 6 0 0 0 6 8c0 7-3 9-3 9h18s-3-2-3-9' },
];

export const GlassmenuWidget: React.FC = () => {
  const [activeTab, setActiveTab] = useState('create');

  return (
    <div className="relative flex items-center gap-3 px-5 py-3 rounded-full border border-teal-500/30 bg-[#072528]/80 backdrop-blur-2xl shadow-[0_20px_50px_rgba(0,0,0,0.6),0_0_30px_rgba(45,212,191,0.2)]">
      {TABS.map((tab) => {
        const isActive = activeTab === tab.id;
        return (
          <button
            key={tab.id}
            onClick={() => setActiveTab(tab.id)}
            className="relative z-10 flex flex-col items-center justify-center w-16 h-14 rounded-full transition-colors text-slate-400 hover:text-white"
          >
            {isActive && (
              <motion.div
                layoutId="activeTabIndicator"
                className="absolute inset-0 bg-teal-400/20 border border-teal-400/40 rounded-full shadow-[0_0_20px_rgba(45,212,191,0.5)]"
       
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class GlassmenuWidget extends StatefulWidget {
  const GlassmenuWidget({super.key});

  @override
  State<GlassmenuWidget> createState() => _GlassmenuWidgetState();
}

class _GlassmenuWidgetState extends State<GlassmenuWidget> {
  int _currentIndex = 2; // Create active

  @override
  Widget build(BuildContext context) {
    return Container(
      decoration: BoxDecoration(
        color: const Color(0xCC072528),
        borderRadius: BorderRadius.circular(32),
        border: Border.all(color: const Color(0x4D2DD4BF)),
        boxShadow: const [
          BoxShadow(color: Colors.black54, blurRadius: 24, offset: Offset(0, 10)),
        ],
      ),
      padding: const EdgeInsets.symmetric(horizontal: 16, vertical: 8),
      child: Row(
        mainAxisSize: MainAxisSize.min,
        children: [
          _buildItem(0, Icons.home_outlined, 'Home'),
          _buildItem(1, Icons.favorite_border, 'Likes'),
          _buildItem(2, Icons.add_circle_outline, 'Create'),
          _buildItem(3, Icons.person_outline, 'Profile'),
          _buildItem(4, Icons.notifications_none, 'Alerts'),
        ],
      ),
    );
  }

  Widget _buildItem(int index, IconData icon, String label) {
    final isSelected = _currentIndex == index;
    return GestureDetector(
      onTap: () => setState(() => _currentIndex = index),
      child: AnimatedContainer(
  
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
