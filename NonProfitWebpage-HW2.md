## Homework 2: Build and Deploy a Custom Map
Advanced GIS Portfolio (90-753)

Client: Saga Education

Consultant: Caroline Sabin

---
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

The initial bid for work, including the cost and scheduling for both phases, can be found at this link: [Bid for Saga Education Mapping Project](https://docs.google.com/document/d/1kxcpC-cjW_rXK1ZVuWrZLn_x9894iQ-yK11TED__hZY/edit?usp=sharing)

---
### Phase 1: Customize the Map Style

#### Color Palette
First, I used the Adobe Color tool to extract five colors from the Saga Education logo, which would become the color palette I will use to align the custom map to the non-profit's brand. The color pallete from Saga Education's branded image is provided here: ![Saga Education: Color Palette](https://github.com/c-sabin/AdvancedGIS_Portfolio/blob/main/Saga%20Color%20Palette.png)


#### Style Look-up Table
After creating the custom color palette, I entered Google Styling Wizard and began customizing various map elements. The style elements that were changed are listed in the look-up table below.

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
When input into the Styling Wizard, these custom elements produced a code chunk that can be utilized to replicate this style. You can download the JSON file containing the custom map style here: [Saga Education: Style Elements JSON](https://raw.githubusercontent.com/c-sabin/AdvancedGIS_Portfolio/main/saga_mapstyle.txt). 


#### Examples
The following screenshots show examples of the custom map style that was produced for this assignment. The examples represent three different Zoom levels, focusing on Chicago——where Saga Education does considerable business. 

This first screenshot shows the custom map when zoomed out to focus on the Eastern United States. The focus on the east coast was chosen because six of the seven Saga Education sites are located east of the Mississippi River. At this zoom extent, only the red major highways and the navy blue water features are visible.
![Zoom level 1](https://github.com/c-sabin/AdvancedGIS_Portfolio/blob/main/NonProfit-Zoom1HW2.png)

The second screenshot represents the same map, zoomed in to highlight Massachusetts——in which Saga Education's headquarters are located. At this zoom extent, we can start to see the green park areas and smaller, salmon-colored roadways popping up on the visualization.
![Zoom level 2](https://github.com/c-sabin/AdvancedGIS_Portfolio/blob/main/NonProfit-Zoom2HW2.png)

The final screenshot in this series is zoomed in even further, to Boston and the surrounding area. The white marker toward the left of this image was chosen to pinpoint the Saga Education HQ in Newton, Massachusetts. At this closer zoom extent, we can now see other points of interest (colored green, teal, and red), as well as more detailed roadways.
![Zoom level 3](https://github.com/c-sabin/AdvancedGIS_Portfolio/blob/main/NonProfit-Zoom3HW2.png)


---
### Phase 2: Embed an Interactive Map

#### Interactive Map
As the first step in phase two, I established an API through Google's Cloud Platform. This allowed me to embed the custom map on a website that the client could further customize to meet their needs. The deployed interactive map can be found at the following site: [Saga Education: Interactive Map](https://c-sabin.github.io/AdvancedGIS_Portfolio/NonProfitCustomMap-HW2). 

#### Points of Interest
In addition to producing the interactive map, I added some of the organization's site locations to this map as point "markers." The points of interest I defined include: 

 + six school districts being serviced
   + Boward County, FL
   + Charleston, SC
   + Chicago, IL
   + New York, NY
   + Providence, RI
   + Washington D.C.
 + organization headquarters: Newton, MA

I utilized Google's MyMaps tool to define these seven points of interest. In addition to defining this point layer, I also customized the icons for each point to be the Saga Education "S" logo. The MyMaps layer containing these point locations can be found here: [Saga Education: Points of Interest](https://www.google.com/maps/d/u/0/edit?mid=1X2hB3TZvF2OSGv880pW4cle3VC8jWoI&hl=en&ll=39.36197068746295%2C-79.42597774999999&z=5). A KML version of this map layer can also be downloaded at this link: [Saga Education: Points of Interest KML](https://raw.githubusercontent.com/c-sabin/AdvancedGIS_Portfolio/main/NonProfitPoints-HW2.kml).
