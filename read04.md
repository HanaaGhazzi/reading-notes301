# CSS Grid 
_is a powerful tool that allows for two-dimensional layouts to be created on the web. This guide was created as a resource to help you better understand and learn Grid, and was organized in a way I thought made the most sense when learning it._

![grid](https://miro.medium.com/max/871/1*kI78qZQjw_ax1kJo4lPOcw.png)


### Grid Container

**Create a grid container by setting the display property with a value of grid or inline-grid. All direct children of grid containers become grid items.**

- display: grid
Grid items are placed in rows by default and span the full width of the grid container

- display: inline-grid 
 generates an inline-level grid 

 ### Explicit Grid

**Explicitly set a grid by creating columns and rows with the grid-template-columns and grid-template-rows properties.**

- grid-template-rows: 50px 100px : A row track is created for each value specified for grid-template-rows. Track size values can be any non-negative, length value (px, %, em, etc.)


- grid-template-columns: 90px 50px 120px: Like rows, a column track is created for each value specified for grid-template-columns.

Items 4, 5 and 6 were placed on a new row track because only 3 column track sizes were defined; and because they were placed in column tracks 1, 2 and 3, their column sizes are equal to items 1, 2 and 3.

- grid-template-columns: 1fr 1fr 2fr: The fr unit helps create flexible grid tracks. It represents a fraction of the available space in the grid container (works like Flexbox’s unitless values). 

- grid-template-columns: 3rem 25% 1fr 2fr
fr is calculated based on the remaining space when combined with other length values.

### Repeating Grid Tracks

**Define repeating grid tracks using the repeat() notation. This is useful for grids with items with equal sizes or many items.**

- grid-template-rows:    repeat(4, 100px);
- grid-template-columns: repeat(3, 1fr);

__The repeat() notation accepts 2 arguments: the first represents the number of times the defined tracks should repeat, and the second is the track definition.__

### Grid Gaps (Gutters)

**The grid-column-gap and grid-row-gap properties create gutters between columns and rows.**

_Grid gaps are only created in between columns and rows, and not along the edge of the grid container ._