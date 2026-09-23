# CSS Snippets

This page lists the CSS snippets included in **Obsidian UI Lab**.

All snippets are stored in:

```
.obsidian/snippets/
```

You can enable or disable them individually in:

**Settings → Appearance → CSS snippets**

---

## Available Snippets

### `custom-colors.css`

Shared color variables and utility classes used across Obsidian UI Lab.

**Purpose**

- Provides the shared project color palette
- Keeps components visually consistent
- Includes text color utilities
- Includes highlight styles
- Can be reused by future cards, chats, dashboards, trackers, and other components

**Used by**

- [[Color Swatch Cards]]

**Example variables**

```
var(--ui-red)
var(--ui-orange)
var(--ui-yellow)
var(--ui-green)
var(--ui-blue)
var(--ui-purple)
var(--ui-pink)
```

Soft variants are also available:

```
var(--ui-soft-red)
var(--ui-soft-orange)
var(--ui-soft-yellow)
var(--ui-soft-green)
var(--ui-soft-blue)
var(--ui-soft-purple)
var(--ui-soft-pink)
```

**Example**

```
color: var(--ui-purple);
background: var(--ui-soft-purple);
```

> [!note]  
> This is a shared utility snippet rather than a standalone component.  
> Other snippets may depend on it.

---

### `color-swatch-cards.css`

Styles the responsive color card component used in [[Color Swatch Cards]].

**Purpose**

- Creates the responsive card grid
- Styles individual swatch cards
- Handles card spacing and layout
- Styles labels and values
- Adds support for light-colored swatches

**Used by**

- [[Color Swatch Cards]]

**Depends on**

- `custom-colors.css`

**Main classes**

```
.swatch-grid
.swatch-card
.swatch-color
.swatch-light
.swatch-content
.swatch-title
.swatch-row
.swatch-label
```

---

## Current Snippet Structure

```
.obsidian/
└── snippets/
    ├── custom-colors.css
    └── color-swatch-cards.css
```

More snippets will be added as new components are introduced.

---

## Installing a Snippet

Copy the required `.css` file into:

```
YOUR-VAULT/
└── .obsidian/
    └── snippets/
```

Then:

1. Open **Obsidian**
2. Go to **Settings**
3. Open **Appearance**
4. Scroll to **CSS snippets**
5. Select **Reload snippets**
6. Enable the snippet

If a component has dependencies, enable those snippets as well.

---

## Dependencies

Some components use shared snippets.

For example:

```
Color Swatch Cards
│
├── custom-colors.css
└── color-swatch-cards.css
```

The component documentation will always list its required CSS files.

---

## Customization

You are free to edit any snippet.

For example, changing a shared variable in `custom-colors.css`:

```
--ui-purple: #A78BFA;
```

will update every component that uses:

```
var(--ui-purple)
```

This makes it possible to create a consistent custom theme without editing every component separately.

---

## Naming Convention

Component-specific snippets use descriptive lowercase filenames separated with hyphens:

```
color-swatch-cards.css
chat-bubbles.css
image-gallery.css
profile-card.css
```

Shared utility files use broader names:

```
custom-colors.css
```

This keeps the snippets folder easy to browse as the project grows.

---

## Related

- [[How to Install]]
- [[Custom Colors]]
- [[Color Swatch Cards]]

---
