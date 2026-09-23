# Obsidian UI Lab

Reusable Markdown layouts and CSS components for making Obsidian more visual.

Obsidian UI Lab is a growing collection of small, copy-friendly UI components for Obsidian. Each component includes a working example, the required CSS, and simple customization guidance.

---

## Current Components

### 🎨 Color Swatch Cards

A responsive card grid for displaying color palettes and reference values inside Obsidian.

**Features**

- Responsive grid layout
- Clean card design
- Supports custom colors and CSS variables
- Works with native HTML inside Obsidian notes
- Light and dark theme friendly
- No third-party plugins required

**Files**

```
01 - Color UI/
└── Color Swatch Cards.md

.obsidian/
└── snippets/
    ├── custom-colors.css
    └── color-swatch-cards.css
```

---

## Shared Theme

The project includes a reusable color system in:

```
.obsidian/snippets/custom-colors.css
```

It provides shared color variables and utility classes that can be reused across future components such as cards, chat interfaces, dashboards, trackers, and other UI elements.

Examples:

```
color: var(--ui-purple);
background: var(--ui-soft-purple);
```

You can use the provided palette or replace it with your own colors.

---

## Installation

You can either:

- Clone or download the entire vault
- Copy individual components into an existing Obsidian vault

Full setup instructions are available in:

```
00 - Start Here/How to Install.md
```

---

## Project Structure

```
obsidian-ui-lab/
│
├── README.md
├── .gitignore
│
├── 00 - Start Here/
│   ├── How to Install.md
│   └── Custom Colors.md
│
├── 01 - Color UI/
│   └── Color Swatch Cards.md
│
└── .obsidian/
    └── snippets/
        ├── custom-colors.css
        └── color-swatch-cards.css
```

The project is intentionally starting small and will grow component by component.

---

## Planned Components

Future additions may include:

- Chat bubbles and message layouts
- Replies and reactions
- Image galleries
- Cards
- Journaling layouts
- Trackers
- Dashboards
- Navigation elements
- Creative writing UI
- Fun interface-inspired components

---

## Philosophy

The goal is to keep each component:

- Easy to understand
- Easy to copy
- Easy to customize
- Independent where possible
- Consistent with the rest of the vault

No giant theme required.

Use only the pieces you want.

---

More components coming soon.