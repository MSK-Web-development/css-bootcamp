# Media queries

Media queries in CSS allow you to apply styles based on the characteristics of the device or viewport, such as screen size, device orientation, or screen resolution. Here's an explanation of various types of media queries with specific examples:

### 1. **Screen Width (`min-width`, `max-width`)**:

- Adjust styles based on the width of the viewport.

```css
/* Applies styles when the viewport width is at least 768px */
@media screen and (min-width: 768px) {
    /* CSS styles */
}

/* Applies styles when the viewport width is at most 1200px */
@media screen and (max-width: 1200px) {
    /* CSS styles */
}
```

### 2. **Screen Height (`min-height`, `max-height`)**:

- Adjust styles based on the height of the viewport.

```css
/* Applies styles when the viewport height is at least 600px */
@media screen and (min-height: 600px) {
    /* CSS styles */
}

/* Applies styles when the viewport height is at most 800px */
@media screen and (max-height: 800px) {
    /* CSS styles */
}
```

### 3. **Device Orientation (`orientation`)**:

- Adjust styles based on the orientation of the device (landscape or portrait).

```css
/* Applies styles when the device is in landscape orientation */
@media screen and (orientation: landscape) {
    /* CSS styles */
}

/* Applies styles when the device is in portrait orientation */
@media screen and (orientation: portrait) {
    /* CSS styles */
}
```

### 4. **Device Pixel Ratio (`min-resolution`, `max-resolution`)**:

- Adjust styles based on the device pixel ratio.

```css
/* Applies styles when the device pixel ratio is at least 2 */
@media screen and (min-resolution: 2dppx) {
    /* CSS styles */
}

/* Applies styles when the device pixel ratio is at most 1.5 */
@media screen and (max-resolution: 1.5dppx) {
    /* CSS styles */
}
```

### 5. **Aspect Ratio (`aspect-ratio`)**:

- Adjust styles based on the aspect ratio of the viewport.

```css
/* Applies styles when the aspect ratio of the viewport is 16:9 */
@media screen and (aspect-ratio: 16/9) {
    /* CSS styles */
}
```

### 6. **Resolution (`resolution`)**:

- Adjust styles based on the resolution of the output device.

```css
/* Applies styles when the resolution is at least 300dpi */
@media screen and (min-resolution: 300dpi) {
    /* CSS styles */
}
```

### 7. **Hover (`hover`)**:

- Adjust styles based on the ability of the device to hover over elements.

```css
/* Applies styles when the device supports hover */
@media (hover: hover) {
    /* CSS styles */
}
```

### 8. **Pointer (`pointer`)**:

- Adjust styles based on the type of pointing device available.

```css
/* Applies styles when the primary input mechanism includes a pointing device */
@media (pointer: fine) {
    /* CSS styles */
}
```

These examples cover various media queries you can use to create responsive designs that adapt to different devices and user environments. Using media queries, you can optimize the presentation of your website or web application across a wide range of devices and screen sizes.