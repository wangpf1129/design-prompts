# Design Prompts

> 30 curated design style prompts for frontend projects

Apply beautiful, production-ready design systems to your React, Vue, or any frontend project. Each style includes comprehensive design specs covering colors, typography, spacing, effects, and component patterns.

## Available Styles (30)

| # | Style | Theme | Description |
|---|-------|-------|-------------|
| 1 | Monochrome | Light | Stark editorial design, pure black & white, oversized serif typography |
| 2 | Bauhaus | Light | Bold geometric modernism with primary colors |
| 3 | Modern Dark | Dark | Cinematic dark mode with ambient lighting & micro-interactions |
| 4 | Newsprint | Light | Newspaper aesthetic, high contrast, tight grids |
| 5 | SaaS | Light | Bold minimalist with Electric Blue gradients |
| 6 | Luxury | Light | Elegant serif, gold accents, ultra-slow animations |
| 7 | Terminal | Dark | Retro command-line interface aesthetic |
| 8 | Swiss Minimalist | Light | International Typographic Style, mathematical grids |
| 9 | Kinetic | Dark | Motion-first design with infinite marquees |
| 10 | Flat Design | Light | Pure color, typography, and layout |
| 11 | Art Deco | Dark | 1920s Gatsby elegance, geometric precision |
| 12 | Material Design | Light | Google's Material Design 3 enhanced |
| 13 | Neo Brutalism | Light | Raw, high-contrast, cream background, thick borders |
| 14 | Bold Typography | Dark | Massive typography as primary visual element |
| 15 | Academia | Light | University aesthetic, warm paper textures |
| 16 | Cyberpunk | Dark | Neon on black, glitch animations, terminal fonts |
| 17 | Web3 | Dark | Bitcoin orange, glowing elements, data visualization |
| 18 | Playful Geometric | Light | Vibrant geometric decorations, Memphis design |
| 19 | Minimal Dark | Dark | Deep slate, warm amber, glass cards |
| 20 | Claymorphism | Light | 3D inflatable clay objects, candy colors |
| 21 | Professional | Light | Editorial minimalist, elegant serif, ivory background |
| 22 | Botanical | Light | Nature-inspired, organic shapes, earth tones |
| 23 | Vaporwave | Dark | 80s retro-futurism, neon pinks & cyans |
| 24 | Enterprise | Light | Modern SaaS, indigo/violet gradients |
| 25 | Sketch | Light | Hand-drawn, wobbly borders, paper textures |
| 26 | Industrial | Light | Dieter Rams inspired, tactile neumorphic elements |
| 27 | Neumorphism | Light | Extruded elements via dual shadows |
| 28 | Organic | Light | Earth palette, blob shapes, wabi-sabi warmth |
| 29 | Maximalism | Dark | Clashing patterns, dense layouts, MORE IS MORE |
| 30 | Retro | Light | 90s nostalgia, Windows 95 beveled UI |

## Usage

Each style has a dedicated reference file in `references/` containing:
- Color palette (hex codes)
- Typography specs (fonts, sizes, weights)
- Spacing system
- Shadow & effect definitions
- Component patterns
- Animation specs

### Example: Applying Neo Brutalism

1. Read `references/neo-brutalism.md`
2. Extract design tokens (colors, fonts, shadows)
3. Apply to your components

```css
/* Neo Brutalism Example */
.btn {
  background: #FFF056;
  border: 4px solid #000;
  box-shadow: 6px 6px 0 #000;
  font-family: 'Space Grotesk', sans-serif;
  font-weight: 700;
}
```

## Inspired By

Originally inspired by [designprompts.dev](https://www.designprompts.dev/) - a popular resource for AI-driven design prompts.

## License

MIT

---

Built for OpenClaw agents. Use with any frontend framework.