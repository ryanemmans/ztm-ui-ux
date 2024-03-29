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

### [GRID CHEATSHEET!](https://grid.malven.co/)

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

- The above can also be used for `grid-row`, but we have to be careful with positioning
- `justify-self` - determines position of column (`start` or `end`)
- `align-self` - determines position of row (`start` or `end`)

## Exercise: CSS Layout

- [HTML](../section37/css-layout/index.html)
- [CSS](../section37/css-layout/style.css)

## Solution: Navigation Bar

```css
body {
  margin: auto 0;
}

.zone {
    /* padding:30px 50px;
    margin:40px 60px; */
    cursor:pointer;
    /* display:inline-block; */
    color:#FFF;
    font-size:2em;
    border-radius:4px;
    border:1px solid #bbb;
    transition: all 0.2s linear;
}

/* NAV */
.main-nav {
  display: flex;
  list-style: none;
  font-size: 0.7em;
  margin: 0;
}

@media only screen and (max-width: 600px) {
  .main-nav {
    font-size: 0.5em;
    padding: 0;
  }
}

.push {
  margin-left: auto;
}

li {
  padding: 20px;
}

a {
  color: #f5f5f6;
  text-decoration: none;
}
```

## Solution: Cover

```css
/* COVER */
.container {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 50vh;
}
```

## Solution: Project Grid + Footer

```css
/* GRID */
.grid-wrapper {
  display: grid;
  gap: 20px;
  grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
}

.box > img {
  width: 100%;
}

.box {
  background-color: #444;
  padding: 130px;
  margin: 20px;
}

footer {
  text-align: center;
}
```

## Solution: Prettify

- The key point is to start with your layout using Flexbox and CSS Grid
- From there it is up to your creativity to put content in its place and build on aesthetics and beauty

```css
body {
  margin: auto 0;
  font-family: Arial, Helvetica, sans-serif;
}

.box:hover {
  -webkit-transform: rotate(-7deg);
  -moz-transform: rotate(-7deg);
  -o-transform: rotate(-7deg);
  transform: rotate(-7deg);
}

/* NAV */

.sticky {
  position: fixed;
  top: 0;
  width: 100%;
  z-index: 1;
}

.cover {
  width: 30rem;;
}
```

## The Truth About CSS

- CSS is notoriously difficult and can be frustrating to learn
- There are so many properties and no way to remember all of them
  - If you are going to pursue being a developer, do not get hung up on CSS
  - Instead focus on JavaScript, as it will be roughly 80% of your job
    - More CSS knowledge will come with time.
- For design roles, HTML/CSS knowledge will be more important.

## END OF COURSE!! 🎉

- - -

[back](../README.md)
