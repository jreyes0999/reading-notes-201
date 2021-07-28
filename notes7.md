# CSS Layout

- CSS Layout
  - Display is CSS’s most important property for controlling layout. Every element has a default display value depending on what type of element it is. The default for most elements is usually block or inline. A block element is often called a block-level element. An inline element is always just called an inline element.

- CSS Elements
  - `<div></div>` div is the standard block-level element. A block-level element starts on a new line and stretches out to the left and right as far as it can. Other common block-level elements are `p` and `form`. IN HTML5 ther is `header`, `footer`, `section`, and many more.

- Inline
  - Inline span is the standard inline element. An inline element can wrap some text inside a paragraph `<span></span>` without disrupting the flow of that paragraph. The `a` element is the most common inline element, since it's used them for links.

- None
  - Another common display value is `none`. Some specialized elements such as script use this as their default. It is commonly used with JavaScript to hide and show elements without actually deleting them.
  - This is different from visibility. Setting display to none will render the page as though the element does not exist. visibility: hidden; will hide the element, but the element will still take up the space it would if it was fully visible.

- Width/Height/Margins
 - Setting the width of a block-level element will prevent it from stretching out to the edges of its container to the left and right. Then, you can set the left and right margins to auto to horizontally center that element within its container. The element will take up the width you specify, then the remaining space will be split evenly between the two margins.
