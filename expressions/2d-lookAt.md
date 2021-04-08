This expression, applied to the rotation value of a layer, forces that layer to point at a target layer. 

```
targetLayer = {pickwhip this to the layer you want to look at};

xDistance = targetLayer.transform.position[0] - transform.position[0];
yDistance = targetLayer.transform.position[1] - transform.position[1];

radians = Math.atan2(yDistance, xDistance);

radiansToDegrees(radians);
```
