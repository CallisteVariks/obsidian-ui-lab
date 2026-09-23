# Basic Chat Bubbles

> [!info]  
> 🔵 **Requires CSS**  
> No third-party plugins required.

Create simple left- and right-aligned chat messages using native Obsidian callouts.

The component includes:

- Left and right message bubbles
- Message tails
- Timestamps
- Read receipts
- Optional date separators
- Obsidian scrollbar fixes

---

## Preview

<div class="chat-date">Today</div>

> [!chat-left]  
> Hey! Are you coming tonight?
> 
> <span class="chat-time">20:41</span>

> [!chat-right]  
> Yeah, I'll be there.
> 
> <span class="chat-time">20:42 ✓✓</span>

> [!chat-left]  
> Perfect. See you later 👋
> 
> <span class="chat-time">20:43</span>

---

## Usage

### Left Message

```
> [!chat-left]
> Hey! Are you coming tonight?
>
> <span class="chat-time">20:41</span>
```

### Right Message

```
> [!chat-right]
> Yeah, I'll be there.
>
> <span class="chat-time">20:42 ✓✓</span>
```

---

## Date Separator

Use a simple HTML element to separate parts of a conversation:

```
<div class="chat-date">Today</div>
```

You can use any text:

```
<div class="chat-date">23 September 2026</div>
```

or:

```
<div class="chat-date">Yesterday</div>
```

---

## Timestamps

Add a timestamp using:

```
<span class="chat-time">20:42</span>
```

Read receipts can be added directly:

```
<span class="chat-time">20:42 ✓✓</span>
```

---

## Features

- Left-aligned messages
- Right-aligned messages
- Message bubble tails
- Timestamps
- Read receipts
- Date separators
- Responsive message width
- Obsidian overflow and scrollbar fixes
- Uses native Obsidian callouts
- No third-party plugins required

---

## Requirements

This component requires:

```
chat-core.css
```

Copy the file into:

```
YOUR-VAULT/
└── .obsidian/
    └── snippets/
        └── chat-core.css
```

Then open:

**Settings → Appearance → CSS snippets**

Select **Reload snippets** and enable:

**chat-core**

---

## Shared Colors

`custom-colors.css` is optional.

If enabled, the right-side message bubble uses the shared Obsidian UI Lab purple:

```
var(--ui-purple)
```

If the shared color snippet is not enabled, `chat-core.css` uses its own fallback color instead.

This means the chat component works independently while still supporting the shared Obsidian UI Lab theme.

---

## CSS Classes

|Class|Purpose|
|---|---|
|`chat-left`|Left-side message callout|
|`chat-right`|Right-side message callout|
|`chat-time`|Timestamp and optional read receipt|
|`chat-date`|Date separator|

---

## Customization

### Message Width

The maximum bubble width is controlled by:

```
max-width: 72%;
```

Increase it for wider messages:

```
max-width: 80%;
```

or reduce it for narrower bubbles:

```
max-width: 60%;
```

---

### Right-Side Bubble Color

The default right-side message uses:

```
background: var(--ui-purple, #6d597a);
```

The first value uses the shared Obsidian UI Lab palette.

The second value:

```
#6d597a
```

is the fallback color used when `custom-colors.css` is not enabled.

You can replace it with any color:

```
background: #457b9d;
```

---

### Bubble Radius

Change:

```
border-radius: 18px;
```

to make the bubbles more or less rounded.

For example:

```
border-radius: 12px;
```

---

## Compatibility

Designed for:

- Obsidian Reading View
- Obsidian Live Preview
- Light themes
- Dark themes

Theme-specific differences may slightly affect colors or spacing.

---

## Related Components

More chat components will build on this base.

Planned additions include:

- Reply messages
- Image messages
- Image galleries
- Message reactions
- Complete chat examples

These will use `chat-core.css` as their foundation.

---
