# After Effects Expression Library

I'm using this repo as a place to store expression snippits that I think are worth saving for later. 

Right now, I'm storing them in markdown files in the [expressions folder](https://github.com/CameronFoxly/AfterEffectsExpressionLibrary/tree/main/expressions) in this repo, but might get around to doing more organizing at some point.


## Index of Expressions

- [Position for Grid Layout](https://github.com/CameronFoxly/AfterEffectsExpressionLibrary/blob/main/expressions/grid-layout.md) - A position expression that can be used to layout a bunch of objects into a grid with spacing controlled by a single slider. 
- [Sample Layermap Brightness](https://github.com/CameronFoxly/AfterEffectsExpressionLibrary/blob/main/expressions/Sample-LayerMap-Luma.md) - Best if used with Grid Layout, this expression samples the luma value of a given layer and uses that value to drive whatever property you apply it to. Basically, it's a custom layer map system like in Trapcode's form. 
- [Global position of parented layer](https://github.com/CameronFoxly/AfterEffectsExpressionLibrary/blob/main/expressions/global-parented-position.md) - Quick little expression for how to get the global [x,y] position value of a layer that is parented to another layer.
- [Respecting Aspect Ratio](https://github.com/CameronFoxly/AfterEffectsExpressionLibrary/blob/main/expressions/respecting-aspect-ratio.md) - Returns a Y value based on an X value that maintains a ratio of X:Y that matches the compositions aspect ratio. Great for the mosiac plugin for getting square "pixels"
- [2d LookAt](https://github.com/CameronFoxly/AfterEffectsExpressionLibrary/blob/main/expressions/2d-lookAt.md) - Effects the rotation of a layer so that it "looks at" another layer in 2D. 
