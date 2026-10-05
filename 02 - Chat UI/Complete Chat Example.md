# Complete Chat Example

> [!info]
> 🔵 **Requires CSS**  
> No third-party plugins required.

A complete example combining the modular Chat UI components from Obsidian UI Lab.

This page demonstrates:

- Basic chat bubbles
- Date separators
- Timestamps
- Read receipts
- Reply messages
- Image messages
- Image galleries
- Message reactions

---

## Requirements

Enable:

```text
chat-core.css
chat-replies.css
chat-images.css
chat-gallery.css
chat-reactions.css
```

Optional:

```text
custom-colors.css
```

---

## Complete Example

<div class="chat-date">Today</div>

> [!chat-left]
> Hey! Did you see the photos from yesterday?
>
> <span class="chat-time">18:41</span>

> [!chat-right]
> Not yet 👀
>
> Send them!
>
> <span class="chat-time">18:42 ✓✓</span>

> [!chat-left]
> ![[example-image-1.png]]
>
> <span class="chat-time">18:43</span>
>
> <span class="chat-reactions"><span class="chat-reaction">❤️</span></span>

> [!chat-right]
> > [!chat-reply] Alex
> > Send them!
>
> I have a few more 😄
>
> <span class="chat-time">18:44 ✓✓</span>

> [!chat-right-gallery]
> ![[example-image.png]]
>
> ![[example-image-0.png]]
>
> ![[example-image-1.png]]
>
> ![[example-image-2.png]]
>
> <span class="chat-time">18:45 ✓✓</span>
>
> <span class="chat-reactions"><span class="chat-reaction reaction-count">🔥 <small>3</small></span><span class="chat-reaction">😍</span></span>

> [!chat-left]
> > [!chat-reply] Alex
> > I have a few more 😄
>
> These turned out so good.
>
> <span class="chat-time">18:46</span>

> [!chat-right]
> Definitely keeping them.
>
> <span class="chat-time">18:47 ✓✓</span>
>
> <span class="chat-reactions"><span class="chat-reaction">💜</span><span class="chat-reaction">✨</span></span>

---

## How the Components Work Together

### Core

Every text message starts with either:

```md
> [!chat-left]
```

or:

```md
> [!chat-right]
```

Provided by:

```text
chat-core.css
```

---

### Replies

Replies use a nested callout:

```md
> [!chat-right]
> > [!chat-reply] Alex
> > Original message
>
> New response
>
> <span class="chat-time">18:44 ✓✓</span>
```

Provided by:

```text
chat-replies.css
```

---

### Images

Native Obsidian image embeds can be placed directly inside a message:

```md
> [!chat-left]
> ![[example-image.png]]
>
> <span class="chat-time">18:43</span>
```

Provided by:

```text
chat-images.css
```

---

### Galleries

Use a gallery-specific callout:

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
> <span class="chat-time">18:45 ✓✓</span>
```

Provided by:

```text
chat-gallery.css
```

---

### Reactions

Reaction HTML should stay on a single line inside Obsidian callouts:

```md
> <span class="chat-reactions"><span class="chat-reaction">❤️</span></span>
```

Multiple reactions:

```md
> <span class="chat-reactions"><span class="chat-reaction">🔥</span><span class="chat-reaction">👏</span></span>
```

Reaction counts:

```md
> <span class="chat-reactions"><span class="chat-reaction reaction-count">❤️ <small>4</small></span></span>
```

Provided by:

```text
chat-reactions.css
```

---

## Component Stack

```text
Basic Chat Bubbles
│
├── Reply Messages
│
├── Image Messages
│
├── Image Gallery
│
└── Message Reactions
│
└── Complete Chat Example
```

The extensions remain separate so you only need to enable the functionality you actually use.

---

## Example Assets

The example conversation uses:

```text
assets/
└── examples/
    ├── example-image.png
    ├── example-image-0.png
    ├── example-image-1.png
    └── example-image-2.png
```

Replace them with any images from your own vault.

---

## Related

- [[Basic Chat Bubbles]]
- [[Reply Messages]]
- [[Image Messages]]
- [[Image Gallery]]
- [[Message Reactions]]
