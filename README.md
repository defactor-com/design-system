# Defactor Design System

Live styleguide: **https://brand.defactor.com**

Design tokens, components, and visual guidelines for building consistent Defactor interfaces with AI coding tools.

## Usage with AI Tools

### Lovable / Replit / Bolt

Paste this in your first prompt:

> Follow the design system at https://brand.defactor.com — use Sora font for body, Space Grotesk for headings/numbers, pill-shaped buttons (#5A5BEB primary violet), 16px card radius. Match the colors, spacing, and component patterns shown there.

For best results, screenshot specific sections from the styleguide and attach them to your prompt. These tools respond well to visual references.

### Claude Code / Codex

Copy `CLAUDE.md` from this repo into the root of your project. Claude Code and Codex automatically read this file and will follow the design tokens and component rules defined in it.

```bash
# From your project root
curl -O https://raw.githubusercontent.com/defactor-com/design-system/main/CLAUDE.md
```

That's it — every component Claude or Codex generates will follow the system.
