This expression can be used to lay out a grid of objects.
Apply it to the position property of whatever object you want place into a grid, before duplicating enough of them enough for the grid.
You'll also want to create a null called "CONTROLLER" and add a slider called "padding" and pickwhip it in line 1 to control the grid's spacing. 

```
padding = {pickwhip to slider on a null controller layer};     
numberOfColumns = Math.ceil(thisComp.width / padding)+1;

xValue = padding * ((index-1) % numberOfColumns);
yValue = padding * Math.floor((index-1) / numberOfColumns);

[value[0]+xValue, value[1] + yValue];
```
