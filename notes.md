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