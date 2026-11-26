---
title: "Modal — 4ZBhE4CPegA_How_Google_AI_Ed (00:00.000)"
description: "Modal UI component (recon_4ZBhE4CPegA_How_Google_AI_Edge_built_a_local_AI_desktop_app_in_10_) with SSIM 0.9885, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_4ZBhE4CPegA_How_Google_AI_Edge_built_a_local_AI_desktop_app_in_10_days_s1_00_modal"
category: "Modal"
ssim: 0.9885
quality_score: 8.72
tags: [modal, ui-design, design-tokens, react, flutter]
---

# Modal — 4ZBhE4CPegA_How_Google_AI_Ed (00:00.000)

> **Category:** [[08_Modal|Modal]] | **SSIM Fidelity:** `0.9885` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[02_Button|Button]], [[06_Input|Input]], [[01_Card|Card]]

Professional Modal reverse-engineered from 4ZBhE4CPegA_How_Google_AI_Edge_built_a_local_AI_desktop_app_in_10_days at 00:00.000. Features FADE_IN_SCALE micro-interaction animation with 15.54:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#151310` | `rgb(21, 19, 16)` | `oklch(0.19 0.007 78.1)` | `24.2%` |
| `surface` | `#45392A` | `rgb(69, 57, 42)` | `oklch(0.35 0.030 72.8)` | `19.0%` |
| `accent` | `#624530` | `rgb(98, 69, 48)` | `oklch(0.42 0.052 56.7)` | `9.6%` |
| `text` | `#ECEBE7` | `rgb(236, 235, 231)` | `oklch(0.94 0.005 95.1)` | `10.5%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `20.287 s`
- **Spring Overshoot:** `True` | **Peak Velocity:** `4.01`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react'
import { motion } from 'framer-motion'

interface ModalProps {
  isOpen: boolean
  onClose: () => void
  children: React.ReactNode
}

export const Modal: React.FC<ModalProps> = ({ isOpen, onClose, children }) => {
  if (!isOpen) return null

  return (
    <motion.div
      initial={{ opacity: 0, scale: 0.95 }}
      animate={{ opacity: 1, scale: 1 }}
      exit={{ opacity: 0, scale: 0.95 }}
      transition={{ type: 'spring', stiffness: 260, damping: 20 }}
      className="fixed inset-0 z-50 flex items-center justify-center"
      role="dialog"
      aria-modal="true"
      aria-labelledby="modal-title"
    >
      {/* Backdrop */}
      <motion.div
        initial={{ opacity: 0 }}
        animate={{ opacity: 0.6 }}
        exit={{ opacity: 0 }}
        className="absolute inset-0 bg-black/60 backdrop-blur-sm"
        onClick={onClose}
      />

      {/* Modal Panel */}
      <motion.div
        initial={{ opacity: 0, y: 20 }}
        animate={{ opacity: 1, y: 0 }}
        exit={{ opacity: 0, y: 20 }}
        transition={{ type: 'spring', stiffness: 260, damping: 20 }}
        className="w-[693px] h-[649px] bg-[#45392A] rounded-[28px] shadow-2xl relative overflow-hidden"
      >
        {/* Close Button */}
        <button
          onClick={onClose}
          className="absolute top-6 right-6 w-8 h-8 rounded-full bg-white/10 hover:bg-white/20 flex items-center justify-center text-white transition-colors"
          aria-label="Close modal"
        >
          <svg className="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
        
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class ModalDemo extends StatefulWidget {
  const ModalDemo({super.key});

  @override
  State<ModalDemo> createState() => _ModalDemoState();
}

class _ModalDemoState extends State<ModalDemo> {
  bool _isOpen = false;

  void _toggleModal() => setState(() => _isOpen = !_isOpen);

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: const Color(0xFF151310),
      body: Center(
        child: Column(
          mainAxisAlignment: MainAxisAlignment.center,
          children: [
            ElevatedButton(
              onPressed: _toggleModal,
              style: ElevatedButton.styleFrom(
                backgroundColor: const Color(0xFF624530),
                foregroundColor: const Color(0xFFECEBE7),
              ),
              child: const Text('Open Modal'),
            ),
            if (_isOpen)
              _buildModal(),
          ],
        ),
      ),
    );
  }

  Widget _buildModal() {
    return AnimatedOpacity(
      duration: const Duration(milliseconds: 300),
      opacity: _isOpen ? 1.0 : 0.0,
      child: AbsorbPointer(
        absorbing: !_isOpen,
        child: Stack(
          children: [
            // Backdrop
            GestureDetector(
              onTap: _toggleModal,
              child: Container(
                color: Colors.black.withOpacity(0.6),
              ),
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2-arch.itch.io/web-app-design-vault](https://emirkankirman2-arch.itch.io/web-app-design-vault)
