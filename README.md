Welcome!

If you are reading this page you were likely directed here from the CBC count circle app and you are hoping to add your count circle to the map. Thats great!

First things first lets talk about the app. This application has flask (python) on the back end serving up GeoJSON files. You must be comfortable making these files. If your count circle has a GIS specialist/analyst they will be more than competent to make such a digitalization. GeoJSON is a little bit strange for some people to make, if your GIS person hasn't worked with them before thats totally ok - we can work that detail out.

The application runs on NoSQL principles. That means that your count circle doesn't really need to match the schemas of the other count circles shown here. With two big exceptions, my application is looking for a 'name' column and a 'desc' column. THESE ARE REQUIRED. In the name column there must be a simple <5 character code. In the case of Oakland you will see they used (primarily) 3 letter codes. In the case of San Francisco they used numbers. In the desc column is the description of the area, it is here you can put a longer name - but not your life story here, lets keep it short (<25 characters).

The digitized boundaries between your count areas must not have gaps or overlaps. This is called topogology. Your GIS person will know what I mean.

Your count areas should be only one polygon per area. It may be really tempting to lump an island in with the 'shore' team, but it is not best practice in this situation to have multiple polygons attributed to one area. It can be done, but try to avoid this when possible. Also when possible do not make count areas with a low compactness. Imagine a large C shaped area surrounding a smaller area. This also is not best practice, but in some situations can be done - please try to avoid this.

Count circles must be 15 miles in diameter. This is an easy calculation to make, don't mess it up by using the wrong projection.

The count circle should be slightly simplified, that is to say not a 100% perfect circle, more like a hexagon but with more sides. Not having to load the extra verticies helps loading time. Take a look at the SF CBC count circle above. I don't remember how many sides I put on that, but zoom in and check it out. Aim for something roughly like that.

Your resulting file MUST be one file, please do not break your polygons into multiple files.

Please use the files above as guides, feel free to download them and look at how they were made. Contact me with any questions you might have. Thanks and happy birding!
