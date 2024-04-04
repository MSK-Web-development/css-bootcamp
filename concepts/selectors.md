# CSS selectors

1. **Element Selector (`element`)**:

   Element selectors target HTML elements by their tag name. They apply styles to all instances of the specified element in the document.

   ```css
   /* Selects all <p> elements and sets their font color to blue */
   p {
     color: blue;
   }
   ```

2. **Class Selector (`.class`)**:

   Class selectors target elements based on their class attribute. They are prefixed with a dot (.) followed by the class name. Multiple elements can share the same class.

   ```css
   /* Selects all elements with the class "highlight" and sets their background color to yellow */
   .highlight {
     background-color: yellow;
   }
   ```

   HTML:

   ```html
   <p class="highlight">This paragraph is highlighted.</p>
   <div class="highlight">This div is also highlighted.</div>
   ```

3. **ID Selector (`#id`)**:

   ID selectors target a single element with a unique identifier. They are prefixed with a hash (#) followed by the ID value. IDs should be unique within the HTML document.

   ```css
   /* Selects the element with the ID "header" and sets its font size to 24px */
   #header {
     font-size: 24px;
   }
   ```

   HTML:

   ```html
   <div id="header">This is the header.</div>
   ```

4. **Attribute Selector (`[attribute]`, `[attribute=value]`, `[attribute~=value]`, `[attribute|=value]`, `[attribute^=value]`, `[attribute$=value]`, `[attribute*=value]`)**:

   Attribute selectors target elements based on the presence or value of their attributes. They are enclosed in square brackets.

   ```css
   /* Selects all <a> elements with a "href" attribute */
   a[href] {
     color: blue;
   }

   /* Selects <input> elements with a "type" attribute equal to "text" */
   input[type="text"] {
     border: 1px solid black;
   }

   /* Selects all elements with the "class" attribute containing "highlight" */
   [class~="highlight"] {
     background-color: yellow;
   }

   /* Selects all elements with the "lang" attribute set to "en" or starting with "en-" */
   [lang|="en"] {
     font-family: Arial, sans-serif;
   }

   /* Selects all <a> elements with the "href" attribute starting with "https://" */
   a[href^="https://"]
   {
     color: green;
   }

   /* Selects all <img> elements with the "src" attribute ending with ".png" */
   img[src$=".png"] {
     border: 1px solid red;
   }
   ```

5. **Pseudo-classes (`:pseudo-class`)**:

   Pseudo-classes target elements based on their state or position in the document tree.

   ```css
   /* Selects the first <p> element and sets its color to red */
   p:first-child {
     color: red;
   }

   /*This pseudo-class selects the last child element of its parent.*/
   ul:last-child {
     color: red;
   }

   /*This pseudo-class selects elements based on their ordinal position within their parent.*/
   ul:nth-child(odd) {
     background-color: lightgray;
   }

   /*This pseudo-class selects elements that are the only child of their parent.*/
   span:only-child {
     color: red;
   }

   /* Selects <input> elements when they are in focus */
   input:focus {
     background-color: lightblue;
   }

   /* This pseudo-class applies when the user's mouse hovers over an element. */
   button:hover {
     background-color: lightblue;
   }

   /*This pseudo-class selects elements that do not match a specified selector.*/
   p:not(.special) {
     font-style: italic;
   }
   ```

6. **Pseudo-elements (`::pseudo-element`)**:

   Pseudo-elements allow styling specific parts of an element.

   ```css
   /* Styles the first letter of <p> elements */
   p::first-letter {
     font-size: 24px;
   }

   /* Styles the first line of <div> elements */
   div::first-line {
     color: green;
   }
   ```

   HTML:

   ```html
   <p>This is a paragraph.</p>
   <div>This is a division.</div>
   ```

7. **Universal Selector (`*`)**:

   The universal selector matches any element in the document.

   ```css
   /* Sets margin and padding to zero for all elements */
   * {
     margin: 0;
     padding: 0;
   }
   ```

These are the primary types of CSS selectors along with examples. Understanding these selectors and their usage will help you effectively style HTML elements in your web projects.
