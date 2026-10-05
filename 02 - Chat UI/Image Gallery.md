# Image Gallery

> [!info]
> 🔵 **Requires CSS**  
> Requires [[Basic Chat Bubbles]]  
> No third-party plugins required.

Display multiple image embeds as a compact two-column chat gallery.

---

## Preview

> [!chat-left-gallery]
> ![[example-image.png]]
>
> ![[example-image-0.png]]
>
> ![[example-image-1.png]]
>
> ![[example-image-2.png]]
>
> <span class="chat-time">20:41</span>

> [!chat-right-gallery]
> ![[example-image.png]]
>
> ![[example-image-0.png]]
>
> ![[example-image-1.png]]
>
> ![[example-image-2.png]]
>
> <span class="chat-time">20:42 ✓✓</span>

---

## Usage

### Left Gallery

```md
> [!chat-left-gallery]
> ![[example-image.png]]
>
> ![[example-image-0.png]]
>
> ![[example-image-1.png]]
>
> ![[example-image-2.png]]
>
> <span class="chat-time">20:41</span>
```

### Right Gallery

```md
> [!chat-right-gallery]
> ![[example-image.png]]
>
> ![[example-image-0.png]]
>
> ![[example-image-1.png]]
>
> ![[example-image-2.png]]
>
> <span class="chat-time">20:42 ✓✓</span>
```

---

## Layout

The default gallery uses two columns:

```css
grid-template-columns: repeat(2, minmax(0, 1fr));
```

Four images produce:

```text
┌─────────────┬─────────────┐
│             │             │
│   Image 1   │   Image 2   │
│             │             │
├─────────────┼─────────────┤
│             │             │
│   Image 3   │   Image 4   │
│             │             │
├───────────────────────────┤
│                     20:41 │
└───────────────────────────┘
```

---

## Using Fewer Images

Two images work naturally:

```md
> [!chat-left-gallery]
> ![[example-image-1.jpg]]
>
> ![[example-image-2.jpg]]
>
> <span class="chat-time">20:41</span>
```

Three images also work:

```text
┌─────────────┬─────────────┐
│   Image 1   │   Image 2   │
├─────────────┼─────────────┤
│   Image 3   │             │
├───────────────────────────┤
│                     20:41 │
└───────────────────────────┘
```

---

## Features

- Native Obsidian image embeds
- Two-column gallery
- Left and right gallery messages
- Responsive gallery width
- Consistent image cropping
- Timestamps
- Read receipts
- Rounded image corners
- Scrollbar cleanup
- No third-party plugins required

---

## Requirements

This component requires:

```text
chat-core.css
chat-gallery.css
```

Copy both files into:

```text
YOUR-VAULT/
└── .obsidian/
    └── snippets/
```

Then enable:

- `chat-core`
- `chat-gallery`

under:

**Settings → Appearance → CSS snippets**

`custom-colors.css` is optional.

---

## Image Size

Gallery images currently use:

```css
height: 150px;
object-fit: cover;
```

This means images with different dimensions still produce a clean grid.

To make the gallery taller:

```css
height: 200px;
```

For smaller thumbnails:

```css
height: 110px;
```

---

## Gallery Width

The default gallery width is:

```css
width: 360px;
max-width: 70%;
```

You can adjust this to suit your vault layout.

For example:

```css
width: 440px;
max-width: 80%;
```

---

## Related

- [[Basic Chat Bubbles]]
- [[Image Messages]]
- [[Reply Messages]]

