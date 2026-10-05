# Message Reactions

> [!info]
> 🔵 **Requires CSS**  
> Requires [[Basic Chat Bubbles]]  
> No third-party plugins required.

Add emoji reactions beneath chat messages.

Reactions sit partially outside the message bubble, similar to reactions in modern messaging apps.

---

## Preview

> [!chat-left]
> I finally finished it!
>
> <span class="chat-time">20:41</span>
>
> <span class="chat-reactions"><span class="chat-reaction">❤️</span></span>


> [!chat-right]
> That looks amazing 👀
>
> <span class="chat-time">20:42 ✓✓</span>
>
> <span class="chat-reactions"><span class="chat-reaction">🔥</span><span class="chat-reaction">👏</span></span>



> [!chat-left]
> The new version is live.
>
> <span class="chat-time">21:03</span>
>
> <span class="chat-reactions"><span class="chat-reaction reaction-count">❤️ <small>4</small></span></span>

> [!chat-right]
> Shipping it today 🚀
>
> <span class="chat-time">21:04 ✓✓</span>
>
> <span class="chat-reactions"><span class="chat-reaction reaction-count">🔥 <small>3</small></span><span class="chat-reaction reaction-count">🚀 <small>2</small></span></span>

---

## Usage

### Single Reaction

```md
> [!chat-left]
> I finally finished it!
>
> <span class="chat-time">20:41</span>
>
> <span class="chat-reactions">
> 	<span class="chat-reaction">❤️</span>
> </span>
```

---

## Multiple Reactions

Add multiple `chat-reaction` elements inside the reaction row:

```md
> [!chat-right]
> That looks amazing 👀
>
> <span class="chat-time">20:42 ✓✓</span>
>
> <span class="chat-reactions">
> 	<span class="chat-reaction">🔥</span>
> 	<span class="chat-reaction">👏</span></span>
```

---

## Reaction Counts

Use `reaction-count` when you want to show how many people reacted:

```md
> [!chat-left]
> The new version is live.
>
> <span class="chat-time">21:03</span>
>
> <span class="chat-reactions">
> 	<span class="chat-reaction reaction-count">❤️ <small>4</small></span>
> </span>
```

You can combine counted and uncounted reactions:

```md
> [!chat-right]
> Shipping it today 🚀
>
> <span class="chat-time">21:04 ✓✓</span>
>
> <span class="chat-reactions">
> 	<span class="chat-reaction reaction-count">🔥 <small>3</small></span>
> 	<span class="chat-reaction reaction-count">🚀 <small>2</small></span>
> </span>
```

---

## Alignment

Reactions automatically follow the message side.

### Left message

```text
┌───────────────────────────┐
│ I finally finished it!    │
│                     20:41 │
└───────────────────────────┘
   ❤️
```

### Right message

```text
             ┌───────────────────────────┐
             │ That looks amazing!       │
             │                 20:42 ✓✓  │
             └───────────────────────────┘
                                      🔥 👏
```

No separate alignment class is required.

---

## Image Messages

Reactions also work with [[Image Messages]]:

```md
> [!chat-right]
> ![[example-image.png]]
>
> <span class="chat-time">20:42 ✓✓</span>
>
> <span class="chat-reactions">
>   <span class="chat-reaction">❤️</span>
> </span>
```

Enable:

- `chat-core.css`
- `chat-images.css`
- `chat-reactions.css`

---

## Image Galleries

Reactions can also be added beneath [[Image Gallery]] messages:

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
>
> <span class="chat-reactions">
>   <span class="chat-reaction reaction-count">
>     ❤️ <small>2</small>
>   </span>
> </span>
```

---

## Features

- Single emoji reactions
- Multiple reactions
- Optional reaction counts
- Automatic left/right alignment
- Works with normal messages
- Works with reply messages
- Works with image messages
- Works with image galleries
- No third-party plugins required

---

## Requirements

The basic component requires:

```text
chat-core.css
chat-reactions.css
```

Copy them into:

```text
YOUR-VAULT/
└── .obsidian/
    └── snippets/
```

Then enable:

- `chat-core`
- `chat-reactions`

under:

**Settings → Appearance → CSS snippets**

Additional message types require their respective snippets.

---

## CSS Classes

| Class | Purpose |
| --- | --- |
| `chat-reactions` | Container holding all reactions |
| `chat-reaction` | Individual emoji reaction |
| `reaction-count` | Makes a reaction wide enough to display a count |

---

## Customization

### Reaction Size

The default size is:

```css
width: 27px;
height: 27px;
```

For slightly larger reactions:

```css
width: 32px;
height: 32px;
```

---

### Distance From Bubble

Reactions currently sit:

```css
bottom: -15px;
```

For more overlap:

```css
bottom: -12px;
```

For more separation:

```css
bottom: -18px;
```

---

## Related

- [[Basic Chat Bubbles]]
- [[Reply Messages]]
- [[Image Messages]]
- [[Image Gallery]]
