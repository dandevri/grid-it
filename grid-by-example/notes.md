## Get started
By default children of the grid will be layout by row.
Order only changes visually, so be careful with source order.

Grid Layout gives us a method of creating grid structures that are described in CSS and not in HTML.

Grid Layout lets us properly separate the order of elements in the source from their visual presentation. As a designer this means you are free to change the location of page elements as is best for your layout at different breakpoints and not need to compromise a sensible structured document for your responsive design.

> Flexbox is for one-dimensional layouts - anything that needs to be laid out in a straight line (or in a broken line, which would be a single straight line if they were joined back together). Grid is for two-dimensional layouts. It can be used as a low-powered flexbox substitute (we’re trying to make sure that a single-column/row grid acts very similar to a flexbox), but that’s not using its full power.

## Placing items on the grid
Grid defaults to spanning one track

>  When grid first shipped in browsers the column-gap, row-gap and gap properties were prefixed with the grid- prefix as grid-column-gap, grid-row-gap and grid-gap respectively.

Gaps only appear between tracks of the grid, they do not add space to the top and bottom, left or right of the container. 

## Sizing of tracks and Items
ch = character zero. fr unit. Sizing keywords.
You can use sizinng keywords such as min-content with CSS grid. `fit-content`

## Alignment of the grid and grid items
Box alignment specification. 
* `justify items` Align items inside an area.
* `justify content` Also justify and align the tracks.
You can also use space-between etc. 

> These alignment properties that we first met in the flexbox specification have been moved into a new specification called Box Alignment Level 3. This specification has details for how alignment should work in all of the different layout methods.

## How does grid work with Flexbox and other specs?
> The basic difference between CSS Grid Layout and CSS Flexbox Layout is that flexbox was designed for layout in one dimension - either a row or a column. Grid was designed for two-dimensional layout - rows, and columns at the same time.

Flexbox works from the content out.
Grid works from the layout in. 

> The fr unit, when combined with the minmax() function can give us very similar behavior to the flex properties in flexbox while still enabling the creation of a layout in two dimensions.

as currently defined, the reordering is only visual. It does not change the logical order of the document. In addition, we need to take great care in considering sighted keyboard users.

Grid is only a replacement for flexbox if you have been trying to make flexbox into a two-dimensional grid. If you want to take a bunch of items and space them out evenly in a single row, use flexbox.

CSS is full of physical positioning keywords – left and right, top and bottom.

Logical properties and values do not make an assumption about text direction. Which is why in Grid Layout we use the keyword start when aligning something to the start of the container. For me, working in English, start may well be on the left, however it doesn’t have to be, and the word start infers no physical location.

## Accessibility, browsers and backwards compatibility
Feature queries.

> Before deciding how you are going to support browsers without grid support, it is worth working out what you mean by support. Support might mean that the site has to look absolutely identical in all the browsers on your list. It might mean that you are happy for some finishing touches not to be available in all browsers. It might mean that you are testing these browsers but are completely happy for them to receive a much simplified experience.

The first part of the picture is the fact that browsers ignore CSS they don’t understand. If a browser that doesn’t support CSS Grid, comes across the grid-template-columns property, it doesn’t know what it is and so throws that line away and continues.

It is here that we come to an issue with simply being able to override one layout method with another. 

This is where Feature Queries can help. Feature Queries act much like a Media Query, instead of checking for the width or orientation of a device, we check to see if the browser supports a CSS feature.

As with any front-end technology choice, the decision to use CSS Grid Layout will come down to the browsers your site visitors are typically using

This had some advantages over the “CSS Positioning” that came afterwards, in that we could take advantage of the alignment and full height columns offered by table display. The biggest downside however was that it tied our design to the mark-up, often creating accessibility issues as it did so.

> Grid layout gives authors great powers of rearrangement over the document. However, these are not a substitute for correct ordering of the document source. The order property and grid placement do not affect ordering in non-visual media (such as speech). Likewise, rearranging grid items visually does not affect the default traversal order of sequential navigation modes (such as cycling through links, see e.g. tabindex HTML5).

* Start with a structured and accessible document
* Create a responsive, and responsible grid
* Returning to the source

The key here is to keep testing, a very simple test is to tab around the document. Does that order still make sense? 

there is a definite temptation when developing a site using CSS Grid Layout to flatten out the markup, to remove semantic elements in order to make it simpler to create a layout.
