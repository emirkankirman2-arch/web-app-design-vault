---
title: "Modal — uMPzaz3BX4c_Grid_to_Fullscre (00:02.402)"
description: "Modal UI component (recon_uMPzaz3BX4c_Grid_to_Fullscreen_with_FLIP_SUMMARY_from_Super_Mario_) with SSIM 0.9946, OKLCH design tokens, SLIDE_DOWN motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_uMPzaz3BX4c_Grid_to_Fullscreen_with_FLIP_SUMMARY_from_Super_Mario_64_3D__s1_00_modal"
category: "Modal"
ssim: 0.9946
quality_score: 8.72
tags: [modal, ui-design, design-tokens, react, flutter]
---

# Modal — uMPzaz3BX4c_Grid_to_Fullscre (00:02.402)

> **Category:** [[08_Modal|Modal]] | **SSIM Fidelity:** `0.9946` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[02_Button|Button]], [[06_Input|Input]], [[01_Card|Card]]

Professional Modal reverse-engineered from uMPzaz3BX4c_Grid_to_Fullscreen_with_FLIP_SUMMARY_from_Super_Mario_64_3D_ at 00:02.402. Features SLIDE_DOWN micro-interaction animation with 7.94:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#26272B` | `rgb(38, 39, 43)` | `oklch(0.27 0.007 274.7)` | `44.6%` |
| `surface` | `#F5B10E` | `rgb(245, 177, 14)` | `oklch(0.80 0.164 80.3)` | `43.3%` |
| `accent` | `#CC9719` | `rgb(204, 151, 25)` | `oklch(0.71 0.140 82.2)` | `0.4%` |
| `text` | `#F5B10E` | `rgb(245, 177, 14)` | `oklch(0.80 0.164 80.3)` | `43.3%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `SLIDE_DOWN`
- **Measured Duration:** `48.048 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.01`

## 3. React + TypeScript + Tailwind Implementation

```tsx
// React TypeScript + Tailwind CSS + Framer Motion
// Reconstructed Modal component based on video evidence
// Source: uMPzaz3BX4c_Grid_to_Fullscreen_with_FLIP_SUMMARY_from_Super_Mario_64_3D_.mp4

import React from 'react'
import { motion, AnimatePresence } from 'framer-motion'

interface ModalProps {
  isOpen: boolean
  onClose: () => void
  children?: React.ReactNode
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
            transition={{ duration: 0.2 }}
            className="fixed inset-0 bg-black/60 backdrop-blur-sm z-50"
            onClick={onClose}
            role="dialog"
            aria-modal="true"
          />

          {/* Modal Container */}
          <motion.div
            initial={{ opacity: 0, y: -8.077302932739258 }}
            animate={{ opacity: 1, y: 0 }}
            exit={{ opacity: 0, y: -8.077302932739258 }}
            transition={{ duration: 48.05, ease: [0.16, 1, 0.3, 1] }}
            className="fixed left-1/2 top-1/2 -translate-x-1/2 -translate-y-1/2 w-[832px] h-[701px] bg-[#F5B10E] rounded-[28px] shadow-2xl z-50 flex items-center justify-center"
            role="document"
          >
            {/* Close Button */}
            <button
              onClick={onClose}
              className="absolute top-6 right-6 text-[#26272B] hover:text-[#CC9719] transition-colors"
              aria
```

## 4. Flutter / Dart Implementation

```dart
// Flutter StatefulWidget
// Reconstructed Modal component based on video evidence

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
      backgroundColor: Color(0xFF26272B),
      body: Center(
        child: Column(
          mainAxisAlignment: MainAxisAlignment.center,
          children: [
            ElevatedButton(
              onPressed: _toggleModal,
              style: ElevatedButton.styleFrom(
                backgroundColor: Color(0xFFF5B10E),
                foregroundColor: Color(0xFF26272B),
                shape: RoundedRectangleBorder(borderRadius: BorderRadius.circular(8)),
              ),
              child: Text('Open Modal'),
            ),
            if (_isOpen)
              ModalOverlay(
                onClose: _toggleModal,
                child: BigKWidget(),
              ),
          ],
        ),
      ),
    );
  }
}

class ModalOverlay extends StatelessWidget {
  final VoidCallback onClose;
  final Widget child;

  const ModalOverlay({Key? key, required this.onClose, required this.child}) : super(key: key);

  @override
  Widget build(Bu
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
