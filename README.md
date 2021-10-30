# breadcrumb-plus-osm
multiple tracks (&lt;trk> s) in GPX track file example  


You can download the powell_butte.gpx file containing several tracks.

Download and install the free GPXSee app. Drag the gpx file over the GPXSee app window and you will see that it correctly displays distinct tracks. <https://github.com/tumic0/GPXSee>

This is not what happens, for example, when loading the same as a path in the COROS app for use with their APEX watch. Discontiguous tracks get connected as if they were one, and falsely show line connecting them. I hope that this can change in the future. That is the point of this repo.

If I add a feature to select a subset of OSM lines to include in a GPX file it will most likely have gaps. The magic of merely connecting them with lines on your screen is a safety issue, because there is no path there at all.

The example gpx file is an output from my offline hiking app PDXWalk (from emulator). It is a track, then a set of nearby OSM lines. Below is an outline of what a gpx file might contain in the future. You can watch my first test of screen recording from my app (<https://twitter.com/LostRat/status/1440886097400061953?s=20>).  If I output just some close OSM paths there will most likely be discontiguous path segments, and others that intersect. I want to show them all and accurately note discontiguous parts.

event tracks

- from others
- OSM snappables
- your own

event waypoints

- from others
- OSM
- your own

event approach (roads to/from)

- from others
- OSM snappables
- your own

array of OSM snappables

- OSM Whole
- OSM Part (with start stop points for segment)

array of OSM nearby

- OSM Whole
