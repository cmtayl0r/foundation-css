# 🎨✨ CSS Foundation

[![Accessibility](https://img.shields.io/badge/WCAG-2.2%20AA-green.svg)](https://www.w3.org/WAI/WCAG22/quickref/)
[![CSS Version](https://img.shields.io/badge/CSS-Module%204%2F5-blue.svg)](https://www.w3.org/Style/CSS/)
[![Color System](https://img.shields.io/badge/Color-OKLCH-purple.svg)](https://oklch.com/)
[![Mobile First](https://img.shields.io/badge/Design-Mobile%20First-ff69b4.svg)](#)
[![Dark Mode](https://img.shields.io/badge/Dark%20Mode-Built%20In-6366f1.svg)](#)
[![Template](https://img.shields.io/badge/GitHub-Template-2ea44f.svg?logo=github)](https://github.com/cmtayl0r/css-foundation)

## 🎯 **What This Does**

An accessibility-first, minimal-bloat Vanilla CSS foundation for my personal React/Next.js projects.

### 👨‍🔧 My objective

Not to recreate Tailwind CSS, but to learn about scalable, usable and pleasurable CSS architectures to make projects more accessible and usable by designers and engineers.

---

## 🚀 Quick Start

### 1. Copy the `styles/` folder to your project

```bash
# In your React/Next.js project root
cp -r styles/ src/styles/
```

### 2. Import in your main CSS/app

```css
/* In your src/index.css or src/app/globals.css */
@import "./styles/index.css";
```

### 3. Choose your color system approach 🌈

#### **Option 🅰️**

- More comprehensive color design token system and layer model
- 11-step scales: 50, 100, 200, 300, 400, 500, 600, 700, 800, 900, 950

```
color-primitives-lean.css
color-semantics-lean.css
```

#### **Option 🅱️**

- Simplified color design tokens for fast prototyping
- 5-step scales: lightest, light, default, dark, darkest

```
color-primitives-lean.css
color-semantics-lean.css
```

> [!IMPORTANT]
> Select/Delete relevant files as appropriate.

### 4. Customize your brand (optional)

```css
/* In styles/tokens/color-primitives.css */
:root {
  --brand-hue: 240; /* Your brand hue (0-360°) */
  --brand-chroma: 0.28; /* Adjust for your brand intensity */
}

/* Same for secondary, error, success, etc */
```

---

## 🎯 What You Get

- ✅ **WCAG 2.2 AA/AAA compliant** accessibility system
- ✅ **OKLCH color system** with hex fallbacks
- ✅ **Modern CSS features** (container queries, logical properties)
- ✅ **7-step spacing scale** (no bloat)
- ✅ **Mobile-first responsive** design
- ✅ **Dark mode** and high contrast support
- ✅ **Layout primitives** (Stack, Grid, Cluster, etc.)
- ✅ **React integration** pattern demos

## 📁 File Organization

- `tokens/` - Design system tokens foundation
- `foundation/` - Reset and base styles
- `accessibility/` - Complete a11y system
- `utilities/` - Essential utility classes
- `components/` - Layout primitives and basic global components

## 🔧 Framework Integration

### React + Vite

```jsx
// src/main.tsx
import "./styles/index.css";
import "./index.css"; // Your custom styles
```

### Next.js

```jsx
// src/app/layout.tsx
import "./globals.css"; // Contains @import "./styles/index.css"
```

## 🎨 Usage Examples

### Button with Full Accessibility

```jsx
<button className="interactive-primary touch-target focus-visible-only">
  Submit
</button>
```

### Accessible Form

```jsx
<input
  className="touch-target focus-visible-only"
  aria-invalid={hasError}
  aria-describedby="field-help"
/>
<div id="field-help" className="sr-only">
  {hasError ? 'Error message' : 'Help text'}
</div>
```

### Layout Primitives

```jsx
<div className="stack stack--comfortable">
  <div className="cluster cluster--space">
    <h1>Title</h1>
    <button>Action</button>
  </div>
  <div className="grid grid--cards">{/* Cards */}</div>
</div>
```

---

## 🚫 What This ISN'T

- ❌ Not a component library
- ❌ Not Tailwind CSS
- ❌ Not a complete design system
- ❌ Not framework-specific

## ✅ What This IS

- ✅ **Foundation to build on**
- ✅ **CSS Module compatible**
- ✅ **Zero JavaScript dependencies**
- ✅ **Production-ready patterns**
- ✅ **Accessibility-first approach**

---

## 📄 **Details**

[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Size](https://img.shields.io/badge/Size-~15KB%20gzipped-brightgreen.svg)](#)
[![Built with Love](https://img.shields.io/badge/Built%20with-❤️%20and%20☕-red.svg)](#)

---

## 👋 **Connect**

Built by Chris Taylor - Design Engineer specializing in accessible AI

- 💼 LinkedIn: [Chris Taylor](https://www.linkedin.com/in/uxchristophertaylor/)
<!-- - 🌐 Portfolio: [apathofbravery.com](http://www.apathofbravery.com) -->
- 📧 Email: [chris@pathtobravery.dev](mailto:chris@pathtobravery.dev)

---

_"Making technology that works for everyone isn't just good practice—it's better business, better design, and better for humanity."_
