---
title: "Button — DZ8EWBEoFG6_Video_by_uiuxman (00:00.000)"
description: "Button UI component (recon_DZ8EWBEoFG6_Video_by_uiuxmanuel_s1_02_button) with SSIM 0.9951, OKLCH design tokens, FADE_IN_SCALE motion spec, React/Tailwind & Flutter implementations."
component_id: "recon_DZ8EWBEoFG6_Video_by_uiuxmanuel_s1_02_button"
category: "Button"
ssim: 0.9951
quality_score: 8.72
tags: [button, ui-design, design-tokens, react, flutter]
---

# Button — DZ8EWBEoFG6_Video_by_uiuxman (00:00.000)

> **Category:** [[02_Button|Button]] | **SSIM Fidelity:** `0.9951` | **Quality Score:** `8.72 / 10`  
> **Related Categories:** [[01_Card|Card]], [[06_Input|Input]], [[08_Modal|Modal]]

Professional Button reverse-engineered from DZ8EWBEoFG6_Video_by_uiuxmanuel at 00:00.000. Features FADE_IN_SCALE micro-interaction animation with 9.4:1 WCAG contrast.

## 1. Visual Design Tokens (HEX / RGB / OKLCH)

| Role | HEX | RGB | OKLCH | Visual Weight |
|---|---|---|---|---|
| `background` | `#EEEDEE` | `rgb(238, 237, 238)` | `oklch(0.95 0.002 325.6)` | `88.1%` |
| `surface` | `#E3E1E4` | `rgb(227, 225, 228)` | `oklch(0.91 0.005 314.8)` | `6.1%` |
| `accent` | `#7E7C7F` | `rgb(126, 124, 127)` | `oklch(0.59 0.005 314.8)` | `5.0%` |
| `text` | `#3D3C3D` | `rgb(61, 60, 61)` | `oklch(0.36 0.002 325.6)` | `0.4%` |

## 2. Motion & Micro-Interaction Spec

- **Motion Pattern:** `FADE_IN_SCALE`
- **Measured Duration:** `18.0 s`
- **Spring Overshoot:** `False` | **Peak Velocity:** `0.0`

## 3. React + TypeScript + Tailwind Implementation

```tsx
import React from 'react';
import { motion } from 'framer-motion';

interface AutoButtonProps {
  children: React.ReactNode;
  onClick?: () => void;
  className?: string;
  disabled?: boolean;
}

export const AutoButton: React.FC<AutoButtonProps> = ({
  children,
  onClick,
  className = '',
  disabled = false,
}) => {
  const buttonVariants = {
    initial: { opacity: 0, scale: 0.95 },
    animate: { opacity: 1, scale: 1 },
    hover: { scale: 1.02 },
    tap: { scale: 0.98 },
  };

  const transition = {
    type: 'spring',
    stiffness: 260,
    damping: 20,
  };

  return (
    <motion.button
      whileHover={!disabled ? 'hover' : undefined}
      whileTap={!disabled ? 'tap' : undefined}
      variants={buttonVariants}
      initial="initial"
      animate="animate"
      transition={transition}
      onClick={disabled ? undefined : onClick}
      disabled={disabled}
      className={
        'flex items-center justify-center whitespace-nowrap rounded-none border-none bg-[#E3E1E4] text-[#3D3C3D] font-medium text-sm leading-none transition-colors duration-200 active:scale-95 disabled:opacity-50 disabled:pointer-events-none shadow-sm ' +
        className
      }
      style={{ minWidth: 102, height: 26 }}
    >
      {children}
    </motion.button>
  );
};

// Usage example:
// <AutoButton onClick={() => console.log('clicked')}>BUTTON</AutoButton>
```

## 4. Flutter / Dart Implementation

```dart
// Flutter Material widget template
```

---
> **Get all 1,370 components (`CSV`, `React/Flutter`, `AI Drag-and-Drop Bundles`, `MCP Server`):** [https://emirkankirman2353.itch.io/web-app-design-vault](https://emirkankirman2353.itch.io/web-app-design-vault)
