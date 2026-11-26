---
title: "Modal — 5V8tP5jDZ8U_How_OpenAI_Built (04:30.687)"
description: "Modal UI component (recon_5V8tP5jDZ8U_How_OpenAI_Built_Its_Data_Agent_s3_00_modal) with SSIM 0.9958, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_5V8tP5jDZ8U_How_OpenAI_Built_Its_Data_Agent_s3_00_modal"
category: "Modal"
ssim: 0.9958
quality_score: 8.72
tags: [modal, ui-design, design-tokens, react, flutter]
---

# Modal — 5V8tP5jDZ8U_How_OpenAI_Built (04:30.687)

> **Category:** [[08_Modal|Modal]] | **SSIM Fidelity:** `0.9958` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[02_Button|Button]], [[06_Input|Input]], [[01_Card|Card]]

Professional Modal reverse-engineered from 5V8tP5jDZ8U_How_OpenAI_Built_Its_Data_Agent at 04:30.687. Features FADE_IN_SCALE micro-interaction animation with 7.17:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#202020` | `rgb(32, 32, 32)` | `oklch(0.24 0.000 89.9)` | `90.7%` |
| `surface` | `#585857` | `rgb(88, 88, 87)` | `oklch(0.46 0.002 106.5)` | `3.3%` |
| `accent` | `#846C33` | `rgb(132, 108, 51)` | `oklch(0.54 0.081 86.6)` | `0.5%` |
| `text` | `#ADACA7` | `rgb(173, 172, 167)` | `oklch(0.74 0.007 97.4)` | `0.5%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `55.055 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
// Reconstructed from video evidence: 5V8tP5jDZ8U_How_OpenAI_Built_Its_Data_Agent.mp4 @ 04:30.687
import React from 'react'
import { motion } from 'framer-motion'

interface ModalProps {
  isOpen: boolean
  onClose: () => void
}

export const Modal: React.FC<ModalProps> = ({ isOpen, onClose }) => {
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
          damping: 20,
          duration: 0.55
        }
        className="w-[734px] h-[595px] bg-[#585857] rounded-[28px] shadow-2xl border border-white/10 relative overflow-hidden"
      >
        {/* Header strip with three dots */}
        <div className="flex justify-center pt-6 pb-4 border-b border-white/10">
          {[1, 2, 3].map((i) => (
            <div
              key={i}
              className="w-3 h-3 rounded-full border border-white/30 bg-transparent"
            />
          ))}
        </di
```

## 4. Flutter / Dart Implementation

```dart
// Flutter StatefulWidget
// Reconstructed from video evidence
import 'package:flutter/material.dart'

class ModalDemo extends StatefulWidget {
  const ModalDemo({super.key})

  @override
  State<ModalDemo> createState() => _ModalDemoState()
}

class _ModalDemoState extends State<ModalDemo> with SingleTickerProviderStateMixin {
  bool _isOpen = false
  late AnimationController _controller
  late Animation<double> _scaleAnim
  late Animation<double> _opacityAnim

  @override
  void initState() {
    super.initState()
    _controller = AnimationController(
      vsync: this,
      duration: const Duration(milliseconds: 550),
    )
    _scaleAnim = Tween<double>(begin: 0.95, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeOutBack),
    )
    _opacityAnim = Tween<double>(begin: 0.0, end: 1.0).animate(
      CurvedAnimation(parent: _controller, curve: Curves.easeIn),
    )
  }

  @override
  void dispose() {
    _controller.dispose()
    super.dispose()
  }

  void _toggleModal() {
    setState(() {
      _isOpen = !_isOpen
      if (_isOpen) _controller.forward()
      else _controller.reverse()
    })
  }

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: const Color(0xFF202020),
      body: Center(
        child: Column(
          mainAxisAlignment: MainAxisAlignment.center,
          children: [
       
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
