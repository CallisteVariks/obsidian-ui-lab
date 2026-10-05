# Image Messages

> [!info]
> 🔵 **Requires CSS**  
> Requires [[Basic Chat Bubbles]]  
> No third-party plugins required.

Display native Obsidian image embeds inside left- or right-aligned chat bubbles.

---

## Preview

> [!chat-left]
> ![[example-image.png]]
>
> <span class="chat-time">20:41</span>

> [!chat-right]
> ![[example-image.png]]
>
> <span class="chat-time">20:42 ✓✓</span>

---

## Usage

### Left Image

```md
> [!chat-left]
> ![[example-image.png]]
>
> <span class="chat-time">20:41</span>
```

### Right Image

```md
> [!chat-right]
> ![[example-image.png]]
>
> <span class="chat-time">20:42 ✓✓</span>
```

The image can be any image already stored in your Obsidian vault.

---

## Image With Message

You can also include text with the image:

```md
> [!chat-right]
> ![[example-image.png]]
>
> Look at this 👀
>
> <span class="chat-time">20:42 ✓✓</span>
```

---

## Features

- Native Obsidian image embeds
- Left and right image messages
- Rounded image corners
- Responsive image sizing
- Timestamps
- Read receipts
- Optional text captions
- Obsidian scrollbar cleanup
- No third-party plugins required

---

## Requirements

This component requires:

```text
chat-core.css
chat-images.css
```

Copy both files into:

```text
YOUR-VAULT/
└── .obsidian/
    └── snippets/
```

Then enable:

- `chat-core`
- `chat-images`

under:

**Settings → Appearance → CSS snippets**

---

## Image Size

Images currently use:

```css
max-width: 380px;
```

To make image messages wider:

```css
max-width: 480px;
```

Or remove the maximum completely:

```css
max-width: 100%;
```

---

## Bubble Width

Image bubbles use:

```css
max-width: 65%;
```

You can increase this for larger images:

```css
max-width: 75%;
```

---

## CSS Behavior

The image component does not redefine the chat bubble itself.

Instead:

```text
chat-core.css
      ↓
left/right bubble
      ↓
chat-images.css
      ↓
image-specific layout
```

This keeps chat components modular.

---

## Related

- [[Basic Chat Bubbles]]
- [[Reply Messages]]
