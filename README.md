
# Medicare Charge Data 

## Summary

* The medicare charge data for around 3000 hospitals has been released by Center for Medicare and Medicaid Services since 2011. Till 2013, only the top 100 _DRG(Diagnosis Related Group)_ for every hospital were released. However, from 2014 onwards, the center has started releasing data related to all DRG. More info about the data can be found [here](https://www.cms.gov/Research-Statistics-Data-and-Systems/Statistics-Trends-and-Reports/Medicare-Provider-Charge-Data/index.html)
* The main idea of the visualization is to convey a story that the hospital charges vary widely across the country. In order to show this finding, we display the average medicare cost for each
state on the map of the Unites States. 
* Next, we present the average medicare cost for each of the hospitals listed in the database. This data visualization displays a comparison of the average medicare cost charged by the hospitals against the national and state averages. There are two levels on which the above comparison can be made. First, on the overall medicare cost and the second on the basis of individual DRG.

## Design

### Original Choices

#### Text

* Small introductory paragraph was written at the top of the page to introduce the graphic.
* Explanations were added in the tooltip.

#### Visualization

* Since the data is quantitative and I wanted to show a comparison of each DRG with the national average for every hospital, I started with a grouped bar chart to display this information.
* A horizontal grouped bar chart was designed in order to accomodate the long DRG names. It also assisted in reducing cognitive load as the text was aligned horizontally from left to right and top to bottom.
* Drop down boxes were utilized to help select the particular hospital. This dropdown box was populated from the data.
* No tooltips were added to this visualization as it had axes with absolute values displayed on x-axis.

### Changes

#### Round 1

* Based on the feedback received, instead of showing the absolute values, the comparison was displayed on the bar graph in terms of how many times the DRG was costly or cheaper.
* Also, the number of DRGs to be displayed was increased from top-5 to top-25.
* Comparison with state average was also included in the visualization.
* Since, now both state and national average comparison were being displayed, two different svg objects were used with a single Y-axis to display the data while avoiding clutter which could be caused by the axis labels. However, two different X-axes were used as the data varied for both of them.
* In order to provide users with absolute values too, it was decided to add a tooltip to the bars to display the absolute values.
* The drop-down was populated with unique values as it was noted in the feedback that the first iteration contained multiple instances of the same hospital in the drop-down.

#### Round 2

* Based on the feedback from round 2, an overall comparison for each hospital was added.
* In order to display the overall average of the hospital, all providers were plotted on a map of the United States. A tooltip was added to these points displaying the overall comparison with national and corresponding state averages. Additionally, the points were colored red and green based on the national average was greater than national average or smaller than national average respectively.
* On click events were added to the hospitals on map which would then display the bar graphs for top-25 DRGs with the national and state comparison.

#### Round 3

* Apparently, the story being displayed on the visulaization was not clear to the user and the visualization seemed to be exploratory in nature. In order to combat this, a new chloropleth map was added as the introduction.
* This chloropleth map contains a clear introduction to the story. It displays the state averages of the medicare cost which clearly depicts wide variation in the hospital costs across the country.
* It was noted that the color coding of the hospitals was not colorblind friendly and had to be changed. Changes were made to the color of these points.

### Feedback

#### Round 1

##### Sumit
* Although I can compare the medicare cost of DRGs for each hospital with the national average cost, I would have been much happier if I could know how many times the particular DRG treatment is costly at the particular hospital.
* Is it possible to show the comparison with state average too?
* The drop down for the hospitals contain the same hospital multiple times. It should display each hospital only once.

#### Round 2

#### Deepak
* The visualization allows me to compare the top-25 DRGs for each hospital with national and state average. However, there is no way to know if a particular hospital is overall costly than the other hospitals in the same state or nation-wide.
* Is there a way we can display this information to find if particular states or areas are more expensive than the national average?
* Some hospitals have fewer than 25 DRGs displayed. (__No resolution for this as some hospitals contain data for less than 25 DRGs__)

#### Round 3

* The story being conveyed in the visualization is not clear. The visualization appears to be an exploratory one.
* The current version of the map isn't color-blind friendly, take a look at how it perceived by color blind people. It is hard to see any difference at all.

### Resources

* [Medicare Provider Utilization and Payment Data](https://www.cms.gov/Research-Statistics-Data-and-Systems/Statistics-Trends-and-Reports/Medicare-Provider-Charge-Data/index.html)

* Interactive Data Visualization for the web by Scott Murray

* Mastering D3.js by Pablo Navarro Castillo
