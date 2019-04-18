
# Overview
This package is designed to provide filters for working with laser scans.

There are a number of filters that this class provides.  There is also
a factory class to provide easy creation and chaining of laser scan
filters as a input to any process.

A filter made with this software will read in data from the `/scan` message, and will output filtered data on the `/scan_filtered` message.

In order to create a custom filter, please follow the instructions on the wiki: http://wiki.ros.org/laser_filters

#Angular Bounds Filter 

The Angular Bounds Filter has been created in order to ignore laser scans outside of a certain field of view. The bounds of the obstruction can be set with `lower_angle` and `upper_angle`


In order to run the filter, please use this commmand:
```
roslaunch laser_filters angularBoundsFilter.launch
```

#Angular Bounds Filter In Place

The Angular Bounds Filter has been created in order to ignore laser scans within a certain subset of the field of view. The bounds of the obstruction can be set with `lower_angle` and `upper_angle`


In order to run the filter, please use this commmand:
```
roslaunch laser_filters angularBoundsFilterInPlace.launch
```

