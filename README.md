# Bootstrap4 - All Elements

Bootstrap 4 - All Elements

I have been searching the web for a 'kitchen sink' document of all Bootstrap 4 elements, but could never find one.  I found some UI kits out there and have borrowed the elements pages to create this.

When I create a UI kit from this, I create an SCSS folder inside the assets folder and create a file called custom.scss.  Using Atom I compile that file to the assets/css/custom.css and replace bootstrap.css in the head section of my index.html with custom.css.  Note that bootstrap.scss has to be imported at the bottom of the custom.scss file for this to work.

Here are some examples of overriding Bootstrap (using custom.scss).

```scss
// override bootstrap default theme colors
$theme-colors: (
  "primary": #375a7f,
  "secondary": #444,
  "success": #00bc8c,
  "info": #3498DB,
  "warning": #F39C12,
  "danger": #E74C3C,
);

// increase the default spacing
$spacer:1.25rem;

// adjust the default heading font weight
$headings-font-weight:300;

// adjust the default font weights
$font-weight-light:200;
$font-weight-normal:300;
$font-weight-bold:500;

// adjust the default font size
$font-size-base:1.2rem;

// add more spacers
$spacer: 1rem !default;
$spacers: (
    6: ($spacer * 4),
    7: ($spacer * 5),
    8: ($spacer * 7.50),
    9: ($spacer * 10)
  );

// set the button border radius
$btn-border-radius:2px;

// change the hyperlink color
$link-color: #00bc8c;

// remove underline from hyperlinks
$link-hover-decoration: none;


// Core bootstrap scss import - this should always be at the bottom of the custom.scss file
@import '../../bootstrap/scss/bootstrap';
```

View the <a href="https://steveshead.github.io/bootstrap4-elements-template/">demo</a> site <a href="https://steveshead.github.io/bootstrap4-element-template/">here</a>.
