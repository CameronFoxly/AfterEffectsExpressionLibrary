Thank you Dan Ebbert, for this useful little expression for returning the global position of a parented layer. I use this all the time.
If you need to get the compoisition [x, y] value of a layer that is parented to another layer, use this expression, but replace "Null 1" with the target layer.

```
L = thisComp.layer("Null 1");
L.toWorld(L.anchorPoint)
```
