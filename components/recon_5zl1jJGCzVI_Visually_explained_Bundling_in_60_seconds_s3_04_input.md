---
title: "Input — 5zl1jJGCzVI_Visually_explain (00:38.000)"
description: "Input UI component (recon_5zl1jJGCzVI_Visually_explained_Bundling_in_60_seconds_s3_04_input) with SSIM 0.9865, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_5zl1jJGCzVI_Visually_explained_-_Bundling_in_60_seconds_s3_04_input"
category: "Input"
ssim: 0.9865
quality_score: 8.72
tags: [input, ui-design, design-tokens, react, flutter]
---

# Input — 5zl1jJGCzVI_Visually_explain (00:38.000)

> **Category:** [[06_Input|Input]] | **SSIM Fidelity:** `0.9865` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[02_Button|Button]], [[08_Modal|Modal]], [[09_SplashAuth|SplashAuth]]

Professional Input reverse-engineered from 5zl1jJGCzVI_Visually_explained_-_Bundling_in_60_seconds at 00:38.000. Features FADE_IN_SCALE micro-interaction animation with 4.65:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#000000` | `rgb(0, 0, 0)` | `oklch(0.00 0.000 0.0)` | `90.7%` |
| `surface` | `#3A3534` | `rgb(58, 53, 52)` | `oklch(0.33 0.007 31.1)` | `1.0%` |
| `accent` | `#030102` | `rgb(3, 1, 2)` | `oklch(0.08 0.013 345.0)` | `5.0%` |
| `text` | `#787676` | `rgb(120, 118, 118)` | `oklch(0.57 0.002 17.2)` | `0.1%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `14.0 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react';
import { motion } from 'framer-motion';

interface InputProps {
  value?: string;
  onChange?: (e: React.ChangeEvent<HTMLInputElement>) => void;
  placeholder?: string;
  className?: string;
}

export const Input: React.FC<InputProps> = ({
  value,
  onChange,
  placeholder = '// bundle.js',
  className = '',
}) => {
  return (
    <motion.div
      initial={{ opacity: 0, scale: 0.95 }}
      animate={{ opacity: 1, scale: 1 }}
      transition={{ type: 'spring', stiffness: 260, damping: 20 }}
      className={\`relative w-full \${className}\`}
    >
      <input
        type="text"
        value={value}
        onChange={onChange}
        placeholder={placeholder}
        className={\`w-full h-8 bg-transparent border-none text-gray-400 placeholder-gray-400 text-sm font-mono outline-none focus:ring-0 focus-visible:ring-0 disabled:cursor-not-allowed disabled:opacity-50 \${className}\`}
        aria-label="Input field"
      />
    </motion.div>
  );
};

// Default export for convenience
export default Input;
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class InputWidget extends StatefulWidget {
  final String? initialValue;
  final ValueChanged<String>? onChanged;
  final String placeholder;

  const InputWidget({
    Key? key,
    this.initialValue,
    this.onChanged,
    this.placeholder = '// bundle.js',
  }) : super(key: key);

  @override
  State<InputWidget> createState() => _InputWidgetState();
}

class _InputWidgetState extends State<InputWidget>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _opacityAnim;
  late Animation<double> _scaleAnim;
  final TextEditingController _textController = TextEditingController();

  @override
  void initState() {
    super.initState();
    _textController.text = widget.initialValue ?? '';
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 14000),
    );
    _opacityAnim = Tween<double>(begin: 0.0, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeInOut),
    );
    _scaleAnim = Tween<double>(begin: 0.95, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeInOut),
    );
    _controller.forward();
  }

  @override
  void dispose() {
    _controller.dispose();
    _textController.dispose();
    super.dispose();
  }

  @override
  Widget build(BuildContext context) {
    return 
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
