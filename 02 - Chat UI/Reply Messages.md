# Reply Messages

> [!info]
> 🔵 **Requires CSS**  
> Requires [[Basic Chat Bubbles]]  
> No third-party plugins required.

Add quoted replies inside chat bubbles.

Reply messages show a compact preview of the original message followed by the new response.

---

## Preview

> [!chat-left]
> > [!chat-reply] Alex
> > Are you coming tonight?
>
> Yeah, I'll be there.
>
> <span class="chat-time">20:42</span>

> [!chat-right]
> > [!chat-reply] Sam
> > Yeah, I'll be there.
>
> Perfect. See you later 👋
>
> <span class="chat-time">20:43 ✓✓</span>


---

## Usage

### Left-side reply

```md
> [!chat-left]
> > [!chat-reply] Alex
> > Are you coming tonight?
>
> Yeah, I'll be there.
>
> <span class="chat-time">20:42</span>
```

### Right-side reply

```md
> [!chat-right]
> > [!chat-reply] Sam
> > Yeah, I'll be there.
>
> Perfect. See you later 👋
>
> <span class="chat-time">20:43 ✓✓</span>
```

---

## How It Works

A reply consists of three parts:

```text
chat-reply
├── chat-reply-name
└── chat-reply-text

chat-message
```

### `chat-reply`

Creates the quoted message container.

### `chat-reply-name`

Displays the name of the person being replied to.

### `chat-reply-text`

Displays a short preview of the original message.

Long quoted messages are automatically shortened with an ellipsis.

### `chat-message`

Contains the new response below the quoted message.

---

## Features

- Quoted message preview
- Reply author/name
- Automatic text truncation
- Different styling for left and right messages
- Works with timestamps and read receipts
- Builds directly on Basic Chat Bubbles
- No third-party plugins required

---

## Requirements

This component requires:

```text
chat-core.css
chat-replies.css
```

Copy both files into:

```text
YOUR-VAULT/
└── .obsidian/
    └── snippets/
```

Then enable both under:

**Settings → Appearance → CSS snippets**

Enable:

- `chat-core`
- `chat-replies`

---

## CSS Classes

| Class | Purpose |
| --- | --- |
| `chat-reply` | Reply preview container |
| `chat-reply-name` | Name of the person being replied to |
| `chat-reply-text` | Original quoted message |
| `chat-message` | New reply text |

---

## Text Truncation

Quoted messages use:

```css
white-space: nowrap;
overflow: hidden;
text-overflow: ellipsis;
```

This keeps long replies compact.

For example:

```text
I was thinking that maybe we could meet a little earlier because...
```

instead of allowing the quoted message to dominate the bubble.

---

## Related

- [[Basic Chat Bubbles]]
