## Information Visualization (GapMinder) : Channelling Hans!

Content
-----------------------------
1. Steps to run project
2. Documentation
	- Recreated Features
	- Extra Features Included
4. References


Steps to run project:
------------

**Step 1:** Clone the Project or Download the project
- To Clone Project:
``` 
git clone git@gitlab.com:akshat.rastogi/gapminder-d3js.git
```

- Download using this [link](https://gitlab.com/akshat.rastogi/gapminder-d3js.git)


**Step 2:** Goto the directory and start localhost server to avoid cross origin error
Example: To start python server:
```
python -m http.server
```

**Step 3:** View the page using the following link
```
http://localhost:8000/chanelling-hans.html
```
Note: The port number may change, check wherever your server is running 

Documentation
------------

* Recreated Features:
-----------------------------
1. Bar chart representing the number of countries per region.
2. Bar chart representing the number of countries with each government type.
3. The selection of a specific country from the provided drop-down list, gives a static visualization depicting the trace of motion of the bubble representing that country.
	- When a viewer uses this control, the remaining controls to jump to the visualization of a specific year and the Play/Pause/Stop buttons would be disabled.
	- The viewer must select the default value “All Countries” from the drop-down list explicitly, to re-enable all the disabled controls.
NOTE:
	- Both bar charts would be displayed to the right of the Gapminder World visualization.


* Extra Features Included:
-------------------------
1. Apart from the bar charts in Mandatory Features (1) & (2), a third bar chart depicting the number of kilometres of Coastline per region.
	- A control using checkboxes is provided, to select any two bar graphs that the user wishes to display along with the GapMinder World visualization.
	- At a time, only two bar charts can be selected by the user and both would be displayed to the right of the Gapminder World visualization.
	- By default, the checkboxes corresponding to the first (number of countries per region) and the second (number of countries with each government type) bar charts would be checked and they would be displayed.
	- Bar Chart 1 and 3 when viewed together, would provide the best insights regarding the changes over the years.

2. In addition to the Mandatory Feature (3), a provision for the users to compare the traces of two different countries is also provided.
	- Once the user selects a country in the first drop-down box to view its trace, the static trace for that country would be displayed in the visualization. At the same time, a second drop-down box would be enabled.
	- The user can select a different country from this list, which would display the trace of the selected country as well in the visualization.
	- The simultaneous display of the traces of two countries can be used for certain comparisons between them.
	- The user finally has to explicitly click the “Reset” button, to get all the other controls enabled.

3. Upon the event of a mouse hover over a particular bubble, the following changes can be seen in the visualization:
	- Only the desired bubble would be highlighted, and the rest of the bubbles would be hidden (opacity reduces).
	- A tooltip window describing the Country, Year, GDP, Life Expectancy and Population data corresponding to that bubble, appears.
	- The animation would be auto-paused. The user would have to explicitly use the play button to resume the animation.

4. A panel consisting of the Play, Pause and Stop buttons to control the animations in the visualization, is provided.
	- The Play button facilitates the animation to be played continuously.
	- The Pause button is to pause the animation explicitly, in case the user wishes to view data in a static form or choose a different bar graph.
	- The Stop button is to stop the animation and the next time the Play button is pressed, the animation starts from the beginning (from the earliest year in the data).


References:
------------
>[1] https://jsfiddle.net/umaar/FV5tm/

>[2] https://www.w3schools.com/howto/howto_js_rangeslider.asp

>[3] https://bl.ocks.org/
