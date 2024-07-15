# 0x02 ADVANCED CSS

As a result of this project and other personal studying, I am familiar with  the following concepts, I easily understand and would hardly forget:

Selectors, properties, and values
The difference between block and inline styling
How to ensure consistency across all browers (CSS reset)
How to setup CSS variables
The differences between inline, embeded and external CSS
How grid systems work (with floats)
The difference between icons webfonts and SVG icons
The difference between pseudo-classes and pseudo-elements
How to make background gradients
How to animate elements in CSS
How to transform (2d, 3d) elements
What vendor prefixes are

Memory updated
Sure, let's dive into these CSS concepts with examples to make them clear and memorable.

Selectors, Properties, and Values
Selectors are patterns used to select the elements you want to style. Properties are the aspects of the elements that you want to change. Values are the settings for those properties.

css

/* Selector */
p {
  /* Property: color, Value: red */
  color: red;
  /* Property: font-size, Value: 16px */
  font-size: 16px;
}
Block vs Inline Styling
Block elements take up the full width available and start on a new line. Examples include <div>, <p>, and <h1>.

Inline elements take up only as much width as necessary and do not start on a new line. Examples include <span>, <a>, and <img>.

html

<div style="background-color: lightblue;">This is a block element</div>
<span style="background-color: lightgreen;">This is an inline element</span>
CSS Reset
A CSS reset ensures consistency across different browsers by removing default browser styles.

css

/* CSS Reset Example */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
Setting Up CSS Variables
CSS variables (also known as custom properties) allow you to reuse values throughout your CSS.

css

:root {
  --main-color: #3498db;
  --padding: 10px;
}

div {
  color: var(--main-color);
  padding: var(--padding);
}
Inline, Embedded, and External CSS
Inline CSS is added directly to an HTML element using the style attribute.

html

<p style="color: red;">This is a paragraph.</p>
Embedded CSS is added within the <style> tag inside the <head> of your HTML document.

html

<head>
  <style>
    p {
      color: blue;
    }
  </style>
</head>
External CSS is written in a separate file and linked to your HTML document.

html

<head>
  <link rel="stylesheet" href="styles.css">
</head>
Grid Systems with Floats
Using floats to create a grid system involves floating elements to the left or right to create a column layout.

html

<div class="container">
  <div class="column">Column 1</div>
  <div class="column">Column 2</div>
  <div class="column">Column 3</div>
</div>

<style>
.container {
  width: 100%;
}

.column {
  float: left;
  width: 33.33%;
  padding: 10px;
  box-sizing: border-box;
}
</style>
Icon Webfonts vs SVG Icons
Icon Webfonts use fonts to display icons. Examples include Font Awesome and Material Icons.

html

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
<i class="fas fa-home"></i> <!-- Font Awesome Icon -->
SVG Icons use Scalable Vector Graphics and can be styled with CSS.

html

<svg width="24" height="24">
  <circle cx="12" cy="12" r="10" stroke="black" stroke-width="2" fill="red" />
</svg>
Pseudo-Classes vs Pseudo-Elements
Pseudo-classes target elements based on their state or position.

css

a:hover {
  color: green; /* Changes color when the link is hovered over */
}
Pseudo-elements target specific parts of an element.

css

p::first-line {
  font-weight: bold; /* Styles the first line of a paragraph */
}
Background Gradients
Creating background gradients with CSS can add depth to your designs.

css

div {
  background: linear-gradient(to right, red, yellow);
  height: 100px;
  width: 100px;
}
Animating Elements in CSS
Using @keyframes to define animations.

css

@keyframes example {
  from {background-color: red;}
  to {background-color: yellow;}
}

div {
  width: 100px;
  height: 100px;
  background-color: red;
  animation-name: example;
  animation-duration: 4s;
}
Transforming Elements (2D, 3D)
2D Transforms include translate, rotate, scale, and skew.

css

div {
  transform: rotate(45deg); /* Rotates the element 45 degrees */
}
3D Transforms include rotateX, rotateY, and rotateZ.

css

div {
  transform: rotateY(180deg); /* Rotates the element 180 degrees around the Y-axis */
}
Vendor Prefixes
Vendor prefixes are used to ensure CSS properties work across different browsers.

css

div {
  -webkit-transition: all 0.5s; /* Safari and Chrome */
  -moz-transition: all 0.5s;    /* Firefox */
  -o-transition: all 0.5s;      /* Opera */
  transition: all 0.5s;         /* Standard */
}
These examples should help solidify your understanding of these CSS concepts. Feel free to experiment with them to get a deeper grasp!