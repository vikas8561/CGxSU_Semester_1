# CSS Margin and Padding

CSS `margin` and `padding` are fundamental properties for controlling spacing around and within elements. This guide provides a detailed explanation of their usage.

## Margin
The `margin` property defines the space *outside* an element's border, creating distance between the element and adjacent elements.

- **Purpose**: Controls external spacing.
- **Values**: Accepts `px`, `%`, `cm`, `auto`, or negative values.
- **Key Notes**:
  - Margins can collapse vertically (e.g., between stacked elements like paragraphs).
  - `margin: auto` is often used to center block elements horizontally.
  - Negative margins can pull elements closer or overlap them.

### Margin: Shorthand
The shorthand `margin` property allows setting all four sides (top, right, bottom, left) in one line.

- **Syntax**: `margin: top right bottom left;`
- **Rules**:
  - **One value**: Applies to all four sides (e.g., `margin: 10px;`).
  - **Two values**: First sets top/bottom, second sets left/right (e.g., `margin: 10px 20px;`).
  - **Three values**: First sets top, second sets left/right, third sets bottom (e.g., `margin: 10px 20px 30px;`).
  - **Four values**: Sets top, right, bottom, left in that order (e.g., `margin: 10px 20px 30px 40px;`).

### Margin: Without Shorthand
Individual properties can be used to set margins for specific sides.

- **Properties**:
  - `margin-top`
  - `margin-right`
  - `margin-bottom`
  - `margin-left`

## Padding
The `padding` property defines the space *inside* an element, between its content and border.

- **Purpose**: Controls internal spacing.
- **Values**: Accepts `px`, `%`, `cm`, or other length units (cannot be negative).
- **Key Notes**:
  - Padding increases an element’s total size unless `box-sizing: border-box` is applied.
  - Affects the space where background colors/images are visible.

### Padding: Shorthand
The shorthand `padding` property sets padding for all four sides in one line.

- **Syntax**: `padding: top right bottom left;`
- **Rules**:
  - **One value**: Applies to all sides (e.g., `padding: 15px;`).
  - **Two values**: First sets top/bottom, second sets left/right (e.g., `padding: 15px 25px;`).
  - **Three values**: First sets top, second sets left/right, third sets bottom (e.g., `padding: 15px 25px 35px;`).
  - **Four values**: Sets top, right, bottom, left in that order (e.g., `padding: 15px 25px 35px 45px;`).

### Padding: Without Shorthand
Individual properties can be used to set padding for specific sides.

- **Properties**:
  - `padding-top`
  - `padding-right`
  - `padding-bottom`
  - `padding-left`

## Examples

### Example 1: Shorthand Margin and Padding
Using shorthand for both margin and padding.

```html
<div style="margin: 20px; padding: 15px; border: 1px solid black;">
  This div has 20px margin and 15px padding on all sides.
</div>
```

### Example 2: Shorthand Margin with Two Values
Applying margin with two values and padding with one value.

```html
<div style="margin: 10px 50px; padding: 20px; border: 1px solid blue;">
  This div has 10px top/bottom margin, 50px left/right margin, and 20px padding.
</div>
```

### Example 3: Non-Shorthand Padding
Setting padding for each side individually.

```html
<div style="padding-top: 10px; padding-right: 20px; padding-bottom: 30px; padding-left: 40px; border: 1px solid green;">
  This div has different padding on each side using individual properties.
</div>
```

### Example 4: Non-Shorthand Margin for Centering
Using `margin-left` and `margin-right` to center a div (alternative to `margin: auto`).

```html
<div style="width: 200px; margin-left: auto; margin-right: auto; padding: 10px; border: 1px solid red;">
  This div is centered using non-shorthand margin properties.
</div>
```

### Example 5: Mixed Shorthand and Non-Shorthand
Combining shorthand for margin and non-shorthand for padding.

```html
<div style="margin: 15px 25px 15px 25px; padding-top: 20px; padding-bottom: 20px; border: 1px solid purple;">
  This div has shorthand margin (15px top/bottom, 25px left/right) and non-shorthand padding (20px top/bottom).
</div>
```


