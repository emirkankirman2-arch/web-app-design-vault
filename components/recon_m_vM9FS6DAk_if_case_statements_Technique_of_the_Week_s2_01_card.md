---
title: "Card — m_vM9FS6DAk_if_case_statemen (00:40.717)"
description: "Card UI component (recon_m_vM9FS6DAk_if_case_statements_Technique_of_the_Week_s2_01_card) with SSIM 0.9937, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_m-vM9FS6DAk_if-case_statements_Technique_of_the_Week_s2_01_card"
category: "Card"
ssim: 0.9937
quality_score: 8.72
tags: [card, ui-design, design-tokens, react, flutter]
---

# Card — m_vM9FS6DAk_if_case_statemen (00:40.717)

> **Category:** [[01_Card|Card]] | **SSIM Fidelity:** `0.9937` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[02_Button|Button]], [[03_GlassMenu|GlassMenu]], [[05_Hero|Hero]]

Professional Card reverse-engineered from m-vM9FS6DAk_if-case_statements_Technique_of_the_Week at 00:40.717. Features FADE_IN_SCALE micro-interaction animation with 10.04:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#C1DFE8` | `rgb(193, 223, 232)` | `oklch(0.88 0.034 217.8)` | `38.4%` |
| `surface` | `#B4DBE6` | `rgb(180, 219, 230)` | `oklch(0.87 0.044 216.7)` | `27.3%` |
| `accent` | `#082B57` | `rgb(8, 43, 87)` | `oklch(0.29 0.089 256.5)` | `14.8%` |
| `text` | `#082B57` | `rgb(8, 43, 87)` | `oklch(0.29 0.089 256.5)` | `14.8%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `12.717 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react'
import { motion } from 'framer-motion'

type CodeSnippetCardProps = {
  code?: string
  className?: string
}

export const CodeSnippetCard: React.FC<CodeSnippetCardProps> = ({
  code = 'if (value case pattern) { ... }',
  className = ''
}) => {
  return (
    <motion.div
      initial={{ opacity: 0, scale: 0.95 }}
      animate={{ opacity: 1, scale: 1 }}
      transition={{ type: 'spring', stiffness: 260, damping: 20 }}
      className={
        'relative rounded-2xl bg-[#082B57] shadow-xl p-6 overflow-hidden ' +
        className
      }
    >
      {/* Decorative top-left accent dot */}
      <div className="absolute top-4 left-4 w-2 h-2 rounded-full bg-[#4CAF50]" />

      <pre className="m-0 font-mono text-sm leading-relaxed text-white">
        <code className="block whitespace-pre">
          <span className="text-[#4CAF50]">if</span>{' '}
          <span className="text-[#64B5F6]">(value case pattern)</span>{' '}
          <span className="text-white">&#123; ... &#125;</span>
        </code>
      </pre>
    </motion.div>
  )
}

// Usage example:
// <CodeSnippetCard code="if (value case pattern) { ... }" />
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class CodeSnippetCard extends StatefulWidget {
  final String code;
  const CodeSnippetCard({Key? key, this.code = 'if (value case pattern) { ... }'}) : super(key: key);

  @override
  State<CodeSnippetCard> createState() => _CodeSnippetCardState;
}

class _CodeSnippetCardState extends State<CodeSnippetCard>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scale;
  late Animation<double> _opacity;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 12716),
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
              width: 1018,
              h
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
