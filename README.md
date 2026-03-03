# Design Prompts

<p align="center">
  <img src="https://img.shields.io/badge/styles-30-green?style=for-the-badge" alt="30 Styles">
  <img src="https://img.shields.io/badge/license-MIT-blue?style=for-the-badge" alt="MIT License">
  <img src="https://img.shields.io/badge/openclaw-compatible-orange?style=for-the-badge" alt="OpenClaw">
</p>

> 30 curated design style prompts for frontend projects - apply beautiful, production-ready design systems to React, Vue, or any frontend project.

## ✨ What is this?

**Design Prompts** is a comprehensive collection of 30 curated design system prompts for frontend development. Each style includes complete design specifications covering:

- 🎨 **Color palette** - Exact hex codes
- 🔤 **Typography** - Fonts, sizes, weights, line heights
- 📏 **Spacing** - Consistent spacing system
- 🌑 **Shadows & Effects** - Depth, glows, blurs
- 🧩 **Component patterns** - Buttons, cards, inputs, etc.
- ✨ **Animations** - Transitions, micro-interactions

## 📚 Available Styles (30)

### Corporate & Professional

| Style | Theme | Description |
|-------|-------|-------------|
| SaaS | Light | Bold minimalist with Electric Blue gradients |
| Professional | Light | Editorial minimalist, elegant serif, ivory background |
| Enterprise | Light | Modern SaaS, indigo/violet gradients |
| Swiss Minimalist | Light | International Typographic Style, mathematical grids |

### Modern & Tech

| Style | Theme | Description |
|-------|-------|-------------|
| Modern Dark | Dark | Cinematic dark mode with ambient lighting & micro-interactions |
| Minimal Dark | Dark | Deep slate, warm amber, glass cards |
| Web3 | Dark | Bitcoin orange, glowing elements, data visualization |
| Cyberpunk | Dark | Neon on black, glitch animations, terminal fonts |
| Terminal | Dark | Retro command-line interface aesthetic |

### Retro & Vintage

| Style | Theme | Description |
|-------|-------|-------------|
| Retro | Light | 90s nostalgia, Windows 95 beveled UI |
| Vaporwave | Dark | 80s retro-futurism, neon pinks & cyans |
| Newsprint | Light | Newspaper aesthetic, high contrast, tight grids |
| Academia | Light | University aesthetic, warm paper textures |

### Elegant & Premium

| Style | Theme | Description |
|-------|-------|-------------|
| Luxury | Light | Elegant serif, gold accents, ultra-slow animations |
| Monochrome | Light | Stark editorial design, pure black & white |
| Art Deco | Dark | 1920s Gatsby elegance, geometric precision |
| Botanical | Light | Nature-inspired, organic shapes, earth tones |

### Bold & Creative

| Style | Theme | Description |
|-------|-------|-------------|
| Neo Brutalism | Light | Raw, high-contrast, cream background, thick borders |
| Bauhaus | Light | Bold geometric modernism with primary colors |
| Kinetic | Dark | Motion-first design with infinite marquees |
| Bold Typography | Dark | Massive typography as primary visual element |
| Maximalism | Dark | Clashing patterns, dense layouts, MORE IS MORE |

### Playful & Fun

| Style | Theme | Description |
|-------|-------|-------------|
| Playful Geometric | Light | Vibrant geometric decorations, Memphis design |
| Claymorphism | Light | 3D inflatable clay objects, candy colors |
| Sketch | Light | Hand-drawn, wobbly borders, paper textures |
| Neo Brutalism | Light | Raw, high-contrast, cream background, thick borders |

### Minimal & Clean

| Style | Theme | Description |
|-------|-------|-------------|
| Flat Design | Light | Pure color, typography, and layout |
| Neumorphism | Light | Extruded elements via dual shadows |
| Organic | Light | Earth palette, blob shapes, wabi-sabi warmth |
| Material Design | Light | Google's Material Design 3 enhanced |

### Industrial

| Style | Theme | Description |
|-------|-------|-------------|
| Industrial | Light | Dieter Rams inspired, tactile neumorphic elements |

## 🚀 Quick Start

### 1. Choose a Style

Browse the 30 styles above and pick one that matches your project vibe.

### 2. Load the Reference

Each style has a detailed reference file in `references/`:
- `references/neo-brutalism.md`
- `references/cyberpunk.md`
- `references/claymorphism.md`
- ...and 27 more!

### 3. Apply to Your Project

Read the reference file and extract:
- Colors → CSS variables or Tailwind config
- Typography → Font families, sizes
- Spacing → Gap/margin scale
- Effects → Box shadows, borders

### Example: Neo Brutalism

```css
/* From references/neo-bralism.md */
:root {
  --color-background: #FFF9F0;
  --color-primary: #FF4D4D;
  --color-secondary: #FFF056;
  --color-text: #000000;
  --border-width: 4px;
  --shadow-offset: 6px;
}

.btn {
  background: var(--color-secondary);
  border: var(--border-width) solid var(--color-text);
  box-shadow: var(--shadow-offset) var(--shadow-offset) 0 var(--color-text);
  font-family: 'Space Grotesk', sans-serif;
  font-weight: 700;
  padding: 12px 24px;
}
```

### Example: Cyberpunk (Tailwind)

```js
// From references/cyberpunk.md
const cyberpunkTheme = {
  colors: {
    background: '#0a0a0f',
    primary: '#00ffff',
    secondary: '#ff00ff',
    accent: '#ffff00',
  },
  fontFamily: {
    mono: ['JetBrains Mono', 'monospace'],
  },
  boxShadow: {
    neon: '0 0 10px #00ffff, 0 0 20px #00ffff',
  },
}
```

## 📁 Project Structure

```
design-prompts/
├── README.md              # This file
├── SKILL.md               # OpenClaw skill format
├── .gitignore
├── references/            # Detailed style references
│   ├── monochrome.md
│   ├── bauhaus.md
│   ├── modern-dark.md
│   ├── cyberpunk.md
│   ├── neo-brutalism.md
│   ├── claymorphism.md
│   └── ... (30 total)
└── LICENSE
```

## 🤖 OpenClaw Integration

This skill is designed for [OpenClaw](https://github.com/openclaw/openclaw) AI assistants.

### Install

```bash
# Copy to your skills directory
cp -r design-prompts ~/.agents/skills/
```

### Usage

When working with an OpenClaw agent:

1. Tell the agent your desired style: "Use neo-brutalism style"
2. The agent will load `references/neo-brutalism.md`
3. Apply the design system to your project

### Triggers

This skill activates when you mention:
- Design style names (neo-brutalism, cyberpunk, etc.)
- Keywords: "design style", "UI aesthetic", "front-end design"
- Style categories: "modern", "retro", "minimal", "playful"

## 📖 Style Guide

### Choosing the Right Style

**Corporate/Business:**
- SaaS, Professional, Enterprise, Swiss Minimalist

**Creative/Artistic:**
- Bauhaus, Art Deco, Maximalism, Sketch

**Modern/Tech:**
- Modern Dark, Minimal Dark, Web3, Cyberpunk, Terminal

**Retro/Vintage:**
- Retro, Vaporwave, Newsprint, Academia

**Playful/Fun:**
- Neo Brutalism, Playful Geometric, Claymorphism

**Elegant/Premium:**
- Luxury, Monochrome, Botanical

**Nature/Organic:**
- Botanical, Organic

**Industrial/Technical:**
- Industrial, Material Design, Flat Design

**Experimental:**
- Kinetic, Neumorphism

## 🙏 Credits & Inspiration

This project is **heavily inspired by [designprompts.dev](https://www.designprompts.dev/)** - a popular resource that went viral on Twitter/X for providing AI-driven design prompts for frontend projects.

The original designprompts.dev collection sparked the idea for this comprehensive skill, which expands on those concepts with:

- Complete, production-ready design specifications
- Multiple output formats (CSS, Tailwind, etc.)
- OpenClaw agent integration
- 30 carefully curated styles (vs. the original ~10)

## 🔧 Tech Stack Compatibility

All style references are framework-agnostic and can be used with:

- **React** - Tailwind, Styled Components, CSS Modules
- **Vue** - Tailwind, SCSS, Composition API
- **Plain HTML/CSS** - Any CSS methodology
- **Next.js / Nuxt** - Full-stack frameworks
- **Svelte** - Component-based styling
- **Mobile** - React Native, Flutter

## 📄 License

MIT License - feel free to use in your projects!

---

<p align="center">Made with ❤️ for the frontend community</p>