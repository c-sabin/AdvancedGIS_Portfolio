## Homework 3: Mapping the DEA's Pain Pill Data with ArcGIS Insights
Advanced GIS Portfolio (90-753)

---
### The Data
The United States' Drug Enforcement Administration (DEA) has a comprehensive database monitoring the nationwide flow of pain pills between manufacturers, distributors, and pharmacies. This database contains the distributor's origin addresses (*REPORTER_ADDRESS*) as well as the destination pharmacy's address (*BUYER_ADDRESS*), which enables analysts to link the distributors to pharmacies for each pain pill sold in the United States. Specifically, the data focuses on oxycodone and hydrocodone pills that travelled across the U.S. between 2006 and 2014. 

Recently, the Washington Post published an article whereby they analyze "nearly 500 million transactions" within this time period. Access to the article and the DEA database can be found here: [Washington Post's analysis of the DEA pain pill database](https://www.washingtonpost.com/graphics/2019/investigations/dea-pain-pill-database/).

#### Mingo County, West Virginia
For this assignment, I will be focusing on Mingo County, West Virginia. This focus comes from the unusually high amount of rates of perscriptions delivered to the pharmacies in this county, given the relatively small population of the area. According to the Washington Post's analysis, the immense flow of prescription pills into Mingo County averages out to *each county resident* buying about 180 pills per year. 

To further analyze this flow of pain pills within Mingo County, I used **ArcGIS Insights**. The resulting analysis can be found below:
<iframe src="https://insights.arcgis.com/#/embed/fcb66ae589ec4d9f80b5db6acc4f5fbc" width="970" height="100%" frameborder="0"></iframe>


### Insights
*What did you learn from working with these data and performing this analysis?*

#### Pain Pills in West Virginia
It is incredibly alarming that there are so many pain pills circulating among a relatively small population. Given that these medications -–hydrocodone and oxycodone——are Schedule II controlled substances, pharmacies should require perscriptions in order to sell to consumers. This makes me wonder if rather than a consumption problem, this signals to an issue of over-perscription by doctors of these schedule two drugs. 

On the consumption side though, I wonder what kind of "black market" there is for these drugs in West Virginia——and Mingo County specifically. I find it hard to believe that each resident in the county is consuming 180 of these pills per year on their own; presumably, consumption of these pills is higher among a smaller population of individuals. If this were true, I could imagine that one individual doesn't use all of the pills they are prescribed——in which case, I could see a situation in which the holders of these prescriptions sell their "extra" pills in an informal drug market. Either way——whether individuals use all of these pills themselves, or sell them in illegal markets——it seems like there is a wider-spread substance abuse problem. 

Given the nationwide flows of pain pills, I also wonder what role policy plays in regulating the potential over-prescription and/or over-consumption of these drugs. I found it interesting that there is only one large distributor, Cardinal Health, within the state of West Virginia. Perhaps the states acting as the sources of these drug flows into West Virginia——namely, Virginia, Ohio and Kentucky——have different regulatory environments around substance II drugs. Seeing as how these states are contiguous to West Virginia, it is possible that those WV customers with a demand for these pills bypass their own state's regulatory system by seeking perscriptions in surrounding states. I would be interested to look further at the regulations surrounding the distribution of schedule II drugs in each of these states to further investigate these interstate flows. 

#### ArcGIS Insights
I really appreciated how easy it was to construct maps using the ArcGIS Insights platform. I thought the card interface, which mirrors the display of Tableau, was really easy to use and understand. I also found the Action Button incredibly helpufl for conducting additional analyses with the data. The options under this prompted me to think about new exploratory questions that I hadn't previously considered, which added to my understanding of the data.

As much as I liked how easy it was to create a basic dashboard with the standard analytic features, I found it a bit harder to do the same level of customization that ArcGIS Pro offers. I don't think there were as many opportunities for customizing the symbology and overall layout of different cards through the **Appearance** tab as there are with ArcGIS Layouts. That said, ArcGIS Insights was much more user-friendly, as the Layouts in ArcGIS Pro tend to be much more finnicky and time consuming. Overall, I would make the tradeoff of fewer customization options in favor of ease-of-use.
