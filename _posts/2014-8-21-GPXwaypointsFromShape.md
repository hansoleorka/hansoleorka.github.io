---
layout: post
title: Convert point shapefile to GPX waypoints for use in Garmin GPS
---

The easiest way or atleast one way to this is with [QGIS](http://www.qgis.org/).

###Step 1
Open QGIS

###Step 2
Edit the table so that it have the three columns name, cmt, and desc. The name column will be the waypoint id, the two other columns are comments (cmt) and description desc). I have to check which one that is most important.

You can create a string description of multiple columns like this:


![an image alt text]({{ site.baseurl }}/images/2014-08-20/image001.png "an image title")


Thus the table with the three default columns:


![_config.yml5]({{ site.baseurl }}/images/2014-08-20/image003.png)

###Step 3

The export to GPX using the Layer menu and Save as. Remember to set the coordinate system of the GPS (Check if important, maybe a geograpichal system is needed??). In the Save vector layer as dialog box set CRS=Selected CRS og Browse to the correct system (eg. WGS84 -  ESPG:4326).


![_config.yml2]({{ site.baseurl }}/images/2014-08-20/image005.png)

The GPX file should den look like this if opened in a text editor:

![_config.yml4]({{ site.baseurl }}/images/2014-08-20/image007.png)

