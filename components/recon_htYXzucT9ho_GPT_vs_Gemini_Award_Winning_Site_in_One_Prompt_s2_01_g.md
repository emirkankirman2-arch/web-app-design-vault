---
title: "GlassMenu — htYXzucT9ho_GPT_vs_Gemini_Aw (05:09.400)"
description: "GlassMenu UI component (recon_htYXzucT9ho_GPT_vs_Gemini_Award_Winning_Site_in_One_Prompt_s2_01_g) with SSIM 0.9937, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_htYXzucT9ho_GPT_vs_Gemini_-_Award_Winning_Site_in_One_Prompt_s2_01_glassmenu"
category: "GlassMenu"
ssim: 0.9937
quality_score: 8.72
tags: [glassmenu, ui-design, design-tokens, react, flutter]
---

# GlassMenu — htYXzucT9ho_GPT_vs_Gemini_Aw (05:09.400)

> **Category:** [[03_GlassMenu|GlassMenu]] | **SSIM Fidelity:** `0.9937` | **Quality Score:** `8.72 / 10`  
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
import { Home, Heart, PlusCircle, User, Bell } from 'lucide-react';

interface GlassMenuProps {
  className?: string;
}

const tabs = [
  { id: 'home', label: 'Home', icon: Home },
  { id: 'likes', label: 'Likes', icon: Heart },
  { id: 'create', label: 'Create', icon: PlusCircle },
  { id: 'profile', label: 'Profile', icon: User },
  { id: 'alerts', label: 'Alerts', icon: Bell },
] as const;

export const GlassMenu: React.FC<GlassMenuProps> = ({ className }) => {
  const [activeTab, setActiveTab] = React.useState<'home' | 'likes' | 'create' | 'profile' | 'alerts'>('home');

  return (
    <motion.nav
      initial={{ opacity: 0, scale: 0.95 }}
      animate={{ opacity: 1, scale: 1 }}
      transition={{ type: 'spring', stiffness: 260, damping: 20 }}
      className={
        'fixed bottom-8 left-1/2 -translate-x-1/2 z-50 ' +
        'bg-black/60 backdrop-blur-xl border border-white/10 rounded-full px-4 py-2.5 shadow-2xl ' +
        'flex items-center gap-2 ' +
        (className ?? '')
      }
      aria-label="Main navigation"
    >
      {tabs.map((tab) => {
        const isActive = activeTab === tab.id;
        const Icon = tab.icon;
        return (
          <button
            key={tab.id}
            onClick={() => setActiveTab(tab.id)}
            aria-pressed={isActive}
            aria-label={tab.label}
            className={
              'relative group flex flex-col items-center justify-center w-10 h-10 rounded-full transition-all duration-200 ' +
              (isActive
                ? 'bg-
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
      left: MediaQuery.of(context).size.width / 2 - 131,
      child: AnimatedContainer(
        duration: const Duration(milliseconds: 1200),
        curve: Curves.elasticOut,
        width: 262,
        height: 59,
        decoration: BoxDecoration(
          color: Colors.black.withOpacity(0.6),
          borderRadius: BorderRadius.circular(9999),
          border: Border.all(color: Colors.white.withOpacity(0.1)),
          boxShadow: [
            BoxShadow(
              color: Colors.black.withOpacity(0.5),
              blurRadius: 50,
              spreadRadius: -12,
            ),
          ],
        ),
        child: ClipRRect(
          borderRadius: BorderRadius.circular(9999),
          child: BackdropFilter(
    
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
