# Section 35 - Extra: CSS 3

## Your First CSS

Cascading Style Sheets

- Cascading - always takes selector at the end
- ` <link rel="stylesheet" type="text/css" href="style.css">`
  - Reference stylesheet in `<head>` section of html file
  - Ideal for larger pages/files
- Can also use inline styling in `<body>`, or `<style>` tags in `<head>`
- Separation of concerns - allows developers to work on separate HTML and CSS files, as opposed to using inline styling

## CSS Properties

CSS Example from exercise:

```css
body {
  background-image: url(img/background-img.jpg);
  background-size: cover;
}

h2 {
  color: #AA3939;
  text-align: center;
  border: 2px solid rgba(255, 170, 170, 0.5);
  cursor: pointer;
}

p {
  color: green;
}

li {
  list-style: none;
  display: inline-block;
}
```

## CSS Selectors

### CSS Cheat Sheet

Reference:

- [CSS Selector Reference](https://www.w3schools.com/cssref/css_selectors.asp)
- [CSS Tricks Almanac](https://css-tricks.com/almanac/)
- [Cascade and Inheritance](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Cascade_and_inheritance)

Cascading Style Sheets - at the most basic level it indicates that the order of CSS rules matter.

```pt
.class (many)
#id (only one)
* (all)
element
element, element (both)
element element (one inside other)
element > element (only applies to child of parent)
element + element (exactly after, not inside)
:hover
:last-child
:first-child
!important (not recommended) (overrides all, breaks the rules of cascading)
```

What selectors win out in the cascade depends on:

- Specificity ([Specificity Calculator](https://specificity.keegan.st/))
- Importance
- Source Order

Inline styles will always take most specificity / priority

## Text and Font

- Import from Google Fonts
  - `  <link href="https://fonts.googleapis.com/css2?family=Poiret+One&display=swap" rel="stylesheet">`

```css
p {
  line-height: 50px;
  font-style: italic;
  font-weight: bold;
  font-size: 180%;
  font-family: 'Poiret One', cursive;
}
```

## Images in CSS

```css
img {
  float: right;
}

footer {
  clear: both;
  text-align: center;
}
```

## Box Model

```css
.boxmodel {
  border: 5px solid red;
  display: inline-block;
  padding: 5px 20px;
  margin: 0px 20px;
  width: 33px;
  height: 55px;
}
```

## px vs em vs rem

- pixels are absolute units
- `em` is the size relative to it's parent element

```css
p {
  font-size: 10px;
}

span {
  font-size: 3em;
}
```

- `rem` is the size relative to root element (`<html>`)
  - Changing parent element does not affect this

[What’s The Difference Between PX, EM, REM, %, VW, and VH?](https://elementor.com/help/whats-the-difference-between-px-em-rem-vw-and-vh/)

## Critical Render Path

## Flexbox

## CSS 3

## Responsive UI

- - -

[back](../README.md)
