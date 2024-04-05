# Specificity

Specificity in CSS determines which styles are applied to elements when multiple conflicting styles are defined. It is calculated based on the combination of selectors used to target elements. Understanding specificity is crucial for resolving style conflicts and ensuring desired styling outcomes.

### Explanation:

In CSS, specificity is a measure of how specific a selector is in targeting elements in the HTML document. Specificity is calculated based on the combination of different types of selectors used in CSS rules. When multiple conflicting styles are defined for the same element, the browser applies the style with the highest specificity.

### Calculation of Specificity:

Specificity is represented using four values: `a, b, c, d`. These values are calculated as follows:

- `a` represents the number of inline styles.
- `b` represents the number of IDs in the selector.
- `c` represents the number of classes, attributes, or pseudo-classes in the selector.
- `d` represents the number of elements or pseudo-elements in the selector.

### Examples:

1. **Inline Styles (Highest Specificity):**

   ```html
   <div style="color: red;">This text is red.</div>
   ```

2. **IDs:**

   ```css
   #unique-id {
     color: blue;
   }
   ```

3. **Classes and Elements:**

   ```css
   .class1 {
     color: green;
   }
   div {
     color: purple;
   }
   ```

4. **Combination of Selectors:**

   ```css
   div.class1 p {
     color: orange;
   }
   ```

5. **Pseudo-classes and Pseudo-elements:**
   ```css
   a:hover {
     color: pink;
   }
   ```

### Specificity Rules:

- Inline styles have the highest specificity and override all other styles.
- ID selectors have higher specificity than class selectors.
- Class selectors have higher specificity than element selectors.
- The more specific selector will override less specific selectors.
- When two selectors have equal specificity, the one defined later in the stylesheet takes precedence.

### Importance:

Understanding specificity helps developers write CSS rules effectively, avoid unintended style conflicts, and ensure the desired styles are applied consistently across the website or web application.

### Conclusion:

Specificity plays a crucial role in determining which CSS rules are applied to elements. By mastering specificity, developers can write cleaner, more maintainable CSS code and avoid common styling pitfalls.
