---
title: "Navbar — DelPxS3oFRd_Video_by_wearepi (00:00.000)"
description: "Navbar UI component (recon_DelPxS3oFRd_Video_by_wearepixelflow_s1_00_navbar) with SSIM 0.9902, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_DelPxS3oFRd_Video_by_wearepixelflow_s1_00_navbar"
category: "Navbar"
ssim: 0.9902
quality_score: 8.72
tags: [navbar, ui-design, design-tokens, react, flutter]
---

# Navbar — DelPxS3oFRd_Video_by_wearepi (00:00.000)

> **Category:** [[04_Navbar|Navbar]] | **SSIM Fidelity:** `0.9902` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[03_GlassMenu|GlassMenu]], [[02_Button|Button]], [[05_Hero|Hero]]

Professional Navbar reverse-engineered from DelPxS3oFRd_Video_by_wearepixelflow at 00:00.000. Features FADE_IN_SCALE micro-interaction animation with 16.01:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#DCE4CC` | `rgb(220, 228, 204)` | `oklch(0.91 0.033 122.1)` | `48.1%` |
| `surface` | `#FDFDFD` | `rgb(253, 253, 253)` | `oklch(0.99 0.000 89.9)` | `2.4%` |
| `accent` | `#163F2E` | `rgb(22, 63, 46)` | `oklch(0.33 0.055 163.3)` | `2.2%` |
| `text` | `#000000` | `rgb(0, 0, 0)` | `oklch(0.00 0.000 0.0)` | `42.4%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `6.0 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
import React from 'react';
import { motion } from 'framer-motion';
import { Home, Heart, Plus, User, Bell } from 'lucide-react';

interface NavbarProps {
  activeTab?: 'home' | 'likes' | 'create' | 'profile' | 'alerts';
  onTabChange?: (tab: string) => void;
}

const Navbar: React.FC<NavbarProps> = ({ activeTab = 'home', onTabChange }) => {
  const tabs = [
    { id: 'home', label: 'Home', icon: <Home size={20} /> },
    { id: 'likes', label: 'Likes', icon: <Heart size={20} /> },
    { id: 'create', label: 'Create', icon: <Plus size={20} /> },
    { id: 'profile', label: 'Profile', icon: <User size={20} /> },
    { id: 'alerts', label: 'Alerts', icon: <Bell size={20} /> },
  ];

  return (
    <nav
      className="fixed bottom-0 left-1/2 -translate-x-1/2 z-50 w-[303px] h-[56px] bg-white/80 backdrop-blur-md border border-white/20 rounded-none shadow-lg"
      aria-label="Main navigation"
    >
      <motion.div
        initial={{ opacity: 0, scale: 0.95 }}
        animate={{ opacity: 1, scale: 1 }}
        transition={{ type: 'spring', stiffness: 260, damping: 20 }}
        className="flex items-center justify-center h-full gap-1 px-2"
      >
        {tabs.map((tab) => {
          const isActive = activeTab === tab.id;
          return (
            <button
              key={tab.id}
              onClick={() => onTabChange?.(tab.id)}
              aria-pressed={isActive}
              aria-label={tab.label}
              className={
                'relative flex flex-col items-center justify-center w-1/5 h-full transitio
```

## 4. Flutter / Dart Implementation

```dart
// Flutter Material widget template
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
