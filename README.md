
# Medicare Charge Data 

### Summary

* The medicare charge data for around 3000 hospitals has been released by Center for Medicare and Medicaid Services since 2011. Till 2013, only the top 100 _DRG(Diagnosis Related Group)_ for every hospital were released. However, from 2014 onwards, the center has started releasing data related to all DRG. More info about the data can be found [here](https://www.cms.gov/Research-Statistics-Data-and-Systems/Statistics-Trends-and-Reports/Medicare-Provider-Charge-Data/index.html)
* This data visualization displays a comparison of the average medicare cost charged by the hospitals against the national and state averages. There are two levels on which the above comparison can be made. First, on the overall medicare cost and the second on the basis of individual DRG.

### Design

* The original design consisted of the national average medicare cost and the hospital average medicare cost displayed as a grouped bar chart for the top-5 DRG.
* However, the design evolved over the period of time to finally display the overall average medicare cost for each hospital plotted over a map with top-25 DRG comparisons for each hospital plotted as a bar chart.

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

### Resources

* [Medicare Provider Utilization and Payment Data](https://www.cms.gov/Research-Statistics-Data-and-Systems/Statistics-Trends-and-Reports/Medicare-Provider-Charge-Data/index.html)

* Interactive Data Visualization for the web by Scott Murray

* Mastering D3.js by Pablo Navarro Castillo
