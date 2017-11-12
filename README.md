# Lab 07 exercise

A simple CSS animation for a common visual effect, using the `transition` property.

## How `transition` works

The `transition` property simply "prepares" an element for a style transition - it does NOT trigger the transition.

```css
figcaption {
  /* figcaption styles here */
  transition: all .5s;
}
```

The styles that are transitioned are only applied to the `figcaption` element when they're triggered.

In this particular example, `transition` is triggered by **hovering** over the`figure` element (which is the *parent* of the `figcaption` element). The `transition` property is then applied to `all` the hover styles, over 0.5 seconds.

```css
figure:hover figcaption {
  /* figcaption hover styles here */
}
```