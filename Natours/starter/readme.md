# Three pillars of good html and css

## Responsive design

- Fluid layouts
- Media queries
- Responsive images
- Correct units
- Desktop first vs mobile first

## Maintable and scalable code

- Clean
- Easy to understand
- Growth
- Reusable
- How to organize files
- How to name classes
- How to structure HTML

## Web performance

- Less HTTP requests
- Less code
- Compress code
- Use a preprocessor
- Less images
- Compress images

# What happens to CSS when we load up a webpage

1. Load html
2. Parse html -> Load css -> parse css
3. Browser generate DOM
4. The final css is stored in the css object model (cssom)

DOM and CSSOM forms a `Render tree`

To render the page: visual formatting model

Final rendered website

# Parse CSS

## CSS terminology

- Selectors and declaration blocks

## Cascade

Combine and resolve conflicts between rules and declarations

Importance -> Specificity -> Source order

## Specificity

inline style, id, classes, element (a, div etc.)
(0,0,0,0)

## How css values are processed

Percentage and relative value are always converted to pixels

### Rem font-size

Always relative to root font-size

## How units are converted from relative to absolute (PX)

The percentage based unit is always based on the parent element

### em (font)

3 x parent element computed font-size = (3 \* 24) = 72px

### em (lengths)

x _ current element computed font-size (3 _ 16) = 48px

### rem (font, length)

x \* root computed font-size

#### Why use rem and em's if they are based on font size?

We can build more robust responsive layouts, because by changing font size, we will automatically change length. Gives flexibility.

### vh

1 vh = 1 % of view height

### vw

1 vw = 1 % of view width
