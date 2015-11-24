Assignment: Programming Assignment Extension UC San Diego/Coursera MOOC
=======================================================================
I added some features, supported by a GUI which emulates option and check controls. These controls allow to select which earthquakes are visible regarding **age** (from "Past day" to "Past month"), **magnitude** (all visible, Top 10 strongest, Top 100 strongest), and also working with the following preferences: **"Show cities"** (show/hide cities on the map), **"Highlight quakes"** (add/remove an X for recent quakes), **"Ocean threat lines"** (show/hide lines for an ocean quake affecting cities within its threat circle), **"Show threat circle"** (show/hide a circle indicating the threat area affected by the quake selected, which is only valid for small threat radius\*), and **"Show coordinates"** (show/hide geographic coordinates for any position pointed by the mouse cursor).

(\*) *Drawing a good approximation of the threat area for any radius is not straightforward at all!!! I use the bisection method (analogous to binary search) to calculate the diameter in pixels for the circle, but I realized the real shape is not a circle. I do not know how a threat area should look, but I figured out some way to implement this, by using numerical methods. I do not have enough time to solve it, since the deadline is tomorrow, but it is a challenge that I will be confronting in the next days... At the end, for relatively small areas, the shape should look similar to a circle as I noticed by the getDistance method behavior (see* **Quakes.jpg - figure 2***).*