# HTML/CSS Style Guide

### General

- no tabs

- 2 spaces for an indent

- No character limit the line lengths, but be reasonable.

### Semantic (when possible)

Code should be as semantic as possible (it should describe what it contains)

Examples:

navbars should be written with the nav tag
```html
<nav>

  nav bar stuff
  
</nav>
```

instead of

```html
<div>

nav bar stuff

</div>
```

footers should be written with the footer tag 

```html
<footer>

  footer stuff

</footer>
```

instead of

```html
<div class="footer">

footer stuff

</div>
```

When using frameworks such as bootstrap it's extremely common to fall into the 
trap known as "div soup" There are about a 100 HTML Tags, each one tag is 
carefully created and exist for a reason, so use them. Having good semantic HTML
Makes code much easier to read, and can help with SEO.


### Tags

HTML is a language that lends itself to nesting and for that reason we will be
using ___2 spaces___ not 4 for indents. Also it helps to add logical spacinging
in between tags. Think about an english paper, your not going to single space it
it's a well known fact that double spaced is easier to read. So why wouldn't
you add spaces to your code.

BAD:
```html
<div class="row">
  <div class="col-xs-12">
    <p> Hello World </p>
  </div>
</div>
```

While this isn't hard to read when there's only 5 lines of code with you start
writing 100s of lines of code tight spacing makes it much harder to read.

```html
<div class="row">

  <div class="col-xs-12">

    <p> Hello World </p>

  </div>

</div>
```

or

```html
<div class="row">
  <div class="col-xs-12">

    <p> Hello World </p>

  </div>
</div>
```

It is okay to not put a space between the 2 divs (in fact it's probably preferred 
in this situation), because rows and columns 
logically group together, but this is one of those things where you're going
to have to use your best judgment. As a rule of thumb if you're not sure put a 
space between it. You're much more likely to have too little spacing than too
much

##### Attributes

- First rule of CLKTech  ___NO STYLE TAGS___
- Second rule of CLKTech  ___NO STYLE TAGS___

Stlye tags are horrible and can very quickly make your code impossible to deal
with. CSS files exist for a reason use them. 

- No spacing in between '='

Bad:

```html
<div class = "row">

</div>
```

__Good__:

```html
<div class="row">

</div>
```


## CSS

For the point of consistency  use 2 spaces when writing CSS code. And include 
blank lines between groups. Class names and IDs should be used to describe the
content they contain. The goal of CSS should be to write as few lines as possible
take advantage of the "cascading" affect of CSS.

___ALL CSS should be written in a CSS file not a style tag___
