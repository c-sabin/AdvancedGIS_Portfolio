## Homework 2: Build and Deploy a Custom Map
Advanced GIS Portfolio (90-753)
Client: Saga Education


### Project Plan

This project is an effort to build and deploy a customized map consistent with the branding of our client, [Saga Education](https://www.sagaeducation.org/about-saga-education/). There will be two phases of work in order to complete this project: the first phase will involve customizing the map style, and the second phase will represent the deployment of an interactive map.

The following deliverables are included in this project: 

    **Phase One**
    + look-up table for style elements
    + JSON file containing style code 
    + webpage demonstration 
    + documentation on using provided materials

    **Phase Two**
    + interactive map embedded on webpage
    + KML file with point locations

### Phase 1: Customize the Map Style

First, I used the Adobe Color tool to extract five colors from the Saga Education logo, which would become the color palette I will use to align the custom map to the non-profit's brand. The color pallete from Saga Education's branded image is provided here: ![Saga Education color palette](https://github.com/c-sabin/AdvancedGIS_Portfolio/blob/main/Saga%20Color%20Palette.png)


#### Style Look-up Table
After creating the custom color palette, I entered [Google Styling Wizard](https://mapstyle.withgoogle.com/) and began customizing various map elements. The style elements that were changed are listed in the look-up table below.

| Feature type | Element type | Stylers |
| -------------| -------------| --------| 
| All	| Geometry | Fill	Color: #f5f5f5
| All	| Labels / Text fill | Color: #616161
| All	| Labels / Text outline	| Color: #f5f5f5
| Administrative / Country | Geometry / Stroke | Color: #000000
| Administrative / Neighborhood	| Labels	| Visibility: Hidden
| Points of interest	| Geometry / Fill	| Color: #23d9c7, Lightness: 20
| Points of Interest / Medical	| Geometry / Fill	| Color: #F25764, Lightness: 20
| Points of Interest / Park	| Geometry / Fill	| Color: #7AD94E, Lightness: 20
| Points of Interest / Park	| Labels	| Visibility: Hidden
| Road	| Geometry / Fill	| Color: #F29984, Weight: 0.5
| Road / Highway	| Geometry / Fill	| Color: #F25764, Weight: 1, Visibility: Shown
| Road / Arterial	| Geometry / Fill | Color: #F29985, Weight: 0.5
| Road / Local	| Geometry / Fill	| Color: #F29985, Weight: 0.5
| Road / Arterial |	Labels	| Visibility: Hidden
| Road / Local	| Labels	| Visibility: Hidden
| Transit	| Geometry	| Color: #E5E5E5
| Water	| Geometry	| Color: #012840
| Water	Labels |  Text fill	| Color: #FFFFFF


#### Map Style JSON File
When input into the Styling Wizard, these custom elements produced a code chunk that can be utilized to replicate this style. You can download the JSON file containing the custom map style here: [Saga Education map style JSON](https://github.com/c-sabin/AdvancedGIS_Portfolio/blob/main/saga_mapstyle.txt). 


#### Examples
The following screenshots show examples of the custom map style that was produced for this assignment. The examples represent three different Zoom levels, focusing on Chicago——where Saga Education does considerable business. 

This first screenshot shows the custom map when zoomed out to focus on the Eastern United States. The focus on the east coast was chosen because six of the seven Saga Education sites are located east of the Mississippi River. At this zoom extent, only the <span style="color: #F25764"> major highways </span> and the <span style="color: #012840"> water features </span> are visible.
![Zoom level 1](https://github.com/c-sabin/AdvancedGIS_Portfolio/blob/main/NonProfit-Zoom1HW2.png)

The second screenshot represents the same map, zoomed in to highlight Massachussets. At this extent, we can start to see the park areas and smaller, arterial roads popping up on the visualization.
![Zoom level 2](https://github.com/c-sabin/AdvancedGIS_Portfolio/blob/main/NonProfit-Zoom2HW2.png)

The final screenshot in this series is zoomed in even further, to Boston and the surround area——in which the Saga Education is headquartered.
![Zoom level 3](https://github.com/c-sabin/AdvancedGIS_Portfolio/blob/main/NonProfit-Zoom3HW2.png)


### Phase 2: Embed an Interactive Map

