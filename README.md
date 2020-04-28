# Advanced CSS Course

## Three Pillars to Write Good HTML and CSS

1. Responsive design
1. Maintainable and scalable code
1. Web performance

### Responsive design

- Fluid layouts
- Media queries
- Responsive images
- Correct units
- Desktop-first vs mobile-first

### Maintainable and scalable code

- Clean
- Easy-to-understand
- Growth
- Reusable
- How to organize code
- How to name classes
- How to structure HTML

### Web performance

- Less HTTP requests
- Less code
- Compress code
- Use a CSS preprocessor
- Less images
- Compress images

## CSS Properties

### Line Height

The line-height property specifies the height of a line

- Default value: normal
- Other values: percentage, 1.6 (recommended)
- Inherited: yes

### Position

The position property specifies the type of positioning method used for an element.

There are five different position values:

1. static: HTML elements are positioned static by default.

Static positioned elements are not affected by the top, bottom, left, and right properties.

An element with position: static; is not positioned in any special way; it is always positioned according to the normal flow of the page

1. relative: An element with position: relative; is positioned relative to its normal position
1. fixed: An element with position: fixed; is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled
1. absolute: An element with position: absolute; is positioned relative to the nearest positioned ancestor (instead of positioned relative to the viewport, like fixed)
1. sticky: An element with position: sticky; is positioned based on the user's scroll position

### Display

The display property specifies the display behavior (the type of rendering box) of an element.

In HTML, the default display property value is taken from the HTML specifications or from the browser/user default style sheet. The default value in XML is inline, including SVG elements.

- Default value: ?
- Inherited: no
- Animatable: no

### Box Shadow

The box-shadow property attaches one or more shadows to an element

`box-shadow: none|h-offset v-offset blur spread color |inset|initial|inherit;`

### Transform

The transform property applies a 2D or 3D transformation to an element. This property allows you to rotate, scale, move, skew, etc., elements.

- Default value: none
- Inherited: no
- Animatable: yes

### Transition

CSS transitions allows you to change property values smoothly, over a given duration.

### Backface Visibility

The backface-visibility property defines whether or not the back face of an element should be visible when facing the user.

The back face of an element is a mirror image of the front face being displayed.

This property is useful when an element is rotated. It lets you choose if the user should see the back face or not.

### Key frames

The @keyframes rule specifies the animation code.

The animation is created by gradually changing from one set of CSS styles to another.

During the animation, you can change the set of CSS styles many times.

### Animation-fill-mode

The animation-fill-mode property specifies a style for the element when the animation is not playing (before it starts, after it ends, or both).

CSS animations do not affect the element before the first keyframe is played or after the last keyframe is played. The animation-fill-mode property can override this behavior.

`animation-fill-mode: none|forwards|backwards|both|initial|inherit;`

### Pseudo-classes

A pseudo-class is used to define a special state of an element.

For example, it can be used to:

- Style an element when a user mouses over it
- Style visited and unvisited links differently
- Style an element when it gets focus

### Pseudo-elements

A CSS pseudo-element is used to style specified parts of an element.

For example, it can be used to:

- Style the first letter, or line, of an element
- Insert content before, or after, the content of an element

```css
selector::pseudo-element {
  property: value;
}
```

### The Cascade and Specificity

- Importance > Specificity > Source Order
- Inline, IDs, Classes, Elements (0,0,0,0)

### Value Processing

- Declared value > Cascaded value > Specified value > Computed value > Used value> Actual value

#### EM's and REM's

- em are measured relative to their parent font-size, if used to specify font-size
- em are measured relative to the current font-size, if used to specify lengths
- rem are always measured relative to the documents root font-size

### Inheritance

- Inheritance passes the values for some specific properties from parents to children - more maintainable code
- Properties related to text are inherited: font-size, font-family, color,...
- The computed value of a property is what gets inherited, not th declared one
- The `inherit` keyword forces inheritance on a certain property
- The `initial` keyword resets a property to its initial value

---

### Box Types

#### Inline (display: inline)

- Content distributed in lines
- Occupies only content's space
- No line-breaks
- No heights and widths
- Padding and margins only horizontal (left and right)

#### Block-level (display: block)

- Elements formatted visually as blocks
- 100% of parent's width
- Vertically, one after another

#### Inline-Block (display: inline-block)

- A mix of inline and block
- Occupies only content's space
- No line-breaks
- Box-model applies as showed

---

### Positioning schemes

#### Normal Flow (position: relative)

- Default positioning scheme
- Not floated
- Not absolutely positioned
- Elements positioned according to their source order

#### Absolute Positioning (position: absolute, position: fixed)

- Element is removed from the normal flow
- No impact on surrounding content or elements
- We use top, bottom, left, and right to offset the element from its relatively positioned container

#### Floats (float: left, float: right)

- Element is removed from the normal flow
- Text and inline elements will wrap around the floated element
- The container will not adjust its height to the element

---

### BEM - Block Element Modifier

- Block: standalone component that is meaningful on its own
- Element: part of a block that has no standalone meaning
- Modifier: a different version of a block or an element

```css
.block {}
.block__element {}
.block__element--modifier {}
```

---

### The 7-1 Pattern

- 7 different folders for partial Sass files
- 1 main Sass file to import all other files into a compiled CSS stylesheet

#### The 7 folders

- base/ - imports all code from other files
- components/ - independent building blocks
- layout/ - the whole page styles (header, footer, ...)
- pages/
- themes/
- abstracts/
- vendors/

---

### SASS

- CSS pre-processor
- Adds power and elegance to the language
- Sass compiles to CSS

#### Features

- Variables: reusable values such as colors, font-sizes, spacing
- Nesting: nest selectors inside of one another, allows to write less code
- Operators: mathematical operators inside of CSS
- Partials and imports: write CSS in different files and importing them all into one single file
- Mixins: write reusable pieces of CSS code
- Functions: similar to mixins, they produce a value than can be later used
- Extends: make different selectors inherit declarations that are common to all of them
- Control directives: for writing complex code using conditionals and loops

#### Working with SASS

- Install the package `node-sass` to compile SASS code to CSS code

```bash
node-sass sass/main.scss css/style.css
```

### Responsive Design Principles

1. Fluid Grids and Layouts

To allow content to easily adapt tp the current viewport width used to browse the website. 
Use % rather than px for all layout-related lengths.

2. Flexible/Responsive Images

Images behave differently than text content.
Ensure they adapt nicely to the current viewport.

3. Media Queries

Change style on certain viewport widths (breakpoints), allowing to create different versions of our website for different screen widths.

#### Layout Types

1. Float Layouts
2. Flexbox
3. CSS Grid 

## Useful Links

### Clippy

Url: [https://bennettfeely.com/clippy/](https://bennettfeely.com/clippy/)
