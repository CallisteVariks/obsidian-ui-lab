# Color Swatch Cards

> [!info]  
> 🔵 **Requires CSS**  
> No third-party plugins required.

A responsive card grid for displaying color swatches and their values.

This component uses the shared color variables from `custom-colors.css` to keep the design consistent across Obsidian UI Lab.

---

## Preview

<div class="swatch-grid">

<div class="swatch-card"> <div class="swatch-color" style="background: var(--ui-red);"></div> <div class="swatch-content"> <div class="swatch-title">Crimson</div> <div class="swatch-row"><span class="swatch-label">HEX</span><span>#E63946</span></div> <div class="swatch-row"><span class="swatch-label">RGB</span><span>230, 57, 70</span></div> <div class="swatch-row"><span class="swatch-label">HSL</span><span>355, 78%, 56%</span></div> <div class="swatch-row"><span class="swatch-label">CMYK</span><span>0, 75, 70, 10</span></div> </div> </div>

<div class="swatch-card"> <div class="swatch-color" style="background: var(--ui-orange);"></div> <div class="swatch-content"> <div class="swatch-title">Apricot</div> <div class="swatch-row"><span class="swatch-label">HEX</span><span>#F4A261</span></div> <div class="swatch-row"><span class="swatch-label">RGB</span><span>244, 162, 97</span></div> <div class="swatch-row"><span class="swatch-label">HSL</span><span>27, 87%, 67%</span></div> <div class="swatch-row"><span class="swatch-label">CMYK</span><span>0, 34, 60, 4</span></div> </div> </div>

<div class="swatch-card"> <div class="swatch-color" style="background: var(--ui-yellow);"></div> <div class="swatch-content"> <div class="swatch-title">Sunflower</div> <div class="swatch-row"><span class="swatch-label">HEX</span><span>#E9C46A</span></div> <div class="swatch-row"><span class="swatch-label">RGB</span><span>233, 196, 106</span></div> <div class="swatch-row"><span class="swatch-label">HSL</span><span>43, 74%, 66%</span></div> <div class="swatch-row"><span class="swatch-label">CMYK</span><span>0, 16, 55, 9</span></div> </div> </div>

<div class="swatch-card"> <div class="swatch-color" style="background: var(--ui-green);"></div> <div class="swatch-content"> <div class="swatch-title">Sea Green</div> <div class="swatch-row"><span class="swatch-label">HEX</span><span>#2A9D8F</span></div> <div class="swatch-row"><span class="swatch-label">RGB</span><span>42, 157, 143</span></div> <div class="swatch-row"><span class="swatch-label">HSL</span><span>173, 58%, 39%</span></div> <div class="swatch-row"><span class="swatch-label">CMYK</span><span>73, 0, 9, 38</span></div> </div> </div>

<div class="swatch-card"> <div class="swatch-color" style="background: var(--ui-blue);"></div> <div class="swatch-content"> <div class="swatch-title">Ocean Blue</div> <div class="swatch-row"><span class="swatch-label">HEX</span><span>#457B9D</span></div> <div class="swatch-row"><span class="swatch-label">RGB</span><span>69, 123, 157</span></div> <div class="swatch-row"><span class="swatch-label">HSL</span><span>203, 39%, 44%</span></div> <div class="swatch-row"><span class="swatch-label">CMYK</span><span>56, 22, 0, 38</span></div> </div> </div>

<div class="swatch-card"> <div class="swatch-color" style="background: var(--ui-purple);"></div> <div class="swatch-content"> <div class="swatch-title">Muted Plum</div> <div class="swatch-row"><span class="swatch-label">HEX</span><span>#6D597A</span></div> <div class="swatch-row"><span class="swatch-label">RGB</span><span>109, 89, 122</span></div> <div class="swatch-row"><span class="swatch-label">HSL</span><span>276, 16%, 41%</span></div> <div class="swatch-row"><span class="swatch-label">CMYK</span><span>11, 27, 0, 52</span></div> </div> </div>

<div class="swatch-card"> <div class="swatch-color" style="background: var(--ui-charcoal);"></div> <div class="swatch-content"> <div class="swatch-title">Charcoal</div> <div class="swatch-row"><span class="swatch-label">HEX</span><span>#222222</span></div> <div class="swatch-row"><span class="swatch-label">RGB</span><span>34, 34, 34</span></div> <div class="swatch-row"><span class="swatch-label">HSL</span><span>0, 0%, 13%</span></div> <div class="swatch-row"><span class="swatch-label">CMYK</span><span>0, 0, 0, 87</span></div> </div> </div>

<div class="swatch-card"> <div class="swatch-color swatch-light" style="background: var(--ui-white);"></div> <div class="swatch-content"> <div class="swatch-title">White</div> <div class="swatch-row"><span class="swatch-label">HEX</span><span>#FFFFFF</span></div> <div class="swatch-row"><span class="swatch-label">RGB</span><span>255, 255, 255</span></div> <div class="swatch-row"><span class="swatch-label">HSL</span><span>0, 0%, 100%</span></div> <div class="swatch-row"><span class="swatch-label">CMYK</span><span>0, 0, 0, 0</span></div> </div> </div>

</div>

---

## Usage

Create a grid using the `swatch-grid` class, then add one or more `swatch-card` elements.

```
<div class="swatch-grid">

  <div class="swatch-card">
    <div class="swatch-color" style="background: var(--ui-red);"></div>

    <div class="swatch-content">
      <div class="swatch-title">Crimson</div>

      <div class="swatch-row">
        <span class="swatch-label">HEX</span>
        <span>#E63946</span>
      </div>

      <div class="swatch-row">
        <span class="swatch-label">RGB</span>
        <span>230, 57, 70</span>
      </div>

      <div class="swatch-row">
        <span class="swatch-label">HSL</span>
        <span>355, 78%, 56%</span>
      </div>

      <div class="swatch-row">
        <span class="swatch-label">CMYK</span>
        <span>0, 75, 70, 10</span>
      </div>
    </div>
  </div>

</div>
```

### Using your own color

You don't have to use the shared Obsidian UI Lab palette.

Any valid CSS color can be used:

```
<div class="swatch-color" style="background:#A78BFA;"></div>
```

You can also define your own CSS variable:

```
:root {
  --my-color: #A78BFA;
}
```

and reference it from the card:

```
<div class="swatch-color" style="background:var(--my-color);"></div>
```

---

## Features

- Responsive card grid
- Automatically adapts to the available width
- Reusable color swatches
- Supports CSS variables and custom colors
- Works with plain HTML inside Obsidian notes
- Uses Obsidian theme variables for card styling
- Light and dark theme friendly
- No third-party plugins required

---

## Requirements

This component uses two CSS snippets:

- `custom-colors.css` — shared Obsidian UI Lab color variables
- `color-swatch-cards.css` — layout and card styling

Copy both files into:

`.obsidian/snippets/`

Then open:

**Settings → Appearance → CSS snippets**

Reload the snippets and enable:

- **custom-colors**
- **color-swatch-cards**

---

## CSS Classes

|Class|Purpose|
|---|---|
|`swatch-grid`|Responsive container for the cards|
|`swatch-card`|Individual color card|
|`swatch-color`|Color preview area|
|`swatch-light`|Adds separation for very light swatches|
|`swatch-content`|Content area below the color|
|`swatch-title`|Color name|
|`swatch-row`|Property/value row|
|`swatch-label`|Property label|

---

## Customization

The minimum card width is controlled in `color-swatch-cards.css`:

```
grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
```

For smaller cards:

```
grid-template-columns: repeat(auto-fill, minmax(180px, 1fr));
```

For larger cards:

```
grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
```

The swatch height can also be changed:

```
.swatch-color {
  height: 100px;
}
```

---
