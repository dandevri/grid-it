## 03 - Grid Fundamentals
Take any element on the page and you are going to display grid it.
You can slice and dice the container. Then we can place the items on the grid.

The columns and rows are called tracks. So no need to position.
When you display grid a container you make all of its direct children items.

Rows are automatically created if you only do columns.
Fractions will replace the need for percentages.

## 04 - Grid Dev Tools
Grid is pretty hard to visualize. They are not elements themselves.
Tracks are not numbered by the rows and columns but by the lines they start and stop them.

Solid line = explicit grid edge
Dashed = explicit
Dotted = implicit

## 05 - Implicit vs Explicit
If you do not create them, they are implicit.
Solid line explicit grids starts and stops.
By default you define your columns and then any extra elements wil lbe turned into rows.
Automatically columns instead of rows is auto-flow.

## 06 - Grid Autoflow
Autoflow will determine if you need another row or column.
Row is default.

## 07 - Sizing
Percentages won't really work, because them grid gap is counted with them.
Fr = fractional unit. Amount of space left if all of them are lay-out.
If you use px you won't really use all of the available grid space.
Fr is a bit like flex grow.
Height of the grid is just the height of the content. Width is the viewport.
Auto = content.

## 08 - Repeat
Alternate.

## 09 - Sizing Items
fr = free space 
Spanning; explicitly tell some items to span multiple columns.
More on how large and small an item should be, not how it should place itself.

## 10 - Placing items
Grid-column is actually a short hand.

## 11 - Spanning and Placing cardio
-

## 12 - auto-fit and auto-fill
You don't tell auto-fill how many columns you want, just say figure it out.
auto-fit: explicit grids stops at the items.

## 13 - Minmax
combination of auto-fill and minmax can replace a lot of media queries.

## 14 - Grid Template Areas
Visual ascii kind of lay-out.

## 15 - Naming Lines
Name track lines with square brackets.

## 16 - Auto Flow
6 spots needed but only 5 left? Grid will layout with a gap. It doesn't really fit these spots.

## 17 - Grid Alignment
justify-* is row axis
align-* is column axis

Container is wider then it should be, you can use justify content.

Sctretch is default.

align-self on a case by case basis. Only for one specific item.
No justify-self in flexbox.

## 18 - Re ordering
Default order of everything is 0.
Screen reader mixes this up. Selection won't work properly.

## 19 - Nesting
With CSS grid you will have less wrapper components.
Grid item can also be container.

## 20 - Image Gallery
