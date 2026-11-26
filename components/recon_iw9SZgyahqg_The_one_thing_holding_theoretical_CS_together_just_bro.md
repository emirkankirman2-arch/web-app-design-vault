---
title: "Modal — iw9SZgyahqg_The_one_thing_ho (02:54.299)"
description: "Modal UI component (recon_iw9SZgyahqg_The_one_thing_holding_theoretical_CS_together_just_bro) with SSIM 0.9884, OKLCH design tokens, SLIDE_DOWN motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_iw9SZgyahqg_The_one_thing_holding_theoretical_CS_together_just_broke...__s2_00_modal"
category: "Modal"
ssim: 0.9884
quality_score: 8.72
tags: [modal, ui-design, design-tokens, react, flutter]
---

# Modal — iw9SZgyahqg_The_one_thing_ho (02:54.299)

> **Category:** [[08_Modal|Modal]] | **SSIM Fidelity:** `0.9884` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[02_Button|Button]], [[06_Input|Input]], [[01_Card|Card]]

Professional Modal reverse-engineered from iw9SZgyahqg_The_one_thing_holding_theoretical_CS_together_just_broke..._ at 02:54.299. Features SLIDE_DOWN micro-interaction animation with 19.0:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#0E0C0D` | `rgb(14, 12, 13)` | `oklch(0.16 0.004 345.8)` | `40.7%` |
| `surface` | `#A6A3A3` | `rgb(166, 163, 163)` | `oklch(0.72 0.003 17.2)` | `5.0%` |
| `accent` | `#D00F1A` | `rgb(208, 15, 26)` | `oklch(0.54 0.216 27.1)` | `3.8%` |
| `text` | `#FCFCFC` | `rgb(252, 252, 252)` | `oklch(0.99 0.000 89.9)` | `21.1%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `SLIDE_DOWN`
- **Measured Duration:** `23.649 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `1.92`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react'
import { motion, AnimatePresence } from 'framer-motion'

interface ModalProps {
  isOpen: boolean
  onClose: () => void
  title?: string
  children: React.ReactNode
}

export const Modal: React.FC<ModalProps> = ({
  isOpen,
  onClose,
  title,
  children,
}) => {
  const containerVariants = {
    hidden: { opacity: 0 },
    visible: {
      opacity: 1,
      transition: { staggerChildren: 0.05 },
    },
    hiddenExit: { opacity: 0 },
  }

  const itemVariants = {
    hidden: { y: -8.122, opacity: 0 },
    visible: {
      y: 0,
      opacity: 1,
      transition: {
        duration: 23.65,
        ease: [0.16, 1, 0.3, 1],
      },
    },
    exit: {
      y: -8.122,
      opacity: 0,
      transition: { duration: 0.2 },
    },
  }

  return (
    <AnimatePresence>
      {isOpen && (
        <>
          <div
            className="fixed inset-0 z-50 bg-black/60 backdrop-blur-sm"
            onClick={onClose}
            aria-hidden="true"
          />
          <motion.div
            initial="hidden"
            animate="visible"
            exit="hiddenExit"
            variants={containerVariants}
            className="fixed inset-0 z-50 flex items-center justify-center p-4"
            role="dialog"
            aria-modal="true"
            aria-labelledby="modal-title"
          >
            <motion.div
              variants={itemVariants}
              className="w-full max-w-[1021px] h-[686px] bg-[#A6A3A3] rounded-[28px] shadow-2xl overflow-hidden flex flex-col"
            >
              {title && (
                <div className="flex
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class ModalWidget extends StatefulWidget {
  final bool isOpen;
  final VoidCallback onClose;
  final String? title;
  final Widget child;

  const ModalWidget({
    Key? key,
    required this.isOpen,
    required this.onClose,
    this.title,
    required this.child,
  }) : super(key: key);

  @override
  State<ModalWidget> createState() => _ModalWidgetState();
}

class _ModalWidgetState extends State<ModalWidget>
    with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _opacity;
  late Animation<Offset> _offset;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      duration: const Duration(milliseconds: 23648),
      vsync: this,
    );
    _opacity = Tween<double>(begin: 0.0, end: 1.0).animate(_controller);
    _offset = Tween<Offset>(begin: const Offset(0, -0.02), end: Offset.zero)
        .animate(
          CurvedAnimation(parent: _controller, curve: Curves.easeInOut),
        );
    if (widget.isOpen) _controller.forward();
  }

  @override
  void didUpdateWidget(ModalWidget oldWidget) {
    super.didUpdateWidget(oldWidget);
    if (widget.isOpen && !oldWidget.isOpen) {
      _controller.forward(from: 0);
    } else if (!widget.isOpen && oldWidget.isOpen) {
      _controller.reverse();
    }
  }

  @override
  void dispose() {
    _c
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
