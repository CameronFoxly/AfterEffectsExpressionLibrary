This expression keeps x and y values in the same aspect ratio of the composition.
This is great for things like the mosiac filter, when you want square "pixels." 
You apply this expression to the Y value, and pickwhip the xValue.

```
xValue = {pickwhip this value to the x value};

(xValue*thisComp.height)/thisComp.width
```
