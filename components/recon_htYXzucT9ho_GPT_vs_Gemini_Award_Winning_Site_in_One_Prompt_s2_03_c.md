---
title: "Card — htYXzucT9ho_GPT_vs_Gemini_Aw (05:09.400)"
description: "Card UI component (recon_htYXzucT9ho_GPT_vs_Gemini_Award_Winning_Site_in_One_Prompt_s2_03_c) with SSIM 0.9946, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_htYXzucT9ho_GPT_vs_Gemini_-_Award_Winning_Site_in_One_Prompt_s2_03_card"
category: "Card"
ssim: 0.9946
quality_score: 8.72
tags: [card, ui-design, design-tokens, react, flutter]
---

# Card — htYXzucT9ho_GPT_vs_Gemini_Aw (05:09.400)

> **Category:** [[01_Card|Card]] | **SSIM Fidelity:** `0.9946` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[02_Button|Button]], [[03_GlassMenu|GlassMenu]], [[05_Hero|Hero]]

Professional Card reverse-engineered from htYXzucT9ho_GPT_vs_Gemini_-_Award_Winning_Site_in_One_Prompt at 05:09.400. Features FADE_IN_SCALE micro-interaction animation with 8.89:1 WCAG contrast.

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
// React TypeScript + Tailwind CSS + Framer Motion
import { motion } from 'framer-motion';

export interface CanvaCardProps {
  children?: React.ReactNode;
  className?: string;
}

export const CanvaCard: React.FC<CanvaCardProps> = ({ children, className }) => {
  return (
    <motion.div
      initial={{ opacity: 0, scale: 0.95 }}
      animate={{ opacity: 1, scale: 1 }}
      transition={{ type: 'spring', stiffness: 260, damping: 20 }}
      className={
        'relative w-[153px] h-[30px] bg-black text-[#AAA8AA] shadow-lg overflow-hidden ' +
        (className ?? '')
      }
    >
      {children}
    </motion.div>
  );
};

export default CanvaCard;
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class CanvaCard extends StatefulWidget {
  const CanvaCard({super.key});

  @override
  State<CanvaCard> createState() => _CanvaCardState();
}

class _CanvaCardState extends State<CanvaCard> with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scale;
  late Animation<double> _opacity;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 1200),
    );
    _scale = Tween<double>(begin: 0.95, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOut),
    );
    _opacity = Tween<double>(begin: 0.0, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOut),
    );
    _controller.forward();
  }

  @override
  void dispose() {
    _controller.dispose();
    super.dispose();
  }

  @override
  Widget build(BuildContext context) {
    return AnimatedBuilder(
      animation: _controller,
      builder: (context, child) {
        return Opacity(
          opacity: _opacity.value,
          child: Transform.scale(
            scale: _scale.value,
            child: Container(
              width: 153,
              height: 30,
              decoration: BoxDecoration(
                color: Colors.black,
                boxShadow: [
       
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
