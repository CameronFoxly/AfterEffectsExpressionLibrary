This expression uses the luma value of a layer to drive a return value to be used elsewhere. The layermap is sampled at the position of the layer you've applied this expression to.
Best if applied to a [grid of other objects](https://github.com/CameronFoxly/AfterEffectsExpressionLibrary/blob/main/expressions/grid-layout.txt), but could probably be used elsewhere. 
You should add three slider controls to your target layer: **sampleSize, minValue and maxValue**.
- **sampleSize** dictates the size of the sample at the given point. 
- **min** and maxValue set the low and high value that you want to map to the layer your adding the expression to.

```
layerMap = thisComp.layer("LayerMap");   //link this value to the layer you want to sample.
sampleSize = layerMap.effect("sampleSize")("Slider");
minValue = layerMap.effect("MinValue")("Slider");
maxValue = layerMap.effect("MaxValue")("Slider");

sampleValue = layerMap.sampleImage(transform.position, [sampleSize, sampleSize], true, time);

HSLValue = rgbToHsl(sampleValue);

brightness = HSLValue[2];

returnValue = linear(brightness, 0, 1, minValue, maxValue);

returnValue;
```
