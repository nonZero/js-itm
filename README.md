The [Israeli Transverse Mercator](http://en.wikipedia.org/wiki/Israeli_Transverse_Mercator) (ITM) 
is the common coordinate system used in Israel by hikers and scientists.  
The conversion between ITM and the [World Geodic System](http://en.wikipedia.org/wiki/WGS84)
angular coordinates (used by GPS) is not trivial and requires some advanced math.

JS-ITM is a simple Javascript library to convert between those two coordinate systems.

Please note that the conversion is NOT accurate and may include ~10m errors 
(So don't design your skyscrapers, particle accelerators etc. using this library.)

###Quick Start:

In the browser:
```html
<script type="text/javascript" src="js-itm.js"></script>
<script>
  alert(JSITM.itmRef2gpsRef("222631"));
  alert(JSITM.gpsRef2itmRef("31.77805 35.23559"));
</script>
```

With npm:
`npm install js-itm --save`


And then in the code:
```javascript
var JSITM = require('js-itm');`
```

----
 * *2015-07-07*: This is an old piece of software auto exported from Google code. 
   You should probably want to use something else instead of this, probably [Proj4js](http://proj4js.org/).
 * *2008-12-07*: Beta.

----

 * This project is a fork of the [GeoTools WGS84/OSGB36 converter](http://www.nearby.org.uk/tests/GeoTools2.html),
   a free library to convert GB/Irish coordinates.
 * Grid parameters source is EPSG 2039: http://spatialreference.org/ref/epsg/2039/
