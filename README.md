# Design Prompts

<p align="center">
  <img src="https://img.shields.io/badge/styles-30-green?style=for-the-badge" alt="30 Styles">
  <img src="https://img.shields.io/badge/license-MIT-blue?style=for-the-badge" alt="MIT License">
  <img src="https://img.shields.io/badge/framework-agnostic-purple?style=for-the-badge" alt="Framework Agnostic">
</p>

> 30 curated design style prompts for frontend projects - apply beautiful, production-ready design systems to React, Vue, or any frontend project.

## ✨ What is this?

**Design Prompts** is a comprehensive collection of 30 curated design system prompts for frontend development. Each style includes complete design specifications covering:

- 🎨 **Color palette** - Exact hex codes with semantic naming
- 🔤 **Typography** - Fonts, sizes, weights, line heights
- 📏 **Spacing** - Consistent spacing system (4px base grid)
- 🌑 **Shadows & Effects** - Depth, glows, blurs, borders
- 🧩 **Component patterns** - Buttons, cards, inputs, modals
- ✨ **Animations** - Transitions, micro-interactions, easing

## 📚 Style Catalog (30 Styles)

### 🎯 By Use Case

#### Corporate & Business
| Style | Theme | Best For |
|-------|-------|----------|
| SaaS | Light | Startups, Web apps, Dashboards |
| Enterprise | Light | B2B SaaS, Admin panels, CRM |
| Professional | Light | Consulting, Legal, Finance |
| Swiss Minimalist | Light | Architecture, Design agencies |

#### Modern & Tech
| Style | Theme | Best For |
|-------|-------|----------|
| Modern Dark | Dark | Developer tools, IDEs, Gaming |
| Minimal Dark | Dark | Mobile apps, Subscriptions |
| Web3 | Dark | Crypto, DeFi, Blockchain |
| Terminal | Dark | CLI tools, Documentation |
| Cyberpunk | Dark | Games, Sci-fi, Hacking themes |

#### Retro & Nostalgia
| Style | Theme | Best For |
|-------|-------|----------|
| Retro | Light | 90s nostalgia, Personal sites |
| Vaporwave | Dark | Music, Art, Experimental |
| Newsprint | Light | Blogs, Editorial, Magazine |
| Academia | Light | Educational, Research, Library |

#### Elegant & Luxurious
| Style | Theme | Best For |
|-------|-------|----------|
| Luxury | Light | High-end brands, Jewelry, Fashion |
| Monochrome | Light | Editorial, Portfolio, Art |
| Art Deco | Dark | Gatsby-style, Wedding, Premium |
| Botanical | Light | Wellness, Nature, Eco-friendly |

#### Creative & Bold
| Style | Theme | Best For |
|-------|-------|----------|
| Neo Brutalism | Light | Portfolio, Landing pages, MVP |
| Bauhaus | Light | Creative agencies, Art galleries |
| Kinetic | Dark | Motion graphics, Entertainment |
| Bold Typography | Dark | Posters, Headlines, Branding |
| Maximalism | Dark | E-commerce, Marketplace, Festival |

#### Playful & Friendly
| Style | Theme | Best For |
|-------|-------|----------|
| Playful Geometric | Light | Kids, Education, Lifestyle |
| Claymorphism | Light | Mobile apps, Consumer apps |
| Sketch | Light | Handmade, Artisan, Creative |

#### Minimal & Clean
| Style | Theme | Best For |
|-------|-------|----------|
| Flat Design | Light | Government, Healthcare, Utility |
| Neumorphism | Light | IoT dashboards, Settings |
| Organic | Light | Sustainability, Organic food |
| Material Design | Light | Android apps, Productivity |

#### Industrial
| Style | Theme | Best For |
|-------|-------|----------|
| Industrial | Light | Hardware, Electronics, Engineering |

## 🚀 Quick Start

### Option 1: Via skills CLI (Recommended)

```bash
npx skills add wangpf1129/design-prompts
```

### Option 2: Manual Install

```bash
# Clone the repository
git clone https://github.com/wangpf1129/design-prompts.git

# Copy to your agents skills directory
cp -r design-prompts ~/.agents/skills/
```

### Usage with AI Agent

```
You: I want to build a landing page for a indie game store
Agent: I'll use the Neo Brutalism style for your game store - it fits the indie/creative vibe perfectly. Let me apply the design system...
```

## 💡 How It Works

```
┌─────────────────────────────────────────────────────────┐
│                    Your Request                         │
│  "Build a dashboard for my SaaS analytics tool"        │
└─────────────────────┬───────────────────────────────────┘
                      ▼
┌─────────────────────────────────────────────────────────┐
│              Style Matching Engine                      │
│  • Analyzes project type, audience, goals              │
│  • Matches against 30 style metadata                   │
│  • Returns best-fit style(s)                           │
└─────────────────────┬───────────────────────────────────┘
                      ▼
┌─────────────────────────────────────────────────────────┐
│            Load Design System                           │
│  references/enterprise.md → Colors, Fonts, Spacing     │
└─────────────────────┬───────────────────────────────────┘
                      ▼
┌─────────────────────────────────────────────────────────┐
│           Apply to Your Codebase                        │
│  • CSS Variables / Tailwind Config                     │
│  • Component patterns                                   │
│  • Consistent design tokens                             │
└─────────────────────────────────────────────────────────┘
```

## 📖 Practical Guide

### When to Use What?

| Your Project | Recommended Style | Why |
|--------------|------------------|-----|
| E-commerce store | SaaS, Enterprise | Trust, conversion-focused |
| Developer tool | Terminal, Modern Dark | Familiar, productive |
| Portfolio | Neo Brutalism, Sketch | Stand out, creative |
| Blog/Magazine | Newsprint, Professional | Readable, editorial |
| Game/Gaming | Cyberpunk, Kinetic | Immersive, exciting |
| Crypto/DeFi | Web3, Minimal Dark | Modern, trustworthy |
| Luxury brand | Luxury, Art Deco | Premium, elegant |
| Mobile app | Claymorphism, Material | Touch-friendly |
| Landing page | Neo Brutalism, Bold Typography | Attention-grabbing |

### Example: Applying a Style

```css
/* 1. Load tokens from references/[style].md */
:root {
  /* Neo Brutalism */
  --bg: #FFF9F0;
  --text: #000;
  --primary: #FF4D4D;
  --secondary: #FFF056;
  --border: 4px solid #000;
  --shadow: 6px 6px 0 #000;
  --font-display: 'Space Grotesk', sans-serif;
}

/* 2. Apply to components */
.card {
  background: var(--secondary);
  border: var(--border);
  box-shadow: var(--shadow);
  font-family: var(--font-display);
  padding: 1.5rem;
}
```

### Tailwind Example

```js
// tailwind.config.js
module.exports = {
  theme: {
    extend: {
      colors: {
        // From references/modern-dark.md
        background: '#0a0a0f',
        primary: '#00ffff',
        secondary: '#ff00ff',
        surface: '#151520',
      },
      fontFamily: {
        mono: ['JetBrains Mono', 'monospace'],
      },
    },
  },
}
```

## 📁 Project Structure

```
design-prompts/
├── README.md              # This file
├── SKILL.md               # OpenClaw skill definition
├── .gitignore
├── references/            # Complete design systems
│   ├── monochrome.md      # ~500 lines per file
│   ├── bauhaus.md
│   ├── cyberpunk.md
│   ├── neo-brutalism.md
│   └── ... (30 total)
└── LICENSE
```

## 🔧 Framework Support

| Framework | How to Use |
|-----------|------------|
| React + Tailwind | Extract colors to `tailwind.config.js` |
| Vue | Add to `App.vue` CSS variables |
| Plain HTML/CSS | Import `references/*.md` CSS directly |
| Next.js | Add to `globals.css` |
| Svelte | Add to `<style:global>` |
| React Native | Map colors to platform tokens |

## ⚡️ Comparison

| Feature | ad-hoc prompting | design-prompts |
|---------|------------------|----------------|
| Consistency | ❌ Variable | ✅ Fixed design system |
| Completeness | ⚠️ Partial | ✅ Full tokens + components |
| Speed | ❌ Iterative | ✅ Direct application |
| Style variety | Limited | 30 curated styles |
| Reference docs | ❌ None | ✅ 30 detailed guides |

## 🙏 Credits & Inspiration

Heavily inspired by **[designprompts.dev](https://www.designprompts.dev/)** - a viral Twitter/X resource for AI-driven design prompts.

This collection expands on the original concept:
- Complete, production-ready specifications
- Multiple output formats (CSS, Tailwind, etc.)
- OpenClaw agent integration
- 30 carefully curated styles (vs ~10 original)

## 🏆 Live Demos

Real projects built with this skill:

| Project | Description | Style |
|---------|-------------|-------|
| [niji-dream](https://dream.hottotech.co.jp/) | AI Dream Interpreter | Neo Brutalism |
| [niji-fortune](https://fortune.hottotech.co.jp/) | Daily Fortune Teller | Cyberpunk |
| [niji-mbti](https://mbti.hottotech.co.jp/) | MBTI Personality Test | Claymorphism |

---

<p align="center">Made with ❤️ for the frontend community</p>