---
title: "GlassMenu — SdumUqJ3EN0_Elevenlabs_MCP_C (00:00.000)"
description: "GlassMenu UI component (recon_SdumUqJ3EN0_Elevenlabs_MCP_Claude_is_the_Ultimate_Creative_Unlock_) with SSIM 0.9883, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_SdumUqJ3EN0_Elevenlabs_MCP_+_Claude_is_the_Ultimate_Creative_Unlock_s1_03_glassmenu"
category: "GlassMenu"
ssim: 0.9883
quality_score: 8.72
tags: [glassmenu, ui-design, design-tokens, react, flutter]
---

# GlassMenu — SdumUqJ3EN0_Elevenlabs_MCP_C (00:00.000)

> **Category:** [[03_GlassMenu|GlassMenu]] | **SSIM Fidelity:** `0.9883` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[04_Navbar|Navbar]], [[01_Card|Card]], [[10_ShaderCanvas|ShaderCanvas]]

Professional GlassMenu reverse-engineered from SdumUqJ3EN0_Elevenlabs_MCP_+_Claude_is_the_Ultimate_Creative_Unlock at 00:00.000. Features FADE_IN_SCALE micro-interaction animation with 17.85:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#080807` | `rgb(8, 8, 7)` | `oklch(0.13 0.003 106.7)` | `36.1%` |
| `surface` | `#413E3C` | `rgb(65, 62, 60)` | `oklch(0.37 0.005 56.2)` | `28.9%` |
| `accent` | `#020302` | `rgb(2, 3, 2)` | `oklch(0.09 0.007 145.0)` | `5.0%` |
| `text` | `#EFF2F7` | `rgb(239, 242, 247)` | `oklch(0.96 0.007 260.7)` | `5.6%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `69.58 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `1.45`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
import React from 'react';
import { motion } from 'framer-motion';
import { Home, Heart, Plus, User, Bell } from 'lucide-react';

interface GlassMenuProps {
  activeTab?: 'home' | 'likes' | 'create' | 'profile' | 'alerts';
  onTabChange?: (tab: string) => void;
}

const tabs = [
  { id: 'home', label: 'Home', icon: Home },
  { id: 'likes', label: 'Likes', icon: Heart },
  { id: 'create', label: 'Create', icon: Plus },
  { id: 'profile', label: 'Profile', icon: User },
  { id: 'alerts', label: 'Alerts', icon: Bell },
] as const;

export const GlassMenu: React.FC<GlassMenuProps> = ({
  activeTab = 'home',
  onTabChange,
}) => {
  return (
    <nav
      className="fixed bottom-6 left-1/2 -translate-x-1/2 z-50"
      aria-label="Main navigation"
    >
      <motion.div
        initial={{ opacity: 0, scale: 0.95 }}
        animate={{ opacity: 1, scale: 1 }}
        transition={{ type: 'spring', stiffness: 260, damping: 20 }}
        className="flex items-center gap-2 px-4 py-2.5 rounded-full bg-black/40 backdrop-blur-xl border border-white/10 shadow-2xl"
      >
        {tabs.map((tab) => {
          const isActive = activeTab === tab.id;
          const Icon = tab.icon;
          return (
            <button
              key={tab.id}
              onClick={() => onTabChange?.(tab.id)}
              aria-pressed={isActive}
              aria-label={tab.label}
              className={
                'relative flex flex-col items-center justify-center w-10 h-10 rounded-lg transition-all duration-200 ease-out group'
           
```

## 4. Flutter / Dart Implementation

```dart
// Flutter Material widget template
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
