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
