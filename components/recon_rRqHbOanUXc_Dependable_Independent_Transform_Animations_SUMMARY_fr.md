---
title: "Modal — rRqHbOanUXc_Dependable_Indep (00:02.502)"
description: "Modal UI component (recon_rRqHbOanUXc_Dependable_Independent_Transform_Animations_SUMMARY_fr) with SSIM 0.9932, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_rRqHbOanUXc_Dependable_Independent_Transform_Animations_SUMMARY_from_Not_s1_00_modal"
category: "Modal"
ssim: 0.9932
quality_score: 8.72
tags: [modal, ui-design, design-tokens, react, flutter]
---

# Modal — rRqHbOanUXc_Dependable_Indep (00:02.502)

> **Category:** [[08_Modal|Modal]] | **SSIM Fidelity:** `0.9932` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[02_Button|Button]], [[06_Input|Input]], [[01_Card|Card]]

Professional Modal reverse-engineered from rRqHbOanUXc_Dependable_Independent_Transform_Animations_SUMMARY_from_Not at 00:02.502. Features FADE_IN_SCALE micro-interaction animation with 7.94:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#26272B` | `rgb(38, 39, 43)` | `oklch(0.27 0.007 274.7)` | `51.7%` |
| `surface` | `#F5B10E` | `rgb(245, 177, 14)` | `oklch(0.80 0.164 80.3)` | `35.5%` |
| `accent` | `#CA961B` | `rgb(202, 150, 27)` | `oklch(0.70 0.139 82.4)` | `0.5%` |
| `text` | `#F5B10E` | `rgb(245, 177, 14)` | `oklch(0.80 0.164 80.3)` | `35.5%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `70.07 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `0.13`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react';
import { motion, AnimatePresence } from 'framer-motion';

interface ModalProps {
  isOpen: boolean;
  onClose: () => void;
}

export const Modal: React.FC<ModalProps> = ({ isOpen, onClose }) => {
  return (
    <AnimatePresence>
      {isOpen && (
        <>
          <motion.div
            initial={{ opacity: 0 }}
            animate={{ opacity: 1 }}
            exit={{ opacity: 0 }}
            className="fixed inset-0 z-50 bg-black/60 backdrop-blur-sm"
            onClick={onClose}
            aria-hidden="true"
          />
          <motion.div
            initial={{ opacity: 0, scale: 0.95 }}
            animate={{ opacity: 1, scale: 1 }}
            exit={{ opacity: 0, scale: 0.95 }}
            transition={{ type: 'spring', stiffness: 260, damping: 20 }}
            className="fixed left-[50%] top-[50%] z-50 w-[830px] h-[693px] -translate-x-[50%] -translate-y-[50%] rounded-[28px] bg-[#F5B10E] shadow-2xl"
            role="dialog"
            aria-modal="true"
            aria-label="Modal"
          >
            <button
              onClick={onClose}
              className="absolute top-4 right-4 w-8 h-8 rounded-full bg-white/20 text-white flex items-center justify-center hover:bg-white/30 transition"
              aria-label="Close modal"
            >
              <svg className="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path strokeLinecap="round" strokeLinejoin="round" strokeWidth={2} d="M6 18L18 6M6 6l12 12" />
              </svg>
            </button>
            <div className="flex h-full
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class ModalDemo extends StatefulWidget {
  @override
  _ModalDemoState createState() => _ModalDemoState();
}

class _ModalDemoState extends State<ModalDemo> with SingleTickerProviderStateMixin {
  bool _isOpen = false;
  late AnimationController _controller;
  late Animation<double> _scale;
  late Animation<double> _opacity;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(vsync: this, duration: Duration(milliseconds: 700));
    _scale = Tween<double>(begin: 0.95, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOut),
    );
    _opacity = Tween<double>(begin: 0.0, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOut),
    );
  }

  @override
  void dispose() {
    _controller.dispose();
    super.dispose();
  }

  void _toggle() {
    setState(() {
      _isOpen = !_isOpen;
      if (_isOpen) _controller.forward();
    });
  }

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Color(0xFF26272B),
      body: Stack(
        children: [
          Center(
            child: ElevatedButton(
              onPressed: _toggle,
              child: Text('Open Modal'),
            ),
          ),
          if (_isOpen)
            GestureDetector(
              onTap: _toggle,
              child
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
