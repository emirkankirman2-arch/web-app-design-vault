---
title: "Modal — 9KuSYhnQy_E_I_built_an_A_I_t (00:08.300)"
description: "Modal UI component (recon_9KuSYhnQy_E_I_built_an_A_I_that_lets_you_track_Fireship_s1_00_moda) with SSIM 0.9865, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_9KuSYhnQy_E_I_built_an_A.I._that_lets_you_track_Fireship_s1_00_modal"
category: "Modal"
ssim: 0.9865
quality_score: 8.72
tags: [modal, ui-design, design-tokens, react, flutter]
---

# Modal — 9KuSYhnQy_E_I_built_an_A_I_t (00:08.300)

> **Category:** [[08_Modal|Modal]] | **SSIM Fidelity:** `0.9865` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[02_Button|Button]], [[06_Input|Input]], [[01_Card|Card]]

Professional Modal reverse-engineered from 9KuSYhnQy_E_I_built_an_A.I._that_lets_you_track_Fireship at 00:08.300. Features FADE_IN_SCALE micro-interaction animation with 19.51:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#010102` | `rgb(1, 1, 2)` | `oklch(0.07 0.008 284.1)` | `52.5%` |
| `surface` | `#65484D` | `rgb(101, 72, 77)` | `oklch(0.43 0.040 7.4)` | `2.6%` |
| `accent` | `#E5BCAE` | `rgb(229, 188, 174)` | `oklch(0.83 0.051 39.7)` | `1.1%` |
| `text` | `#F9F7F4` | `rgb(249, 247, 244)` | `oklch(0.98 0.005 78.3)` | `5.5%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `53.95 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.03`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
// Reconstructed Modal component based on video evidence (00:08.300)
// Dimensions: 641x589, Border radius: 28, Dark theme

import React from 'react'
import { motion, AnimatePresence } from 'framer-motion'

interface ModalProps {
  isOpen: boolean
  onClose: () => void
  children: React.ReactNode
}

export const Modal: React.FC<ModalProps> = ({ isOpen, onClose, children }) => {
  return (
    <AnimatePresence>
      {isOpen && (
        <>
          {/* Backdrop */}
          <motion.div
            initial={{ opacity: 0 }}
            animate={{ opacity: 1 }}
            exit={{ opacity: 0 }}
            className="fixed inset-0 z-50 bg-black/60 backdrop-blur-sm"
            onClick={onClose}
            aria-hidden="true"
          />

          {/* Modal Container */}
          <motion.div
            initial={{ opacity: 0, scale: 0.95 }}
            animate={{ opacity: 1, scale: 1 }}
            exit={{ opacity: 0, scale: 0.95 }}
            transition={
              type: 'spring',
              stiffness: 260,
              damping: 20
            }
            className="fixed left-[50%] top-[50%] z-50 w-[641px] h-[589px] -translate-x-[50%] -translate-y-[50%] rounded-[28px] bg-[#65484D] shadow-2xl p-8"
            role="dialog"
            aria-modal="true"
            aria-labelledby="modal-title"
          >
            <div className="flex justify-between items-start mb-6">
              <h2 id="modal-title" className="text-xl font-semibold text-[#F9F7F4]">
                Modal Title
              </h2>
        
```

## 4. Flutter / Dart Implementation

```dart
// Flutter Widget - Modal Component
// Reconstructed based on video evidence

import 'package:flutter/material.dart';

class ReconstructedModal extends StatefulWidget {
  final bool isOpen;
  final VoidCallback onClose;
  final Widget child;

  const ReconstructedModal({
    Key? key,
    required this.isOpen,
    required this.onClose,
    required this.child,
  }) : super(key: key);

  @override
  State<ReconstructedModal> createState() => _ReconstructedModalState();
}

class _ReconstructedModalState extends State<ReconstructedModal>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _scaleAnimation;
  late Animation<double> _opacityAnimation;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      duration: const Duration(milliseconds: 500),
      vsync: this,
    );
    _scaleAnimation = Tween<double>(begin: 0.95, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOut),
    );
    _opacityAnimation = Tween<double>(begin: 0.0, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOut),
    );
  }

  @override
  void didUpdateWidget(ReconstructedModal oldWidget) {
    super.didUpdateWidget(oldWidget);
    if (widget.isOpen && !oldWidget.isOpen) {
      _controller.forward();
    } else if (!widget.isOpen && oldWidget.isOp
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
