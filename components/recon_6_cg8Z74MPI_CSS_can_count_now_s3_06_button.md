---
title: "Button — 6_cg8Z74MPI_CSS_can_count_no (04:22.933)"
description: "Button UI component (recon_6_cg8Z74MPI_CSS_can_count_now_s3_06_button) with SSIM 0.9904, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_6-cg8Z74MPI_CSS_can_count_now_s3_06_button"
category: "Button"
ssim: 0.9904
quality_score: 8.72
tags: [button, ui-design, design-tokens, react, flutter]
---

# Button — 6_cg8Z74MPI_CSS_can_count_no (04:22.933)

> **Category:** [[02_Button|Button]] | **SSIM Fidelity:** `0.9904` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[01_Card|Card]], [[06_Input|Input]], [[08_Modal|Modal]]

Professional Button reverse-engineered from 6-cg8Z74MPI_CSS_can_count_now at 04:22.933. Features FADE_IN_SCALE micro-interaction animation with 5.63:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#15181D` | `rgb(21, 24, 29)` | `oklch(0.21 0.011 260.7)` | `35.3%` |
| `surface` | `#534C54` | `rgb(83, 76, 84)` | `oklch(0.43 0.016 322.0)` | `2.9%` |
| `accent` | `#252034` | `rgb(37, 32, 52)` | `oklch(0.26 0.037 295.1)` | `5.0%` |
| `text` | `#9B88BC` | `rgb(155, 136, 188)` | `oklch(0.66 0.079 301.0)` | `1.5%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `71.533 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react';
import { motion } from 'framer-motion';
import { Code2 } from 'lucide-react';

interface GlassMenuButtonProps {
  icon: React.ReactNode;
  label: string;
  isActive?: boolean;
  onClick?: () => void;
}

export const GlassMenuButton: React.FC<GlassMenuButtonProps> = ({
  icon,
  label,
  isActive = false,
  onClick,
}) => {
  return (
    <motion.button
      whileHover={{ scale: 1.05 }}
      whileTap={{ scale: 0.95 }}
      onClick={onClick}
      className={
        'relative flex flex-col items-center justify-center w-16 h-8 rounded-md transition-all duration-200 ' +
        (isActive
          ? 'bg-[#252034] text-[#9B88BC] shadow-[0_0_15px_rgba(37,32,52,0.6)]'
          : 'bg-[#15181D]/80 backdrop-blur-md text-[#534C54] hover:bg-[#252034]/50 hover:text-[#9B88BC]')
      }
      aria-label={label}
    >
      <div className="absolute inset-0 rounded-md bg-gradient-to-b from-white/10 to-transparent opacity-0 hover:opacity-100 transition-opacity" />
      <span className="relative z-10 text-[10px] font-medium tracking-tight leading-none">
        {icon}
      </span>
      <span className="relative z-10 mt-0.5 text-[10px] font-medium tracking-tight leading-none">
        {label}
      </span>
    </motion.button>
  );
};

export const GlassMenuBar: React.FC = () => {
  const tabs = [
    { icon: <Code2 size={14} strokeWidth={1.5} />, label: 'Home' },
    { icon: <Code2 size={14} strokeWidth={1.5} />, label: 'Likes' },
    { icon: <Code2 size={14} strokeWidth={1.5} />, label: 'Create' },
    { icon: <Code2 size={14} strokeWidth={1.5} />, label: '
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class GlassMenuButton extends StatelessWidget {
  final IconData icon;
  final String label;
  final bool isActive;
  final VoidCallback? onTap;

  const GlassMenuButton({
    super.key,
    required this.icon,
    required this.label,
    this.isActive = false,
    this.onTap,
  });

  @override
  Widget build(BuildContext context) {
    return GestureDetector(
      onTap: onTap,
      child: AnimatedContainer(
        duration: const Duration(milliseconds: 200),
        width: 76,
        height: 32,
        decoration: BoxDecoration(
          color: isActive ? const Color(0xFF252034) : const Color(0xFF15181D).withOpacity(0.8),
          borderRadius: BorderRadius.circular(6),
          boxShadow: isActive
              ? [
                  BoxShadow(
                    color: const Color(0xFF252034).withOpacity(0.6),
                    blurRadius: 15,
                    spreadRadius: 0,
                  )
                ]
              : null,
          border: Border.all(
            color: Colors.white.withOpacity(0.05),
            width: 1,
          ),
        ),
        child: Column(
          mainAxisAlignment: MainAxisAlignment.center,
          children: [
            Icon(
              icon,
              size: 14,
              color: isActive ? const Color(0xFF9B88BC) : const Color(0xFF534C54),
            ),
   
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
