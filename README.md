# geodata


## Creating a combined map in QGIS
To create a combined map, we cannot simply merge the two maps.

NJ and NYC have different data ranges, so we need to account for that.
Below are the steps taken to create the merged map.
- For each map, use raster statistics to find the min and max.
- Create a new raster calculation that is a percentage using the equation
    (x - min) / (max - min)
    The above finds the percentage in the interval
-
