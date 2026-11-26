---
title: "Modal — d26zVaVJZgM_I_Redesigned_App (00:08.800)"
description: "Modal UI component (recon_d26zVaVJZgM_I_Redesigned_Apps_to_Look_Like_Their_NAMES_s1_00_modal) with SSIM 0.9881, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_d26zVaVJZgM_I_Redesigned_Apps_to_Look_Like_Their_NAMES_s1_00_modal"
category: "Modal"
ssim: 0.9881
quality_score: 8.72
tags: [modal, ui-design, design-tokens, react, flutter]
---

# Modal — d26zVaVJZgM_I_Redesigned_App (00:08.800)

> **Category:** [[08_Modal|Modal]] | **SSIM Fidelity:** `0.9881` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[02_Button|Button]], [[06_Input|Input]], [[01_Card|Card]]

Professional Modal reverse-engineered from d26zVaVJZgM_I_Redesigned_Apps_to_Look_Like_Their_NAMES at 00:08.800. Features FADE_IN_SCALE micro-interaction animation with 12.71:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#1C1A18` | `rgb(28, 26, 24)` | `oklch(0.22 0.005 67.6)` | `45.4%` |
| `surface` | `#80756F` | `rgb(128, 117, 111)` | `oklch(0.57 0.016 50.6)` | `4.6%` |
| `accent` | `#6AB3D9` | `rgb(106, 179, 217)` | `oklch(0.73 0.092 232.6)` | `0.7%` |
| `text` | `#EADACA` | `rgb(234, 218, 202)` | `oklch(0.90 0.028 67.5)` | `3.0%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `66.0 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `1.18`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react'
import { motion } from 'framer-motion'

interface ModalProps {
  isOpen: boolean
  onClose: () => void
  title?: string
  children?: React.ReactNode
}

export const Modal: React.FC<ModalProps> = ({
  isOpen,
  onClose,
  title = 'Modal Title',
  children,
}) => {
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
        className="w-[490px] h-[430px] bg-[#80756F] text-[#EADACA] shadow-2xl relative flex flex-col"
      >
        {/* Header */}
        <div className="flex items-center justify-between px-6 py-4 border-b border-white/10">
          <h2
            id="modal-title"
            className="text-lg font-medium tracking-tight"
          >
            {title}
          </h2>
          <button
            onClick={onClose}
            className="w-8 h-8 rounded flex items-center justify-center hover:bg-white/10 transition-colors"
            
```

## 4. Flutter / Dart Implementation

```dart
import 'package:flutter/material.dart';

class ModalDemo extends StatefulWidget {
  @override
  _ModalDemoState createState() => _ModalDemoState();
}

class _ModalDemoState extends State<ModalDemo> {
  bool _isOpen = false;

  void _toggleModal() => setState(() => _isOpen = !_isOpen);

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      backgroundColor: Color(0xFF1C1A18),
      body: Center(
        child: Column(
          mainAxisAlignment: MainAxisAlignment.center,
          children: [
            ElevatedButton(
              onPressed: _toggleModal,
              style: ElevatedButton.styleFrom(
                backgroundColor: Color(0xFF6AB3D9),
                foregroundColor: Color(0xFF1C1A18),
              ),
              child: Text('Open Modal'),
            ),
            if (_isOpen) _buildModal(),
          ],
        ),
      ),
    );
  }

  Widget _buildModal() {
    return AnimatedOpacity(
      duration: Duration(milliseconds: 200),
      opacity: _isOpen ? 1.0 : 0.0,
      child: AbsorbPointer(
        absorbing: !_isOpen,
        child: ModalBarrier(
          color: Colors.black.withOpacity(0.6),
          dismissible: true,
        ),
      ),
    );
  }
}

class CustomModal extends StatelessWidget {
  final String title;
  final Widget child;
  final VoidCallback onClose;

  const CustomModal({
    Key? key,
    required this
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
