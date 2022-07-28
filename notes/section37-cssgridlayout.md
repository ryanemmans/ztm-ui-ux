# Section 37 - Extra: CSS Grid + CSS Layout

## CSS Grid vs Flexbox vs Bootstrap

Using CSS for layout is a very important skill as a developer

- Three of the current best ways
  1. Flexbox
  2. Bootstrap
  3. Grid
- Flexbox and Grid are complementary tools and should be thought of as working really well together
  - Flexbox is good for one dimension (columns)
  - Grid is very powerful especially for 2-dimensional layouts (columns and rows)

<img src="https://miro.medium.com/max/860/1*FifZUGz97Onmb7RUOairbg.png" width="600" alt="Flexbox vs Grid">

- Bootstrap came at a time when Flexbox and CSS Grid did not yet exist
- If we know Flexbox and Grid, we can create any layouts we want
  - It is now also more valuable to employers
  - Flexbox is more widely supported across browsers
    - It is only a matter of time until Grid is more widely supported

## CSS Grid

```css
.container {
  display: grid;
  gap: 20px;
  grid-template-columns: 1fr 1fr 2fr;
  grid-template-rows: 1fr;
  /* We will use fraction, instead of using pixels, percentage, em, or rem */
}
```

```css
grid-template-columns: repeat(3, 1fr);
/* SAME AS */
grid-template-columns: 1fr 1fr 1fr;
```

- `auto` (in place of, say, `1fr` could be thought of as max size of content
  - following columns or rows will match that dimension
- `justify-items` and `align-items` - `stretch` is default
  - `start` and `end` align contents in grid along the *row axis*
  - Grid can be viewed in Chrome Dev Tools

```css
grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
/* Column system adjusts according to size of viewport */
```

```css
grid-column: 1/4;
/* Start/End, content will span these specific columns */
grid-column: 1/-1;
/* Will take the content to the end of the grid */
grid-column: span 2;
/* Content will span 2 grids */
```

The above can also be used for `grid-row`, but we have to be careful with positioning

- `justify-self` - determines position of column (`start` or `end`)
- `align-self` - determines position of row (`start` or `end`)

### [GRID CHEATSHEET!](https://grid.malven.co/)

## Exercise: CSS Layout

## Solution: Navigation Bar

## Solution: Cover

## Solution: Project Grid + Footer

## Solution: Prettify

## The Truth About CSS

- - -

[back](../README.md)
