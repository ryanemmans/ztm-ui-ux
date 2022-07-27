# Section 36 - Extra: Bootstrap, Templates, and Building Your Startup Landing Page

## Evolving Technology

- What we're learning will always change over the years
  - Everything in tech moves and changes quickly
  - Programming languages, text editors, dependencies, best practices, libraries, APIs
- This course is designed to learn old methods (eg: React) and update them
- A developer is maintaining software and programs, which are always evolving
  - Ensure that your code is running years from now
- Developers are problem solvers, constantly fluidly changing and evolving *with* the technology

## Bootstrap Introduction

[getbootstrap.com](https://getbootstrap.com/)

- Bootstrap is essentially a CSS file and a JavaScript file
  - It prevents us as developers from having to keep reinventing the wheel
  - Enables us to build websites very quickly
  - Components can be implemented as UI elements
- With the component building blocks, you can use Bootstrap classes as well as add custom CSS styles on top
  - Enables endless customization

## Bootstrap

- CSS and JS files could be downloaded
- Or linked through a CDN
  - Content Delivery Network, where Bootstrap hosts the files for us
  - [What is a CDN?](https://www.cloudflare.com/learning/cdn/what-is-a-cdn/)

  ```html
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-gH2yIJqKdNHPEq0n4Mqa/HGKIhSkIHeL5AyhkYV8i59U5AR6csBvApHHNl/vI1Bx" crossorigin="anonymous">
  <link rel="stylesheet" type="text/css" href="style.css">
  <!-- Our own stylesheet will override Bootstrap's default styles -->
  ```

  ```html
  <!-- Always place JavaScript at bottom of <body> -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0/dist/js/bootstrap.bundle.min.js" integrity="sha384-A3rJD856KowSb7dwlZdYEkO39Gagi7vIsF0jrRAoQmDKKtQBHUuLZ9AsSv4jD4Xa" crossorigin="anonymous"></script>
  ```

[Bootstrap exercise](../section36/bootstrap/index.html)

## Bootstrap 5 Update

- Packages, libraries, and tools are constantly being updated
  - Projects must be maintained
  - Bootstrap's latest version is 5.2.0, and our code must reflect that.

## Bootstrap Grid

[Grid Documentation](https://getbootstrap.com/docs/5.2/layout/grid/)

```html
<div class="container">
  <div class="row align-items-start">
    <div class="col col-sm-6 col-md-12 col-lg-12">
      1 of 3 columns
    </div>
    <div class="col col-sm-3 col-md-6 col-lg-12">
      2 of 3 columns
    </div>
    <div class="col col-sm-3 col-md-6 col-lg-12">
      3 of 3 columns
    </div>
  </div>
</div>
```

## Exercise: Startup Landing Page

## Exercise: Adding Email Subscribe Form with MailChimp

## Exercise: Putting Your Website Online

## Developer Fundamentals: IV

## Using Templates

- - -

[back](../README.md)
