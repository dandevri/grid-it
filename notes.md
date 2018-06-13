# CSS Grid

## 03 Grid Fundamentals
The idea of a grid, display grid it. You can then slice it. You can then splice each section in columns and rows. You can take each item and move / position it.

* Dice it in columns and rows (tracks)
* Items and lay them out inside the grid

Just as flexbox, CSS Grid container and CSS Grid items. Direct children. You then also need to slice and dice it.

Rows are automatically defined. Grid gap is spacing between each row and colum. Columns and rows collectively are called tracks. Margin between tracks.

Percentages aren't the best option, you have new unit in grid fr or auto.

If you don't specify the columns, you just have one.

## 04 Grid Tools
You can't really select tracks in the dev tools cause they are not really separate elements.

Devtools > Layout

Track are not numbers by the actual column itself but by the lines that start and stop them. Not by the column. So 2 columns is always 3 tracks.

Explicit = we created them
Implicit = browser created

## 05 Implicit Explicit
Explicit define what the columns should be, but implicit the rows. If you do not create them they are implicit.

Solid = Explicit  
Dotted = Implicit

If you add more items then let's say column browser will make implicit. So the solid lines are were the explicit lines end.

Grid auto rows; implicit created styling.

If you define columns, any extra will be turned into rows.

## 06 Grid Auto Flow
If items are added as columnns or as rows. What do we do with the extra item?
Row is default.

## 07 Sizing Tracks
Relates to box model. Percentage wil not include the grid gap.
Fractional unit; amount of space left when all elements are layed out. 
A bit like flex grow and shrink. fr = FRee space

Height of the element is a big as the content. So fr in rows don't work. Width is as viewport (block).
Auto = max size of content. Widthest content of width column.

## 08 Grid Repeat
How many you times you want to repeat it and what you want to repeat.
Multiple arguments it will alternate.

## 09 Sizing Grid Items
All previous stuff have been on the grid container.

Will lock the width of that column and that with fr will take up the free space.
Not width and content size but you can use spanning.

## 10 Placing Grid Items
Span and grid column; where to start and where to end.
* Column goes to full width
* Rows -1 goes to explicit width not bottom of grid.

## 11 
-

## 12 Auto Fit and Fill
Most used pieces of grid.
Auto-fill; figure out how many columns you need.
Auto-fit; grid stops at items. (explicit)

Difference is when you don't have enough items. With fill it wil create new columns.

## 13 Min Max
Mostly used with auto fit and fill. Will replace media queries.
Flow as wide as need to be. Minimum and maximum of the track. (max 1fr)
Fit-content function; gets a max width or height.

## 14 Template Areas
Other way of sizing and place grid items. Explicit say where you want to items to be. You name sections of the grid and place.
Also use them in media queries to resize.
Naming them is pretty good if you don't know how many numbers your track are going to be.

When you create areas, you get line names.
Name the areas and tag a start or end to it.

## 15 Naming lines
The lines are not the columns themselves lines inbetween columns.
Name them when you define them.

## 16 Auto Flow
More items that can fit it wil create a implicit row.
Dense will fill up the space to fit.
Mostly used when you don't care about the order the items are in.
Without auto flow dense you have holes.

## 17 Grid Alignment
Even if the site you are building is not grid heavy, grid can be really helpful for placing and alignment. (one column)
justify-* is row axis
align-* is column axis

Unlike flexbox they don't flip.

## 18 Ordering
Default order is zero. Order will mess with a11y or text selection.

## 19 Nesting Grid
Grid item can also be a grid container.
The grid is bound by resizing the browser.

By using auto-fit and minmax it's behaves a bit like container queries.