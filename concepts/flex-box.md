# Flexbox

### 1. **Introduction to Flexbox**:

Flexbox is a layout model in CSS designed to make the alignment and distribution of elements within a container more efficient and flexible. It provides a set of properties for controlling the size, alignment, and spacing of items within a container.

### 2. **Flex Container Properties**:

#### a. `display`

- Defines the container as a flex container.

```css
.container {
  display: flex;
}
```

#### b. `flex-direction`

- Defines the main axis along which flex items are laid out within the container.

```css
.container {
  flex-direction: row; /* default */
  /* Other values: column, row-reverse, column-reverse */
}
```

#### c. `flex-wrap`

- Controls whether flex items are forced onto a single line or can wrap onto multiple lines.

```css
.container {
  flex-wrap: nowrap; /* default */
  /* Other values: wrap, wrap-reverse */
}
```

#### d. `justify-content`

- Aligns flex items along the main axis of the container.

```css
.container {
  justify-content: flex-start; /* default */
  /* Other values: flex-end, center, space-between, space-around */
}
```

#### e. `align-items`

- Aligns flex items along the cross axis of the container.

```css
.container {
  align-items: stretch; /* default */
  /* Other values: flex-start, flex-end, center, baseline */
}
```

#### f. `align-content`

- Aligns flex lines within the container when there is extra space in the cross axis.

```css
.container {
  align-content: stretch; /* default */
  /* Other values: flex-start, flex-end, center, space-between, space-around */
}
```

### 3. **Flex Item Properties**:

#### a. `order`

- Controls the order in which flex items appear within the container.

```css
.item {
  order: 2;
}
```

#### b. `flex-grow`

- Specifies how flex items grow relative to other flex items in the container.

```css
.item {
  flex-grow: 1; /* default */
}
```

#### c. `flex-shrink`

- Specifies how flex items shrink relative to other flex items in the container.

```css
.item {
  flex-shrink: 1; /* default */
}
```

#### d. `flex-basis`

- Specifies the initial main size of a flex item before any remaining space is distributed.

```css
.item {
  flex-basis: auto; /* default */
}
```

#### e. `flex`

- Shorthand for `flex-grow`, `flex-shrink`, and `flex-basis`.

```css
.item {
  flex: 1 1 auto; /* default */
}
```

#### f. `align-self`

- Overrides the `align-items` value for a single flex item.

```css
.item {
  align-self: flex-start; /* default */
  /* Other values: flex-end, center, baseline, stretch */
}
```

### 4. **Example**:

```html
<div class="container">
  <div class="item">Item 1</div>
  <div class="item">Item 2</div>
  <div class="item">Item 3</div>
</div>
```

```css
.container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}

.item {
  flex: 1;
  background-color: lightblue;
  margin: 5px;
  padding: 10px;
  border: 1px solid black;
}
```

This example creates a flex container with three flex items evenly spaced along the main axis. The flex items have equal width and are vertically centered within the container.

### Summary:

CSS Flexbox provides a powerful and flexible way to create layouts in CSS. By using flex container and flex item properties, you can easily create responsive and adaptive designs that adjust to different screen sizes and devices. Mastering Flexbox is essential for modern web development, as it simplifies the process of building complex layouts and improves the overall user experience.
