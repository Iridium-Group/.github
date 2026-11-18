# Iridium Group brand

This folder holds the official Iridium Group mark. Use these files as they are. Do not redraw, trace, or recreate the mark.

## Files

| File                           | Use                                                                                    |
| ------------------------------ | -------------------------------------------------------------------------------------- |
| `iridium-mark.svg`             | The mark on a wide canvas. Use it in README headers and documentation.                 |
| `iridium-mark-square.svg`      | The mark on a square canvas. Use it for icons and anywhere a square shape is expected. |
| `iridium-mark-512.png`         | 512 x 512 raster version of the mark, for places that do not accept SVG.               |
| `iridium-avatar-dark-1024.png` | 1024 x 1024 avatar on a dark background, for the organization and social profiles.     |

In a repository README, place the mark at the top, centered, at a width of 96 pixels:

```html
<p align="center">
  <img src="./.github/assets/iridium-mark.svg" width="96" alt="Iridium Group" />
</p>
```

## Project marks

Projects do not have their own logos. A project mark is the Iridium mark followed by the project name set in type, for example the mark with "iridium-transport" in Space Grotesk beside it.

## Clear space

Keep an empty margin around the mark equal to at least one quarter of its height on every side. Do not place text, borders, or other graphics inside that space.

## Minimum size

Do not display the mark smaller than 16 pixels high on screen. Below 32 pixels, prefer the square file.

## Colors

All Iridium web projects use these design tokens, with exactly these names. The theme is dark-first.

| Token                | Value     | Role                 |
| -------------------- | --------- | -------------------- |
| `--ir-bg`            | `#0B0A12` | Page background      |
| `--ir-surface`       | `#12111C` | Raised surface       |
| `--ir-surface-2`     | `#191726` | Second surface level |
| `--ir-border`        | `#272438` | Default 1px border   |
| `--ir-border-strong` | `#3A3554` | Emphasized border    |
| `--ir-text`          | `#ECEAF6` | Primary text         |
| `--ir-text-muted`    | `#A7A3BD` | Secondary text       |
| `--ir-text-subtle`   | `#6F6A88` | Tertiary text        |
| `--ir-accent`        | `#8B5CF6` | Accent               |
| `--ir-accent-strong` | `#6D28D9` | Strong accent        |
| `--ir-accent-soft`   | `#D9D4FA` | Soft accent          |
| `--ir-steel`         | `#A9ABD0` | Steel neutral        |
| `--ir-ok`            | `#3FB68B` | Success              |
| `--ir-warn`          | `#E0B341` | Warning              |
| `--ir-err`           | `#E5484D` | Error                |
| `--ir-info`          | `#6CA8FF` | Information          |
| `--ir-focus`         | `#B79CFF` | Focus ring           |

Other tokens:

```css
:root {
  --ir-radius: 8px;
  --ir-radius-sm: 6px;
  --ir-font-sans: "Inter", system-ui, -apple-system, "Segoe UI", sans-serif;
  --ir-font-display: "Space Grotesk", "Inter", system-ui, sans-serif;
  --ir-font-mono:
    "JetBrains Mono", ui-monospace, SFMono-Regular, Menlo, monospace;
}
```

An optional light theme uses `#FAF9FE` for the background and `#15131F` for text.

## Style

Dark, refined, technical, and editorial. Use thin 1px borders, small radii, and restrained purple. Use at most one subtle glass surface per page, keep motion minimal, and respect `prefers-reduced-motion`.

## Do not

- Redraw, trace, distort, stretch, or rotate the mark.
- Change the mark's colors, add outlines, shadows, glows, or gradients, or place it on busy images.
- Create new logos or icons for individual projects.
- Combine the mark with another organization's logo in a way that suggests a partnership or endorsement.
- Use neon colors, large gradients, or stock illustrations alongside the mark.
- Use another project's branding, logos, or layouts in Iridium Group material.
