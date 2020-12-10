# Final-Project
# Baltimore City Life Expectancy and Mortality Rates

People are dying faster than warranted in poorer areas in Baltimore. This is not equitable and if there are ways to fix this, they should be fixed. Although we hypothesized that various food system initiatives might be better to improve health concerns, we found that median household income was one of the most important variables. Government officials should increasing the median household income through exploration of initiatives like Universal Basic Income or food distribution centers.

## Background

[CBS Baltimore](https://baltimore.cbslocal.com/2017/07/06/life-expectancy-baltimore/) stated there are discrepancies in terms of life-expectancy in different areas of Baltimore. In fact, poorer areas of Baltimore had a life expectancy that was 20-years lower than that of richer areas. Lower life expectancy and higher rates of mortality in poorer areas indicate that people are dying prematurely when these are preventable solutions, as those in richer areas are not dying so early. This problem is important as obviously we would like to create for a more equitable society, where people's livelihoods are not affected based on where they live- especially if there are ways to do so. According to [Baltimore City’s health department](https://health.baltimorecity.gov/state-health-baltimore-winter-2016/state-health-baltimore-white-paper-2017#:~:text=The%20leading%20causes%20of%20death,and%20chronic%20lower%20respiratory%20diseases), the leading cause of death in the city is heart disease. Life expectancy and mortality rates in the 45-64 age group in Baltimore can be assumed to be correlated with heart disease. There are many different causes of heart disease, but [The Mayo Clinic](https://www.mayoclinic.org/diseases-conditions/heart-disease/symptoms-causes/syc-20353118) states that the most common type of heart disease, atherosclerosis, is caused by an unhealthy diet, lack of exercise, and being overweight. These are issues that are amendable. Thus, a look into various variables related to food systems and physical activity in neighborhoods in the city of Baltimore was endeavored. This issue is of interest to us because we are both Baltimore citizens at least until we graduate from Hopkins. Not only is this relevant to us, but it also relevant for government officials who could learn the most effective ways to increase life expectancy and decrease rates of mortality. Not to mention, the leading cause of death in the United States is heart disease, so information from our analysis could help with the larger United States as well. 


## Business Question

___How can we combat life expectancy and mortality rates in the 45-64 age group in Baltimore City?___


## Open Data 

[Baltimore Neighborhood Indicators Alliance](https://vital-signs-bniajfi.hub.arcgis.com/):Open data source that we received data from. 

- [Average Healthy Food Availability Index](https://vital-signs-bniajfi.hub.arcgis.com/datasets/ebf53cd13e164a96b1f890c7162cf8c7_0?geometry=-76.915%2C39.192%2C-76.326%2C39.378): measures the nutritional environment of food retails in the area. It's a score that combines the nutritional and access to the food. Higher the score, the better the access to healthy food.

- [Percentage of Students Receiving Free or Reduced Meals](https://vital-signs-bniajfi.hub.arcgis.com/datasets/2748ad5e859841f5bba17d3f208b56df_0)

- [Number of Miles of Bike Lanes](https://vital-signs-bniajfi.hub.arcgis.com/datasets/d88926354e4d4bab93c174a7cf2cdf2d_0)

- [Median Household Income](https://vital-signs-bniajfi.hub.arcgis.com/datasets/8613366cfbc7447a9efd9123604c65c1_0)

- [Mortality by Age (45-64 Years old)](https://vital-signs-bniajfi.hub.arcgis.com/datasets/d7f38ce4d36b4731b1b6cad189c8fddf_0)

- [Life Expectancy](https://vital-signs-bniajfi.hub.arcgis.com/datasets/c7bc491a655741f59b3d80932b9857d6_0)


## Data Questions

_Which variables explain the changes in mortality rate (45-64 age) and life expectancy in Baltimore City?_

_Does median income and free and reduced meals explain the changes in mortality rate (45-64 age) and life expectancy in Baltimore City?_

_How does the data group itself into separate clusters of neighborhoods in Baltimore City?_

## Data Analysis 

__Regression__

We initially wanted to look and see whether all our variables were significant enough to affect the dependent variable. However, after doing multiple linear regression analysis for both mortality rate and life expectancy, only 1-2 variables were significant, so we decided to do simple linear regression on all the independent variables and found that 2 variables, free and reduced meals and median household income, were significant for both mortality rate and life expectancy. Average healthy food index was significant for mortality rate with a p-value of 0.0358, but its R-squared value was 0.0805, so we decided to not include it as one of the variables to visualize and discuss.

![alt text](https://github.com/skang06/Baltimore-City-Livelihood/blob/main/midterm%20project%20mort%20rate%20graphs.png)

__**Mortality Rate, 45-64:**__

The p-value for free and reduced meals was 7.5133E-11 and the p-value for median household income was 2.5459E-11, meaning that both these independent variables were significant and are able to explain the changes in the dependent variable. As we can see in the graphs above, the trendline mostly fits the shape and direction of the data points and there are no extreme outliers that skew the data. Mortality rate has a positive relationship with free and reduced meals and has a negative relationship with median household income. This means that mortality rate increases when there are more free and reduced meals and mortality rate decreases when median household income is greater.

Equations:

Mortality rate = 1.922(free/reduced meals) – 21.416

Mortality rate = -0.001(median household income) + 180.110

![alt text](https://github.com/skang06/Baltimore-City-Livelihood/blob/main/midterm%20project%20life%20exp%20graphs.png)

__**Life Expectancy:**__

The p-value for free and reduced meals was 8.0678E-11 and the p-value for median household income was 6.3693E-14, meaning that both these independent variables were significant and are able to explain the changes in the dependent variable. As we can see in the graphs above, the trendline mostly fits the shape and direction of the data points and there are no extreme outliers that skew the data. Life expectancy has a negative relationship with free and reduced meals and has a positive relationship with median household income. This means that life expectancy decreases when there are more free and reduced meals and life expectancy increases when median household income is greater

Equations:

Life expectancy = -0.240(free/reduced meals) + 90.609

Life expectancy = 0.0001(median household income) – 66.240

__Clusters and Their Characteristics__

![alt text](https://github.com/skang06/Baltimore-City-Livelihood/blob/main/mortalityratte.png)

__Mortality Rate:__ 

_Cluster 1_ (Lauraville): Cluster in between Cluster 2 and 3 in terms of all measures.

_Cluster 2_ (Greater Roland Park/Poplar Hill): Most below average level of mortality rate. Most below average number of people on free and reduced meals and lowest average healthy food availability index. Most above average median household income, number of bike lanes. 

_Cluster 3_(Pimlico/Arlington/Hilltop): Highest above average rate of mortality. Highest above average number of people in free and reduced meals. Also, the most below average median household income, number of bike lanes, and average healthy food accessibility index among the different clusters.  


__Life Expectancy:__ 

![alt text](https://github.com/skang06/Baltimore-City-Livelihood/blob/main/lifeexpectancy.png) 

_Cluster 1_ (Lauraville): Cluster in between Cluster 2 and 3 in terms of all measures.

_Cluster 2_ (Allendale/Irvington/S.Hilton) : Most below average age of life expectancy among the different clusters. Highest above average number of people in free and reduced meals. Also, the most below average median household income, number of bike lanes, and average healthy food availability index. 

_Cluster 3_ (North Baltimore/Guilford/Homeland): Most above average age of life expectancy. Most below average number on free and reduced meals and lowest average healthy food availability index. Highest above average median household income, number of bike lanes. 


## Business Answer and Solutions

The cluster analysis found that although some of the variables were not shown as significant in the multiple linear regression, there was a clear pattern in the cluster analysis. For instance, bike lanes were not shown to be significant in the multiple linear regression. However, according to the cluster analysis, those clusters with the most above average rate of mortality or most below average age for life expectancy, also had the highest number of bike lanes. Thus, like free and reduced meals, this could be more associated with the median household income in the neighborhoods in the cluster. Thus, we could relay to officials that bike lanes is not that important of a method to spend money in, although a cluster analysis alone might have suggested it. 

Overall, the cluster analysis helps us understand where to focus our efforts and initiatives. We should focus on the neighborhoods in cluster 3, in the analysis that included the mortality rate variable, as it had the most above average rate of mortality, and cluster 2, in the analysis with the life expectancy variable, as it had the most below average lowest life expectancy. There are 28 neighborhoods and 31 neighborhoods in the respective clusters. 

The linear regression analysis of our data showed that free and reduced meals and median income are significant variables that can explain the changes in life expectancy and mortality rate. Although there is a negative relationship between life expectancy and free and reduced meals, the negative relationship is more due to the free and reduced meals being an indicator for low income rather than it directly causing the lower life expectancy and higher mortality rate. Therefore, a major focus of our policies should be putting more disposable income into the hands of those who most need it.

Disposable income can be distributed in many ways, but we feel that a potentially useful policy for this is universal basic income. Many studies have shown that the minimum wage is no longer a living wage and many poorer families struggle to put food on the table ([The New Yorker](https://www.newyorker.com/magazine/2018/07/09/who-really-stands-to-win-from-universal-basic-income)). Universal basic income is a hotly debated topic that could potentially mitigate this ([Investopedia](https://www.investopedia.com/articles/personal-finance/022615/can-family-survive-us-minimum-wage.asp#:~:text=The%20minimum%20wage%20in%20the,more%20than%20half%20a%20century.)). Various experiments are being conducted across the US to see the efficacy of such a policy and should it prove effective, we believe that this would be a potential solution. 

We originally wanted to work with obesity prevalence data to have a more pointed solution, especially since some of the leading causes of mortality in Baltimore City are heart disease and stroke, of which obesity is a major risk indicator ([Baltimore City Health Department](https://health.baltimorecity.gov/state-health-baltimore-winter-2016/state-health-baltimore-white-paper-2017#:~:text=The%20leading%20causes%20of%20death,and%20chronic%20lower%20respiratory%20diseases.)). However, since we did not have the data necessary for a direct analysis, we are extrapolating our data relating to mortality rate and life expectancy and our own research into the major causes of mortality and the public health situation in Baltimore City in order to make further detailed conclusions with the data.

As shown in Baltimore City Health Department’s snapshot of the city’s public health situation, one in three high school students are either obese or overweight and many have unhealthy eating habits. In addition, “less than half of middle school students eat breakfast on a daily basis” ([Baltimore City Health Department](https://health.baltimorecity.gov/state-health-baltimore-winter-2016/state-health-baltimore-white-paper-2017#:~:text=The%20leading%20causes%20of%20death,and%20chronic%20lower%20respiratory%20diseases.)). Judging by these observations, a policy such as additional education program in middle school or high school teaching students proper eating habits and how to eat healthily could help students improve their eating habits. 

However, the cause of the eating habits may not be due to the students themselves but rather a lack of income necessary to buy healthier food options. This related to a policy we suggested above, universal basic income; there are also other ways to supply healthy food options such as food distribution centers and special discounts on certain food items, similar to programs such as the WIC program ([WIC](https://www.fns.usda.gov/wic)). In addition, many of these unhealthy food options are provided by the school itself. Many school lunches contain unhealthy calories and quite a few students rely on free and reduced lunches to get one meal a day ([UC Davis Health](https://health.ucdavis.edu/good-food/blog/school-lunches-and-kids.html)). Therefore, schools should increase their funding for providing healthier food options for school lunches.
 

## Future Suggestions

The policies we have suggested can be pitched to public entities such as the Baltimore City Health Department, which is already working on various programs to help with food access, and also private entities such as NGOs like Eco City Farms or Food Link, Inc. ([Foodtank](https://foodtank.com/news/2014/11/five-awesome-food-organizations-in-maryland/)). There isn’t necessarily a shift or pivot that needs to happen in order for such changes like we have suggested to occur. Rather, there just needs to be stronger urgency in establishing programs like universal basic income and better assistance with healthy food access. 

To further draw more specific conclusions, more specific data on heart disease and obesity would help to determine which indepdendent variables affect these specific problems the most. 
