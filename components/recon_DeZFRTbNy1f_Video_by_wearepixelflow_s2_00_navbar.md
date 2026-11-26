---
title: "Navbar — DeZFRTbNy1f_Video_by_wearepi (00:06.533)"
description: "Navbar UI component (recon_DeZFRTbNy1f_Video_by_wearepixelflow_s2_00_navbar) with SSIM 0.9917, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_DeZFRTbNy1f_Video_by_wearepixelflow_s2_00_navbar"
category: "Navbar"
ssim: 0.9917
quality_score: 8.72
tags: [navbar, ui-design, design-tokens, react, flutter]
---

# Navbar — DeZFRTbNy1f_Video_by_wearepi (00:06.533)

> **Category:** [[04_Navbar|Navbar]] | **SSIM Fidelity:** `0.9917` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[03_GlassMenu|GlassMenu]], [[02_Button|Button]], [[05_Hero|Hero]]

Professional Navbar reverse-engineered from DeZFRTbNy1f_Video_by_wearepixelflow at 00:06.533. Features FADE_IN_SCALE micro-interaction animation with 20.47:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#000000` | `rgb(0, 0, 0)` | `oklch(0.00 0.000 0.0)` | `55.6%` |
| `surface` | `#49494E` | `rgb(73, 73, 78)` | `oklch(0.41 0.008 286.0)` | `18.8%` |
| `accent` | `#4F535B` | `rgb(79, 83, 91)` | `oklch(0.44 0.014 264.4)` | `5.0%` |
| `text` | `#FCFCFC` | `rgb(252, 252, 252)` | `oklch(0.99 0.000 89.9)` | `3.4%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `13.533 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
import React from 'react';
import { motion, AnimatePresence } from 'framer-motion';

interface NavItem {
  id: string;
  label: string;
  icon: React.ReactNode;
}

const NAV_ITEMS: NavItem[] = [
  { id: 'home', label: 'Home', icon: <svg className="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path strokeLinecap="round" strokeLinejoin="round" strokeWidth={2} d="M3 12l2-2m0 0l7-7 7 7M5 10v10a1 1 0 001 1h3m10-11l2 2m-2-2v10a1 1 0 01-1 1h-3m-6 0a1 1 0 001-1v-4a1 1 0 011-1h2a1 1 0 011 1v4a1 1 0 001 1m-6 0h6"></path></svg> },
  { id: 'likes', label: 'Likes', icon: <svg className="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path strokeLinecap="round" strokeLinejoin="round" strokeWidth={2} d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z"></path></svg> },
  { id: 'create', label: 'Create', icon: <svg className="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path strokeLinecap="round" strokeLinejoin="round" strokeWidth={2} d="M12 6v6m0 0v6m0-6h6m-6 0H6"></path></svg> },
  { id: 'profile', label: 'Profile', icon: <svg className="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path strokeLinecap="round" strokeLinejoin="round" strokeWidth={2} d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z"></path></svg> },
  { id: 'alerts', label: 'Alerts', icon: <svg className="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path strokeLinecap="round" strokeLinejoin
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
      bottom: 24,
      left: MediaQuery.of(context).size.width / 2 - 169,
      child: ClipRRect(
        borderRadius: BorderRadius.circular(30),
        child: BackdropFilter(
          filter: ImageFilter.blur(sigmaX: 8, sigmaY: 8),
          child: Container(
            width: 338,
            height: 61,
            decoration: BoxDecoration(
              color: const Color(0xFF49494E).withOpacity(0.8),
              border: Border.all(color: Colors.white.withOpacity(0.1)),
              borderRadius: BorderRadius.circular(30),
              boxShadow: [
                BoxShadow(
                  color: Colors.black.withOpacity(0.5),
                  blurRadius: 25,
                  spreadRadius: -12,
          
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
