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

## 8. Obliterate Boxiness with CSS Shapes
Effects are dramatic and fallback is easy with css shapes.
Shape-outside; run the flow content.

## 9. Basics of CSS Grid: The Big Picture
Comes from CSS specification, the browser builders use this to implement features.
Level 1 specification, that's locked down.
* Grid container
* Grid items

Grid items need to be direct children. Doesn't matter what elements they are.
Level 2 might have a subgrid, you can pull a grid through the grandchildren.
For now you have to use nested grids.

* Every unit is a grid cell
* Grid area can be multiple cells
Every cell is a square.

Rows and columns are both tracks.
Grid-lines and gaps. You cannot put content in a grid gap.

Explicit grid also defines negative numbers, other way around.
Two different ways to target lines.

Implicit, the browser creates tracks for you.

Grid only lives in the CSS so it can't be styled. Doesn't exist in the dom.

## 10. Using Flexbox + CSS Grid Together: Easy Gallery Layout
Flexbox most of the time want to give items the full width (stretch) and with a grid
layout most of the time you don't want that. Grid is better suited for that.

Fallback layouts from grids is not really that hard.

## 11. Whitespace on The Web! — with CSS Grid
Grid is really great for using white space.
Management of white space is the best design tool. 
Having rows chnges everything. If you explicit create a grid you can manage the white space.

## 12. HTML Source Order and When There’s No CSS
What is the source order if there is not layout? You want to design the order
when no CSS is applied.
* Screen reader; there are also people who can see but have limited vision. Dyslexia.
* SEO
* Reader view; without css and javascript

Put something on the bottom in the source order but visually on the top of the page. So screen readers
get to the content first.

