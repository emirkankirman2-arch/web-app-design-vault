---
title: "Input — DeVKbIFOOy0_Video_by_viewcci (00:00.000)"
description: "Input UI component (recon_DeVKbIFOOy0_Video_by_viewcci_s1_00_input) with SSIM 0.992, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_DeVKbIFOOy0_Video_by_viewcci_s1_00_input"
category: "Input"
ssim: 0.992
quality_score: 8.72
tags: [input, ui-design, design-tokens, react, flutter]
---

# Input — DeVKbIFOOy0_Video_by_viewcci (00:00.000)

> **Category:** [[06_Input|Input]] | **SSIM Fidelity:** `0.992` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[02_Button|Button]], [[08_Modal|Modal]], [[09_SplashAuth|SplashAuth]]

Professional Input reverse-engineered from DeVKbIFOOy0_Video_by_viewcci at 00:00.000. Features FADE_IN_SCALE micro-interaction animation with 13.18:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#020102` | `rgb(2, 1, 2)` | `oklch(0.07 0.010 326.5)` | `24.9%` |
| `surface` | `#6B554D` | `rgb(107, 85, 77)` | `oklch(0.47 0.032 40.9)` | `15.5%` |
| `accent` | `#847552` | `rgb(132, 117, 82)` | `oklch(0.57 0.053 87.4)` | `5.0%` |
| `text` | `#DFCAB8` | `rgb(223, 202, 184)` | `oklch(0.85 0.034 63.0)` | `4.2%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `10.2 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.05`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS
// Reverse-engineered Input component (Style: AUTO)
// Dimensions: 159x35, Border Radius: 6, Dark Theme
// Motion: FADE_IN_SCALE, spring, 10200ms

import React from 'react'
import { motion } from 'framer-motion'

interface InputProps {
  value?: string
  onChange?: (e: React.ChangeEvent<HTMLInputElement>) => void
  placeholder?: string
  className?: string
}

export const Input: React.FC<InputProps> = ({
  value,
  onChange,
  placeholder = 'Enter text...',
  className,
}) => {
  return (
    <motion.div
      initial={{ opacity: 0, scale: 0.95 }}
      animate={{ opacity: 1, scale: 1 }}
      transition={
        type: 'spring',
        stiffness: 260,
        damping: 20,
      }
      className={
        'relative w-[159px] h-[35px] ' + (className || '')
      }
    >
      <input
        type="text"
        value={value}
        onChange={onChange}
        placeholder={placeholder}
        className={
          'w-full h-full bg-[#020102] border border-[#6B554D] rounded-[6px] ' +
          'text-[#DFCAB8] placeholder-[#DFCAB8]/50 ' +
          'text-sm font-medium leading-none ' +
          'outline-none focus:border-[#847552] focus:ring-1 focus:ring-[#847552] ' +
          'transition-colors duration-200 ease-in-out ' +
          'px-3 py-1.5'
        }
        aria-label="Text input"
        autoComplete="off"
        spellCheck={false}
      />
    </motion.div>
  )
}

export default Input
```

## 4. Flutter / Dart Implementation

```dart
// Flutter StatefulWidget
// Reverse-engineered Input component (Style: AUTO)
// Dimensions: 159x35, Border Radius: 6, Dark Theme

import 'package:flutter/material.dart';

class InputWidget extends StatefulWidget {
  final String? initialValue;
  final ValueChanged<String>? onChanged;
  final String placeholder;

  const InputWidget({
    Key? key,
    this.initialValue,
    this.onChanged,
    this.placeholder = 'Enter text...',
  }) : super(key: key);

  @override
  State<InputWidget> createState() => _InputWidgetState();
}

class _InputWidgetState extends State<InputWidget>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scaleAnimation;
  late Animation<double> _opacityAnimation;
  final TextEditingController _textController = TextEditingController();

  @override
  void initState() {
    super.initState();
    _textController.text = widget.initialValue ?? '';
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 10200),
    );
    _scaleAnimation = Tween<double>(begin: 0.95, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOut),
    );
    _opacityAnimation = Tween<double>(begin: 0.0, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOut),
    );
    _controller.forward();
  }

  @override
  void dispose() 
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
