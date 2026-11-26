---
title: "Card — QZVzuq28eFw_OpenAI_s_lead_en (02:29.399)"
description: "Card UI component (recon_QZVzuq28eFw_OpenAI_s_lead_engineer_was_secretly_a_spy_s2_00_card) with SSIM 0.996, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_QZVzuq28eFw_OpenAI_s_lead_engineer_was_secretly_a_spy..._s2_00_card"
category: "Card"
ssim: 0.996
quality_score: 8.72
tags: [card, ui-design, design-tokens, react, flutter]
---

# Card — QZVzuq28eFw_OpenAI_s_lead_en (02:29.399)

> **Category:** [[01_Card|Card]] | **SSIM Fidelity:** `0.996` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[02_Button|Button]], [[03_GlassMenu|GlassMenu]], [[05_Hero|Hero]]

Professional Card reverse-engineered from QZVzuq28eFw_OpenAI_s_lead_engineer_was_secretly_a_spy... at 02:29.399. Features FADE_IN_SCALE micro-interaction animation with 19.5:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#0E0C0D` | `rgb(14, 12, 13)` | `oklch(0.16 0.004 345.8)` | `73.6%` |
| `surface` | `#B07864` | `rgb(176, 120, 100)` | `oklch(0.63 0.077 40.5)` | `0.1%` |
| `accent` | `#F4BDC1` | `rgb(244, 189, 193)` | `oklch(0.85 0.064 13.6)` | `0.3%` |
| `text` | `#FFFFFF` | `rgb(255, 255, 255)` | `oklch(1.00 0.000 89.9)` | `21.6%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `25.525 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `2.66`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react';
import { motion } from 'framer-motion';

export const CardWidget: React.FC = () => {
  return (
    <motion.div
      initial={{ opacity: 0, y: 16 }}
      animate={{ opacity: 1, y: 0 }}
      transition={{ duration: 0.4, ease: [0.16, 1, 0.3, 1] }}
      className="p-6 border border-slate-700/40 backdrop-blur-md shadow-lg"
      style={{
        backgroundColor: '#0E0C0D',
        color: '#FFFFFF',
        borderRadius: '28px',
        maxWidth: '941px',
      }}
    >
      <div class="space-y-3">
        <span class="text-xs font-semibold uppercase tracking-wider text-sky-400">ARGON Reconstructed</span>
        <h3 class="text-xl font-bold tracking-tight">Interactive Design Spec</h3>
        <p class="text-sm opacity-80 leading-relaxed">
          Reverse-engineered UI component reconstructed from video capture.
        </p>
      </div>
    </motion.div>
  );
};
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class CardWidget extends StatelessWidget {
  const CardWidget({super.key});

  @override
  Widget build(BuildContext context) {
    return Container(
      width: 941.0,
      padding: const EdgeInsets.all(24.0),
      decoration: BoxDecoration(
        color: const Color(0xFF0E0C0D),
        borderRadius: BorderRadius.circular(28),
      ),
      child: const Text('Interactive Design Spec'),
    );
  }
}
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
