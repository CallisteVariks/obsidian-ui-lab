# Obsidian UI Lab

[![License: MIT](https://img.shields.io/badge/License-MIT-purple.svg)](LICENSE)
[![Release](https://img.shields.io/github/v/release/CallisteVariks/obsidian-ui-lab?color=8b5cf6)](https://github.com/CallisteVariks/obsidian-ui-lab/releases)

> Reusable Markdown layouts and CSS components for making Obsidian more visual.

Obsidian UI Lab is a growing collection of small, copy-friendly UI components for Obsidian. Each component includes a working example, the required CSS, and simple customization guidance.

Use the whole vault as a playground, or copy only the components you want.

**No giant theme. No unnecessary plugins. Just reusable pieces.**

---

## ✨ Components

### 🎨 Color Swatch Cards

A responsive card grid for displaying color palettes and reference values inside Obsidian.

![Color Swatch Cards](assets/screenshots/color-swatch-cards.png)

**Features**

- Responsive grid layout
- Clean card design
- Supports custom colors and CSS variables
- Works with native HTML inside Obsidian notes
- Light and dark theme friendly
- No third-party plugins required

[View component →](01%20-%20Color%20UI/Color%20Swatch%20Cards.md)

---

### 📋 Color Reference Table

A compact visual reference table for displaying color swatches and structured data.

![Color Reference Table](assets/screenshots/color-reference-table.png)

The underlying table component is intentionally generic and can also be adapted for:

- Design tokens
- Project references
- Status lists
- Inventories
- Structured datasets

[View component →](01%20-%20Color%20UI/Color%20Reference%20Table.md)

---

### 💬 Basic Chat Bubbles

A simple chat-style conversation using native Obsidian callouts.

![Basic Chat Bubbles](assets/screenshots/basic-chat-bubbles.png)

**Features**

- Left and right message bubbles
- Message tails
- Timestamps
- Read receipts
- Date separators
- Responsive message width
- Scrollbar fixes for Obsidian callouts
- No third-party plugins required

[View component →](02%20-%20Chat%20UI/Basic%20Chat%20Bubbles.md)

The chat system will grow modularly with replies, images, galleries, and reactions.

---

## 🚀 Quick Start

### Use the whole vault

Clone the repository:

```bash
git clone https://github.com/CallisteVariks/obsidian-ui-lab.git
```

Then open the cloned folder as a vault in Obsidian.

### Use only one component

Each component page tells you exactly which CSS snippet it needs.

CSS snippets live in:

```text
.obsidian/snippets/
```

Copy the required snippet into the same folder in your own vault, then enable it under:

**Settings → Appearance → CSS snippets**

For complete instructions:

[Read the installation guide →](00%20-%20Start%20Here/How%20to%20Install.md)

---

## 🎨 Shared Color System

Obsidian UI Lab includes an optional shared color system:

```text
.obsidian/snippets/custom-colors.css
```

Components can reference reusable variables such as:

```css
var(--ui-purple)
var(--ui-soft-purple)
var(--ui-blue)
var(--ui-green)
```

For example:

```css
color: var(--ui-purple);
background: var(--ui-soft-purple);
```

The shared palette helps components feel consistent, but components are designed to remain customizable and independent wherever possible.

[View custom colors →](00%20-%20Start%20Here/Custom%20Colors.md)

---

## 🧩 CSS Snippets

Current snippets:

```text
.obsidian/snippets/
├── custom-colors.css
├── color-swatch-cards.css
├── reference-table.css
└── chat-core.css
```

Dependencies and available classes are documented here:

[CSS Snippets →](00%20-%20Start%20Here/CSS%20Snippets.md)

---

## 📁 Project Structure

```text
obsidian-ui-lab/
│
├── README.md
├── .gitignore
│
├── assets/
│   └── screenshots/
│
├── 00 - Start Here/
│   ├── How to Install.md
│   ├── CSS Snippets.md
│   └── Custom Colors.md
│
├── 01 - Color UI/
│   ├── Color Swatch Cards.md
│   └── Color Reference Table.md
│
├── 02 - Chat UI/
│   └── Basic Chat Bubbles.md
│
└── .obsidian/
    └── snippets/
        ├── custom-colors.css
        ├── color-swatch-cards.css
        ├── reference-table.css
        └── chat-core.css
```

---

## 🛠️ Design Principles

Components in Obsidian UI Lab aim to be:

- **Easy to copy**
- **Easy to understand**
- **Easy to customize**
- **Independent where possible**
- **Consistent where useful**
- **Plugin-free unless explicitly stated**

Take one component, take several, or use the entire vault.

---

## 🗺️ Coming Next

### Chat UI

- Reply messages
- Image messages
- Image galleries
- Message reactions
- Complete chat examples

### More UI

- Cards
- Image layouts
- Journaling layouts
- Trackers
- Dashboards
- Navigation components
- Creative writing UI
- Interface-inspired components

---

## 💜 About

Obsidian UI Lab is an evolving personal collection of UI experiments turned into reusable components.

More components coming soon.

---

## 📄 License

This project is available under the [MIT License](LICENSE).

Feel free to use, modify, and adapt the components for your own projects.