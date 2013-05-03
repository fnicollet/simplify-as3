simplify-as3
============

simplify-as3 is a simple port of simplify.js by Vladimir Agafonkin (https://github.com/mourner/simplify-js)

### Usage
```
import flash.geom.Point;
import simplify.Simplify;

var points:Vector.<Point> = ...;
var tolerance:Number = 10;
var highQuality:Boolean = false;
var simplified:Vector.<Point> = Simplify.simplify(points, tolerance, highQuality);
```

points: An Vector of Points. If you have an Array, use Vector.<Point>(someArray)

tolerance (optional, 1 by default): Affects the amount of simplification that occurs (the smaller, the less simplification).

highestQuality (optional, false by default): Flag to exclude the distance pre-processing. Produces higher quality results, but runs slower.
