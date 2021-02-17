# Google Earth Engine: Drawing Polygons

This document will teach you how to:
1. Open a new script
2. Set the map center
3. Draw a polygon

## Google Earth Engine

First, go to [**Google Earth Engine**](https://code.earthengine.google.com/). 

Make sure you first [sign up](earthengine.google.com) for a Google Earth Engine account. You cannot use Google Earth Engine unless your application has been approved and this can take several days to a week. Once you receive the application approval email, you can log in to the Earth Engine Code Editor.

## New Script

Click the red button in the top left corner that says **NEW**. 

![](https://i.imgur.com/FDKJDCd.png)

## Set Map Center

In this example we're looking at the US, so type:

`Map.setCenter(-105.9, 39.0, 5);`

## Draw Polygons

Now click the polygon tool at the top left of the map view. Try to trace the outline of a nice square state, e.g.
* Colorado
* Wyoming
* North Dakota
When you finish tracing your state, click back on the first point to finish creating your geometry import. Now you'll see a box pop up with the geometry you just drew.

![](https://i.imgur.com/Cgc9hVC.png)

Select the settings option (the little gear) and name your shape whatever you'd like, e.g. **Colorado**. You can also change the color.


## Create your script.

Now you have empty script with one import. Type:

`var feature0 = ee.Feature(Colorado, {'name': 'Colorado'});`
`Map.addLayer(feature0, {'color': '0000FF'});`

Now save your script. 

## Print to Console

Enter: 

`print(feature0);`

to see the features in the console, where you can investigate the geometry and properties. 

## That's it!

Double check that you've saved your script and you can close the window. Now whenever you want to draw some polygons, they'll already be loaded and ready for you.
For more helpful tips on getting started with **Google Earth Engine** check out Dr. 

<a href="https://www.youtube.com/watch?v=_4o6sbOu5do&ab_channel=QiushengWu" target="_blank">
<img src="https://www.youtube.com/watch?v=_4o6sbOu5do&ab_channel=QiushengWu/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>
