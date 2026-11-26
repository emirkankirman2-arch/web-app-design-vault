---
title: "Navbar — bF28LFPjFsI_How_the_JVM_Actu (00:00.000)"
description: "Navbar UI component (recon_bF28LFPjFsI_How_the_JVM_Actually_Works_s1_00_navbar) with SSIM 0.994, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_bF28LFPjFsI_How_the_JVM_Actually_Works_s1_00_navbar"
category: "Navbar"
ssim: 0.994
quality_score: 8.72
tags: [navbar, ui-design, design-tokens, react, flutter]
---

# Navbar — bF28LFPjFsI_How_the_JVM_Actu (00:00.000)

> **Category:** [[04_Navbar|Navbar]] | **SSIM Fidelity:** `0.994` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[03_GlassMenu|GlassMenu]], [[02_Button|Button]], [[05_Hero|Hero]]

Professional Navbar reverse-engineered from bF28LFPjFsI_How_the_JVM_Actually_Works at 00:00.000. Features FADE_IN_SCALE micro-interaction animation with 11.75:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#2D2D2E` | `rgb(45, 45, 46)` | `oklch(0.30 0.002 286.3)` | `50.2%` |
| `surface` | `#4C4B4B` | `rgb(76, 75, 75)` | `oklch(0.41 0.001 17.2)` | `15.6%` |
| `accent` | `#8E6F3E` | `rgb(142, 111, 62)` | `oklch(0.56 0.077 77.6)` | `2.8%` |
| `text` | `#EDEDED` | `rgb(237, 237, 237)` | `oklch(0.95 0.000 89.9)` | `0.7%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `71.0 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `0.42`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react'
import { motion } from 'framer-motion'

interface NavItem {
  id: string
  label: string
  icon: React.ReactNode
}

const NAV_ITEMS: NavItem[] = [
  { id: 'home', label: 'Home', icon: <span className="sr-only">Home</span> }, // Placeholder for SVG icons
  { id: 'likes', label: 'Likes', icon: <span className="sr-only">Likes</span> },
  { id: 'create', label: 'Create', icon: <span className="sr-only">Create</span> },
  { id: 'profile', label: 'Profile', icon: <span className="sr-only">Profile</span> },
  { id: 'alerts', label: 'Alerts', icon: <span className="sr-only">Alerts</span> },
]

export default function GlassNavbar({ activeId = 'home' }: { activeId?: string }) {
  return (
    <nav
      className="fixed bottom-0 left-0 w-full z-50"
      aria-label="Main Navigation"
    >
      <motion.div
        initial={{ opacity: 0, scale: 0.95 }}
        animate={{ opacity: 1, scale: 1 }}
        transition={{ type: 'spring', stiffness: 260, damping: 20 }}
        className="mx-auto w-[674px] h-[118px] bg-[#2D2D2E]/80 backdrop-blur-md border border-white/10 rounded-none shadow-2xl flex items-center justify-center gap-1"
      >
        {NAV_ITEMS.map((item) => (
          <button
            key={item.id}
            className={
              'relative flex flex-col items-center justify-center w-12 h-12 transition-all duration-200 ease-out rounded-lg ' +
              (activeId === item.id
                ? 'bg-[#8E6F3E] text-white shadow-[0_0_15px_rgba(142,111,62,0.6)]'
                : 'text-[#EDEDED]/70 hover:text-white hover:bg-white/10')
         
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class GlassNavbar extends StatefulWidget {
  const GlassNavbar({Key? key}) : super(key: key);

  @override
  State<GlassNavbar> createState() => _GlassNavbarState();
}

class _GlassNavbarState extends State<GlassNavbar> {
  int _selectedIndex = 0;

  final List<String> _titles = const ['Home', 'Likes', 'Create', 'Profile', 'Alerts'];

  @override
  Widget build(BuildContext context) {
    return Positioned(
      bottom: 0,
      left: 0,
      right: 0,
      child: SizedBox(
        width: 674,
        height: 118,
        child: ClipRect(
          child: BackdropFilter(
            filter: ImageFilter.blur(sigmaX: 12, sigmaY: 12),
            child: Container(
              width: 674,
              height: 118,
              decoration: BoxDecoration(
                color: const Color(0xFF2D2D2E).withOpacity(0.8),
                border: Border.all(color: Colors.white.withOpacity(0.1)),
                boxShadow: [
                  BoxShadow(
                    color: Colors.black.withOpacity(0.5),
                    blurRadius: 25,
                    spreadRadius: -12,
                  ),
                ],
              ),
              child: Row(
                mainAxisAlignment: MainAxisAlignment.center,
                children: List.generate(_titles.length, (index) {
                  final isSelected = _selectedIndex 
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
