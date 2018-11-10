## 1. Incredibly Easy Layouts with CSS Grid
Explicit vs implicit grid. The browser will decide implicit.
Grid container, all direct children becomes item. Everything that's outside that container cannot be placed on that grid.
Image are inline, they have a bit of line-height so that why display block.
Fraction of the space.

## 2. Flexibility & The Fold – new possibilities with CSS Grid
We don't have control of the width of the viewvport.
We care about left and right, but what about bottom and top? That's where the 'fold' comes in.
'We have no idea where the fold is'. It's from news, things above the fold would apear in the newsstand.
Bottom is basically the 'fourth edge'. Viewport units make sure you can design for height.
Viewport is basically a box.

`max content` large as possibly but no larger then the content.

## 3. Responsive Mondrian
Peter Mondrian; get rid of ornaments, but still symmetrical.
auto-fit; browser decides the amount of tracks
Automatically one cell if you don't tell an item how bit it should be
Auto-flow dense; not in source order.

## 4. Internet Explorer + CSS Grid????
non-grid supported browsers, just one single column? Progressive enhancement.
Feature query; supports display grid

## 5. Flexbox vs. CSS Grid — Which is Better?
Does this replace flexbox? No, mix grid with flexbox etc.
* Flexbox lines up in one direction wrap etc. Flexbox only row.
* Grid two directions, thinks about both of them

Grid can overlap items, with flexbox you can not.

## 6. Innovative & Practical Graphic Design with CSS Grid
Simple layout for browsers that don't support grid, and then use supports to enhance.

## 7. CSS Grid like you are Jan Tschichold
You can transform on a whole grid to get some really interestinng layouts.
You can't style the grid, so you have to place an element on the grid and style that.
Transforms don't alter the painting. Writing-mode takes up space.
