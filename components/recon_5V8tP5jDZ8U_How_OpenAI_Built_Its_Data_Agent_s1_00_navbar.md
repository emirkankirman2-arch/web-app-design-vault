---
title: "Navbar — 5V8tP5jDZ8U_How_OpenAI_Built (00:00.000)"
description: "Navbar UI component (recon_5V8tP5jDZ8U_How_OpenAI_Built_Its_Data_Agent_s1_00_navbar) with SSIM 0.9943, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_5V8tP5jDZ8U_How_OpenAI_Built_Its_Data_Agent_s1_00_navbar"
category: "Navbar"
ssim: 0.9943
quality_score: 8.72
tags: [navbar, ui-design, design-tokens, react, flutter]
---

# Navbar — 5V8tP5jDZ8U_How_OpenAI_Built (00:00.000)

> **Category:** [[04_Navbar|Navbar]] | **SSIM Fidelity:** `0.9943` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[03_GlassMenu|GlassMenu]], [[02_Button|Button]], [[05_Hero|Hero]]

Professional Navbar reverse-engineered from 5V8tP5jDZ8U_How_OpenAI_Built_Its_Data_Agent at 00:00.000. Features FADE_IN_SCALE micro-interaction animation with 14.26:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#6EECB7` | `rgb(110, 236, 183)` | `oklch(0.86 0.137 163.4)` | `47.6%` |
| `surface` | `#FDFDFD` | `rgb(253, 253, 253)` | `oklch(0.99 0.000 89.9)` | `20.5%` |
| `accent` | `#F6CE94` | `rgb(246, 206, 148)` | `oklch(0.87 0.087 76.5)` | `1.3%` |
| `text` | `#010101` | `rgb(1, 1, 1)` | `oklch(0.07 0.000 89.9)` | `16.7%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `55.055 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.0`

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

export default function Navbar() {
  return (
    <nav className="fixed top-0 left-0 w-full z-50">
      <motion.div
        initial={{ opacity: 0, scale: 0.95 }}
        animate={{ opacity: 1, scale: 1 }}
        transition={{ type: 'spring', stiffness: 260, damping: 20 }}
        className="mx-auto max-w-[1172px] h-[118px] bg-white/80 backdrop-blur-md border-b border-black/10 flex items-center justify-between px-6 py-4 shadow-lg"
      >
        <div className="flex items-center gap-3">
          <div className="w-2 h-12 rounded-full bg-[#6EECB7]" />
          <h1 className="text-3xl font-bold text-black tracking-tight">
            How OpenAI Built Its Data Agent
          </h1>
        </div>
        <div className="flex items-center gap-6">
          {NAV_ITEMS.map((item) => (
            <button
              key={item.label}
              className={
                'flex flex-col items-center justify-center gap-1.5 p-2 rounded-lg transition-all duration-200 ' +
                (item.active
                  ? 'bg-[#F6CE94] tex
```

## 4. Flutter / Dart Implementation

```dart
// Flutter StatefulWidget
import 'package:flutter/material.dart';

class Navbar extends StatefulWidget {
  const Navbar({super.key});

  @override
  State<Navbar> createState() => _NavbarState();
}

class _NavbarState extends State<Navbar> {
  int _selectedIndex = 0;

  final List<Map<String, dynamic>> _items = [
    {'icon': Icons.home, 'label': 'Home'},
    {'icon': Icons.favorite, 'label': 'Likes'},
    {'icon': Icons.add, 'label': 'Create'},
    {'icon': Icons.person, 'label': 'Profile'},
    {'icon': Icons.notifications, 'label': 'Alerts'},
  ];

  @override
  Widget build(BuildContext context) {
    return Positioned.fill(
      child: Align(
        alignment: Alignment.topCenter,
        child: AnimatedContainer(
          duration: const Duration(milliseconds: 550),
          curve: Curves.easeOut,
          width: 1172,
          height: 118,
          decoration: BoxDecoration(
            color: Colors.white.withOpacity(0.8),
            border: Border(bottom: BorderSide(color: Colors.black.withOpacity(0.1))),
            boxShadow: [
              BoxShadow(
                color: Colors.black.withOpacity(0.1),
                blurRadius: 15,
                offset: const Offset(0, 5),
              ),
            ],
          ),
          child: ClipRect(
            child: BackdropFilter(
              filter: ImageFilter.blur(sigmaX: 12, sigmaY: 12),
           
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
