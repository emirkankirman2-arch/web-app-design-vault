---
title: "Modal — lUS2HOWj4o8_Cursor_Tracking_ (03:11.658)"
description: "Modal UI component (recon_lUS2HOWj4o8_Cursor_Tracking_with_CSS_Variables_SUMMARY_iOS_Button_) with SSIM 0.9939, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_lUS2HOWj4o8_Cursor_Tracking_with_CSS_Variables_SUMMARY_iOS_Button_Hover__s3_00_modal"
category: "Modal"
ssim: 0.9939
quality_score: 8.72
tags: [modal, ui-design, design-tokens, react, flutter]
---

# Modal — lUS2HOWj4o8_Cursor_Tracking_ (03:11.658)

> **Category:** [[08_Modal|Modal]] | **SSIM Fidelity:** `0.9939` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[02_Button|Button]], [[06_Input|Input]], [[01_Card|Card]]

Professional Modal reverse-engineered from lUS2HOWj4o8_Cursor_Tracking_with_CSS_Variables_SUMMARY_iOS_Button_Hover_ at 03:11.658. Features FADE_IN_SCALE micro-interaction animation with 7.96:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#25262A` | `rgb(37, 38, 42)` | `oklch(0.27 0.008 274.7)` | `48.2%` |
| `surface` | `#F4B00D` | `rgb(244, 176, 13)` | `oklch(0.80 0.164 80.2)` | `40.2%` |
| `accent` | `#D29B19` | `rgb(210, 155, 25)` | `oklch(0.72 0.144 82.0)` | `0.5%` |
| `text` | `#F4B00D` | `rgb(244, 176, 13)` | `oklch(0.80 0.164 80.2)` | `40.2%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `106.239 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.52`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
// Reconstructed Modal component based on video evidence
// Source: lUS2HOWj4o8_Cursor_Tracking_with_CSS_Variables_SUMMARY_iOS_Button_Hover_.mp4

import React from 'react'
import { motion } from 'framer-motion'

interface ModalProps {
  isOpen: boolean
  onClose: () => void
  children?: React.ReactNode
}

export const Modal: React.FC<ModalProps> = ({ isOpen, onClose, children }) => {
  if (!isOpen) return null

  return (
    <div
      className="fixed inset-0 z-50 flex items-center justify-center"
      role="dialog"
      aria-modal="true"
      aria-labelledby="modal-title"
    >
      {/* Backdrop */}
      <motion.div
        initial={{ opacity: 0 }}
        animate={{ opacity: 1 }}
        exit={{ opacity: 0 }}
        transition={{ duration: 0.2 }}
        className="absolute inset-0 bg-black/60 backdrop-blur-sm"
        onClick={onClose}
      />

      {/* Modal Panel */}
      <motion.div
        initial={{ opacity: 0, scale: 0.95 }}
        animate={{ opacity: 1, scale: 1 }}
        exit={{ opacity: 0, scale: 0.95 }}
        transition={
          type: 'spring',
          stiffness: 260,
          damping: 20
        }
        className="w-[868px] h-[693px] bg-[#F4B00D] rounded-[28px] shadow-2xl relative overflow-hidden"
      >
        {/* Close Button */}
        <button
          onClick={onClose}
          className="absolute top-6 right-6 w-10 h-10 rounded-full bg-white/20 hover:bg-white/30 flex items-center justify-center transition-colors"
          aria-label="Close modal"
        >
          <svg class
```

## 4. Flutter / Dart Implementation

```dart
// Flutter StatefulWidget
// Reconstructed Modal component based on video evidence

import 'package:flutter/material.dart';\n\nclass ReconstructedModal extends StatefulWidget {\n  final bool isOpen;\n  final VoidCallback onClose;\n  final Widget? child;\n\n  const ReconstructedModal({\n    Key? key,\n    required this.isOpen,\n    required this.onClose,\n    this.child,\n  }) : super(key: key);\n\n  @override\n  State<ReconstructedModal> createState() => _ReconstructedModalState();\n}\n\nclass _ReconstructedModalState extends State<ReconstructedModal>\n    with SingleTickerProviderStateMixin {\n  late AnimationController _controller;\n  late Animation<double> _scaleAnimation;\n  late Animation<double> _opacityAnimation;\n\n  @override\n  void initState() {\n    super.initState();\n    _controller = AnimationController(\n      duration: const Duration(milliseconds: 800),\n      vsync: this,\n    );\n    _scaleAnimation = Tween<double>(begin: 0.95, end: 1.0).animate(\n      CurvedAnimation(parent: _controller, curve: Curves.easeOutBack),\n    );\n    _opacityAnimation = Tween<double>(begin: 0.0, end: 1.0).animate(\n      CurvedAnimation(parent: _controller, curve: Curves.easeIn),\n    );\n    if (widget.isOpen) _controller.forward();\n  }\n\n  @override\n  void didUpdateWidget(ReconstructedModal oldWidget) {\n    super.didUpdateWidget(oldWidget);\n    if (widget.isOpen && !oldWid
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
