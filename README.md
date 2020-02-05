# Advanced CSS Course

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

---

## Useful Links

### Clippy

Url: [https://bennettfeely.com/clippy/](https://bennettfeely.com/clippy/)
