---
title: "Card — SOwUWPtXQ9I_Jensen_Huang_jus (02:42.500)"
description: "Card UI component (recon_SOwUWPtXQ9I_Jensen_Huang_just_pulled_out_of_Nvidia_s2_03_card) with SSIM 0.9965, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_SOwUWPtXQ9I_Jensen_Huang_just_pulled_out_of_Nvidia..._s2_03_card"
category: "Card"
ssim: 0.9965
quality_score: 8.72
tags: [card, ui-design, design-tokens, react, flutter]
---

# Card — SOwUWPtXQ9I_Jensen_Huang_jus (02:42.500)

> **Category:** [[01_Card|Card]] | **SSIM Fidelity:** `0.9965` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[02_Button|Button]], [[03_GlassMenu|GlassMenu]], [[05_Hero|Hero]]

Professional Card reverse-engineered from SOwUWPtXQ9I_Jensen_Huang_just_pulled_out_of_Nvidia... at 02:42.500. Features FADE_IN_SCALE micro-interaction animation with 19.46:1 WCAG contrast.

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
        backgroundColor: '#FEFEFE',
        color: '#0B0C07',
        borderRadius: '8px',
        maxWidth: '258px',
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
      width: 258.0,
      padding: const EdgeInsets.all(24.0),
      decoration: BoxDecoration(
        color: const Color(0xFFFEFEFE),
        borderRadius: BorderRadius.circular(8),
      ),
      child: const Text('Interactive Design Spec'),
    );
  }
}
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
