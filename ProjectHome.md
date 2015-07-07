The [Israeli Transverse Mercator](http://en.wikipedia.org/wiki/Israeli_Transverse_Mercator) (ITM) is the common coordinate system used in Israel by hikers and scientists.  The conversion between ITM and the [World Geodic System](http://en.wikipedia.org/wiki/WGS84) angular coordinates (used by GPS) is not trivial and requires some advanced math.

JS-ITM is a simple Javascript library to convert between those two coordinate systems.

Please note that the conversion is NOT accurate and may include ~10m errors (So don't design your skyscrapers, particle accelerators etc. using this library.)

Quick Start:
```
<script type="text/javascript" src="js-itm.js"></script>
<script>
  alert(JSITM.itmRef2gpsRef("222631"));
  alert(JSITM.gpsRef2itmRef("31.77805 35.23559"));
</script>
```


A simple example is available [here](http://static.peace-love-freedom.net/js-itm/trunk/examples/js-itm-example-1.html).

Documentation:  http://static.peace-love-freedom.net/js-itm/trunk/jsdoc/index.html


---


  * **2008-12-07**: Yey!  The library is now online.  Let's say this is beta - bug reports welcome.  Some more docs to come (lots of jsdoc is already inside).


---


  * This project is a fork of the [GeoTools WGS84/OSGB36 converter](http://www.nearby.org.uk/tests/GeoTools2.html), a free library to convert GB/Irish coordinates.
  * Grid parameters source is EPSG 2039: http://spatialreference.org/ref/epsg/2039/



