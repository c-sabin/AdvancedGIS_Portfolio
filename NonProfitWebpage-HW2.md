## Homework 2: Build and Deploy a Custom Map
Advanced GIS Portfolio (90-753)
Client: Saga Education

### Phase 1: Customize the Map Style

First, I used the Adobe Color tool to extract five colors from the Saga Education logo, which would become the color palette I will use to align the custom map to the non-profit's brand. The color pallete from Saga Education's branded image is provided here: 
![Saga Education color palette](https://github.com/c-sabin/AdvancedGIS_Portfolio/blob/main/Saga%20Color%20Palette.png)\

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



