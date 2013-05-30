# force-geojson

[![Dependency Status](https://gemnasium.com/tmcw/force-geojson.png)](https://gemnasium.com/tmcw/force-geojson)

[![](http://api.tiles.mapbox.com/v3/tmcw.miserables/0,0,2/400x300.png)](http://a.tiles.mapbox.com/v3/tmcw.miserables/page.html#1.00/0/20)

Marrying [d3js](http://d3js.org/)'s [force directed graph implementation](http://bl.ocks.org/mbostock/4062045)
with [GeoJSON](http://www.geojson.org/) so you can abuse map-making tools
like [TileMill](http://www.mapbox.com/tilemill/) to make big big force directed
graphs.

    npm install -g force-geojson

    force-geojson foo.json > foo.geojson

The input needs to be formatted like d3 wants it to be: [read the docs](https://github.com/mbostock/d3/wiki/Force-Layout).

Takes a few options:

* `times`: how many iterations to work on the graph position
* `padx`: how close points can get to -180 and 180 longitude
* `pady`: how close points can get to -90 and 90 latitude
