# How to Install

Obsidian UI Lab is a collection of reusable Markdown layouts and CSS components for [Obsidian](https://obsidian.md/).

You can either:

1. **Download the entire vault** to explore all components and examples, or    
2. **Install individual components** into an existing Obsidian vault.

No third-party Obsidian plugins are required unless a component specifically says otherwise.

---

## Option 1 — Download the Full Vault

### Download from GitHub

Open the repository:

`https://github.com/CallisteVariks/obsidian-ui-lab`

Select:

**Code → Download ZIP**

Extract the downloaded archive somewhere on your computer.

Then open Obsidian and select:

**Open folder as vault**

Choose the extracted `obsidian-ui-lab` folder.

---

### Clone with Git

If you use Git, you can clone the repository instead:

```
git clone https://github.com/CallisteVariks/obsidian-ui-lab.git
```

Then open the cloned folder in Obsidian using:

**Open folder as vault**

---

## Option 2 — Install Individual Components

You do not need to download the entire vault.

Each component normally consists of:

- A Markdown example or documentation file
- One component-specific CSS snippet
- Sometimes a shared CSS dependency such as `custom-colors.css`

For example, **Color Swatch Cards** uses:

```
01 - Color UI/
└── Color Swatch Cards.md
```

and:

```
.obsidian/
└── snippets/
    ├── custom-colors.css
    └── color-swatch-cards.css
```

You can copy only the files you need into your own vault.

---

## Installing CSS Snippets

Obsidian loads custom CSS snippets from:

```
YOUR-VAULT/
└── .obsidian/
    └── snippets/
```

If the `snippets` folder does not exist, create it manually.

For example:

```
My Vault/
│
├── Notes/
│
└── .obsidian/
    └── snippets/
        ├── custom-colors.css
        └── color-swatch-cards.css
```

> [!tip]  
> The `.obsidian` folder may be hidden by your operating system.  
> Enable **Show hidden files** if you cannot see it.

---

## Enable a CSS Snippet

After copying a `.css` file into `.obsidian/snippets/`:

1. Open **Obsidian**
2. Go to **Settings**
3. Select **Appearance**
4. Scroll to **CSS snippets**
5. Select **Reload snippets**
6. Enable the snippet you want to use

For example:

- `custom-colors`
- `color-swatch-cards`

The component should update immediately.

---

## Shared CSS

Some components use shared styles from Obsidian UI Lab.

The main shared stylesheet is:

```
custom-colors.css
```

It contains reusable color variables such as:

```
--ui-red
--ui-orange
--ui-yellow
--ui-green
--ui-blue
--ui-purple
--ui-pink
```

as well as softer variants used across different components.

For example:

```
color: var(--ui-purple);
```

or:

```
background: var(--ui-soft-purple);
```

This helps components maintain a consistent visual style.

> [!note]  
> Components are not necessarily locked to these colors.  
> You can replace the provided variables with your own CSS colors or custom variables.

---

## Component Requirements

Each component page includes a requirements section near the top.

For example:

> [!info]  
> 🔵 **Requires CSS**  
> No third-party plugins required.

Some components may require more than one stylesheet.

Always check the **Requirements** section of the component before using it.

---

## Using the Markdown Examples

Most components contain a ready-to-copy example.

For example:

```
<div class="swatch-card">
  <div class="swatch-color" style="background: var(--ui-red);"></div>

  <div class="swatch-content">
    <div class="swatch-title">Crimson</div>
  </div>
</div>
```

Copy the example into one of your Obsidian notes and customize the content as needed.

The corresponding CSS snippet controls the visual appearance.

---

## Updating the Full Vault

If you cloned the repository with Git, you can retrieve new components and updates with:

```
git pull
```

If you downloaded the repository as a ZIP, download a newer version whenever you want to update it.

---

## Customizing Components

You are encouraged to change:

- Colors
- Spacing
- Fonts
- Border radius
- Card sizes
- Layout widths
- Labels
- Content

For example, a component using:

```
background: var(--ui-purple);
```

can instead use:

```
background: #A78BFA;
```

or your own variable:

```
background: var(--my-accent);
```

The examples in this vault are intended as starting points rather than fixed themes.

---

## Troubleshooting

### My CSS snippet does not appear

Check that the file is located directly inside:

```
.obsidian/snippets/
```

Then go to:

**Settings → Appearance → CSS snippets → Reload snippets**

---

### The component has no styling

Make sure all CSS files listed under the component's **Requirements** section are enabled.

For example, Color Swatch Cards currently uses:

```
custom-colors.css
color-swatch-cards.css
```

Both should be enabled.

---

### I changed the CSS but nothing happened

Try:

**Settings → Appearance → CSS snippets → Reload snippets**

You can also toggle the affected snippet off and back on.

---

### The `.obsidian` folder is missing

The folder exists inside every Obsidian vault but may be hidden by your operating system.

Enable hidden files in your file explorer to display it.

---

## Current Structure

The project will grow over time, but the initial vault is intentionally small:

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

New UI components and categories will be added gradually.

---
