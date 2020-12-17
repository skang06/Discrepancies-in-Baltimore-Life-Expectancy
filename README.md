# Final-Project
# Baltimore City Life Expectancy and Mortality Rates

People are dying faster than warranted in poorer areas in Baltimore. This is not equitable and if there are ways to fix this, they should be fixed. Although we hypothesized that various food system initiatives might be better to improve health concerns, we found that median household income was one of the most important variables. Government officials should increasing the median household income through exploration of initiatives like Universal Basic Income or food distribution centers.

## Background

[CBS Baltimore](https://baltimore.cbslocal.com/2017/07/06/life-expectancy-baltimore/) stated there are discrepancies in terms of life-expectancy in different areas of Baltimore. In fact, poorer areas of Baltimore had a life expectancy that was 20-years lower than that of richer areas. Lower life expectancy and higher rates of mortality in poorer areas indicate that people are dying prematurely when these are preventable solutions, as those in richer areas are not dying so early. This problem is important as obviously we would like to create for a more equitable society, where people's livelihoods are not affected based on where they live- especially if there are ways to do so. According to [Baltimore City’s health department](https://health.baltimorecity.gov/state-health-baltimore-winter-2016/state-health-baltimore-white-paper-2017#:~:text=The%20leading%20causes%20of%20death,and%20chronic%20lower%20respiratory%20diseases), the leading cause of death in the city is heart disease. Life expectancy and mortality rates in the 45-64 age group in Baltimore can be assumed to be correlated with heart disease. There are many different causes of heart disease, but [The Mayo Clinic](https://www.mayoclinic.org/diseases-conditions/heart-disease/symptoms-causes/syc-20353118) states that the most common type of heart disease, atherosclerosis, is caused by an unhealthy diet, lack of exercise, and being overweight. These are issues that are amendable. Thus, a look into various variables related to food systems and physical activity in neighborhoods in the city of Baltimore was endeavored. This issue is of interest to us because we are both Baltimore citizens at least until we graduate from Hopkins. Not only is this relevant to us, but it also relevant for government officials who could learn the most effective ways to increase life expectancy and decrease rates of mortality. Not to mention, the leading cause of death in the United States is heart disease, so information from our analysis could help with the larger United States as well. 

Our primary stakeholder is Dr. Letitia Dzirasa, the current Baltimore City Health Commissioner. We believe that she will be particularly interested in this issue because one of her special interests include obesity management. Moreover, the previous Baltimore City health commissioner, Dr. Leana Wen, has mentioned that she wants to close the life expectancy gap between poor and wealthy areas per an article in the [Baltimore Business Journal](https://www.bizjournals.com/baltimore/news/2018/06/13/baltimore-health-chief-wen-others-discussclosing.html?fbclid=IwAR2Zfy91CoIY2mmkTy-creAW91gThk0SlIB8E6PplxzKtfMNk4Kf2RRd_4A). Our secondary stakeholder will be the Baltimore City mayor, Brandon Scott. Although there are many different departments in the process of getting a budget approved, the mayor has the ability to approve the total budget at the end of the process. 

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

We initially wanted to look and see whether both free and reduced meals and median household income were significant enough to affect life expectancy. However, after doing multiple linear regression analysis for ife expectancy, only free and reduced meals had a significant p-value, so we decided to do simple linear regression on free and reduced meals and median household income individually and found that both variables were significant for life expectancy. 

![alt text](https://github.com/skang06/Baltimore-City-Livelihood/blob/main/midterm%20project%20life%20exp%20graphs.png)

__**Life Expectancy:**__

The p-value for free and reduced meals was 8.0678E-11 and the p-value for median household income was 6.3693E-14, meaning that both these independent variables were significant and are able to explain the changes in the dependent variable. As we can see in the graphs above, the trendline mostly fits the shape and direction of the data points and there are no extreme outliers that skew the data. Life expectancy has a negative relationship with free and reduced meals and has a positive relationship with median household income. This means that life expectancy decreases when there are more free and reduced meals and life expectancy increases when median household income is greater

Equations:

Life expectancy = -0.240(free/reduced meals) + 90.609

Life expectancy = 0.0001(median household income) – 66.240



__Clusters and Their Characteristics__

![alt text](ADD LINK TO CLUSTER CHART)

__Life Expectancy:__ 

![alt text](add link!!!!) 

_Cluster 1_ (Allendale/Irvington/S.Hilton): Most below average age of life expectancy among the different clusters. Highest above average number of people in free and reduced meals. Also, the most below average median household income.

_Cluster 2_ (Beechfield/Ten Hills/West Hills) : Cluster in between Cluster 1 and 3 in terms of all measures. 

_Cluster 3_ (Belair Edison): Most above average age of life expectancy. Most below average number on free and reduced meals. Highest above average median household income.

We should focus on the neighborhoods in cluster 1 as it had the most below average lowest life expectancy. The cluster analysis coincides with our regression analysis in that there is a negative relationship between life expectancy and free/reduced meals, and a positive relationship between life expectancy and median household income.

## Similar Data Analysis Outside of Baltimore

__Unemployment Rate vs Poverty Rate for Cities in Bay Area, California:__

![alt text](add link!!!!) 

As expected and demonstrated in the graph, those cities with lowest rates of poverty compared to others in the Bay Area, have higher unemployment rates in their particular city. Overall, unemployment rate and poverty have similar trends, meaning that they are either both higher or both lower comparably. However, the unemployment rate and the poverty rates do not demonstrate the strong direct relationship that was assumed. Interestingly enough, there are several cities where the poverty rate is higher than the unemployment rate. Nearly all the cities that have the highest rates of poverty in the Bay Area, based on the chart, have a lower unemployment rate than poverty rate in that city.
This provides more evidence for the need for UBI. For most of the cities with the worst poverty, there is an unemployment rate that is not that high comparably. This could indicate that getting more disposable income is more of an effective solution to combating poverty than more jobs.

__Life Expectancy and Poverty Rate for Counties in Bay Area, California:__
![alt text](https://raw.githubusercontent.com/skang06/bayarea_ue_poverty_life_expectancy/main/Screen%20Shot%202020-12-06%20at%204.02.49%20PM.png) 

As shown in the combined line and bar graph there is a roughly inverse relationship between poverty rate and life expectancy. When poverty rate is lower, the life expectancy is higher. This helps to confirm the article that indicated the life expectancy is lower in places with more poverty. As this is a wider data set encompassing all counties in the Bay Area, we can assume we can apply to results to Baltimore City.As shown in the combined line and bar graph there is a roughly inverse relationship between poverty rate and life expectancy. When poverty rate is lower, the life expectancy is higher. This helps to confirm the article that indicated the life expectancy is lower in places with more poverty. As this is a wider data set encompassing all counties in the Bay Area, we can assume we can apply to results to Baltimore City.

__Life expectancy vs. Poverty rate for Baltimore and Chicago__

Before the poverty rate and life expectancy rate comparison in both cities, it would make sense to compare how two cities are different from each other in terms of demographics, including the total population, age group population, and gender ratio. 

__Age group distribution in Baltimore and Chicago (add bar graphs)__

Age group distribution in Chicago and Baltimore are almost the same. The highest age group population is 30 - 49 years old for both cities, and both cities have bell curved shape distributions. Also, the second highest age group populaiton were 21-29 age group and 50-61 age group for both cities. One of the main differences is that the total populaiton is much higher for Chicago where the total populaiton is 600K compared to Baltimore where the total populaiton is almost 2.7M. Due to the higher population in Chicago, although the trend for age group distributions are same for both cities, the actual population for each bar is much higher for Chicago. 

__Gender Ratio in Baltimore and Chicago__

Next is gender ratio comparison in both cities. In both cities, there are more male population than female population. However, Baltimore has a slightly higher male population of 53.1% whereas the male populaton in Chicago is 51.3%.

Now that we have seen the differences and similarities of both cities in terms of demographcis, we can see if the same trend between the poverty rate and life expectancy holds in both cities.

__Linear Regression__

As shown in the linear regression summary output, the poverty rate is significant enough in explaining the output of life expectancy rate in Baltimore given that the p-value of poverty rate is lower than 0.05. Same applies to Chicago where the p-value of poverty rate was also lower than 0.05.

__Scatter plot and trend line__
 
Both scatter plots and trend lines clearly show that both the poverty rate and life expectancy rate have an inverse relationship in both Baltimore and Chicago. As poverty rate increases, the life expectancy tend to decrease and vice versa. Given the slight difference in Baltimore and Chicago in terms of demographics, still the poverty rate and life expectancy rate had a strong inverse relationship. This reinforces that how important it’s to lower the poverty rate to increase the life expectancy rate. 

__Per capita income vs. Life expectancy rate in Chicago  (add scatter plot)__

In the previous part, we compared the median household income and life expectancy rate in Baltimore. Here, we used per capita income instead of median household income for Chicago. Compared to the Baltimore scatterplot, both cities have the same trend of positive relaitonship between two variables which means that as income increases, the life expectancy rate increased. The only main difference is that the individual dots are more spread out for Chicago whereas the individual dots are more closely clustered around the trend line for Baltimore. This might indicate that the R^2 value could be lower for Chicago, which means that per capita income could be better in explaining the life expectancy rate in Baltimore. Thus, it would be much more significant for Baltimore to have solutions that could increase the income level and lower the poverty rate to eventually increase the life expectancy rate in Baltimore. 


## Business Answer and Solutions

The cluster analysis found that although some of the variables were not shown as significant in the multiple linear regression, there was a clear pattern in the cluster analysis. For instance, bike lanes were not shown to be significant in the multiple linear regression. However, according to the cluster analysis, those clusters with the most above average rate of mortality or most below average age for life expectancy, also had the highest number of bike lanes. Thus, like free and reduced meals, this could be more associated with the median household income in the neighborhoods in the cluster. Thus, we could relay to officials that bike lanes is not that important of a method to spend money in, although a cluster analysis alone might have suggested it. 

Overall, the cluster analysis helps us understand where to focus our efforts and initiatives. We should focus on the neighborhoods in cluster 3, in the analysis that included the mortality rate variable, as it had the most above average rate of mortality, and cluster 2, in the analysis with the life expectancy variable, as it had the most below average lowest life expectancy. There are 28 neighborhoods and 31 neighborhoods in the respective clusters. 

The linear regression analysis of our data showed that free and reduced meals and median income are significant variables that can explain the changes in life expectancy and mortality rate. Although there is a negative relationship between life expectancy and free and reduced meals, the negative relationship is more due to the free and reduced meals being an indicator for low income rather than it directly causing the lower life expectancy and higher mortality rate. Therefore, a major focus of our policies should be putting more disposable income into the hands of those who most need it.

Disposable income can be distributed in many ways, but we feel that a potentially useful policy for this is universal basic income. Many studies have shown that the minimum wage is no longer a living wage and many poorer families struggle to put food on the table ([The New Yorker](https://www.newyorker.com/magazine/2018/07/09/who-really-stands-to-win-from-universal-basic-income)). Universal basic income is a hotly debated topic that could potentially mitigate this ([Investopedia](https://www.investopedia.com/articles/personal-finance/022615/can-family-survive-us-minimum-wage.asp#:~:text=The%20minimum%20wage%20in%20the,more%20than%20half%20a%20century.)). Various experiments are being conducted across the US to see the efficacy of such a policy and should it prove effective, we believe that this would be a potential solution. 

We originally wanted to work with obesity prevalence data to have a more pointed solution, especially since some of the leading causes of mortality in Baltimore City are heart disease and stroke, of which obesity is a major risk indicator ([Baltimore City Health Department](https://health.baltimorecity.gov/state-health-baltimore-winter-2016/state-health-baltimore-white-paper-2017#:~:text=The%20leading%20causes%20of%20death,and%20chronic%20lower%20respiratory%20diseases.)). However, since we did not have the data necessary for a direct analysis, we are extrapolating our data relating to mortality rate and life expectancy and our own research into the major causes of mortality and the public health situation in Baltimore City in order to make further detailed conclusions with the data.

As shown in Baltimore City Health Department’s snapshot of the city’s public health situation, one in three high school students are either obese or overweight and many have unhealthy eating habits. In addition, “less than half of middle school students eat breakfast on a daily basis” ([Baltimore City Health Department](https://health.baltimorecity.gov/state-health-baltimore-winter-2016/state-health-baltimore-white-paper-2017#:~:text=The%20leading%20causes%20of%20death,and%20chronic%20lower%20respiratory%20diseases.)). 

Research has found that obesity in young adults has the potential to shorten life expectancy by up to 8 years and even reduce healthy living years by up to 19 years. Obesity can also lead to and has high comorbidity with other health issues such as diabetes type 2 and cardiovascular disease. In fact, researchers say that “the more an individual weighs and the younger their age, the greater the effect on their health, as they have many years ahead of them during which the increased health risks associated with obesity can negatively impact their lives” ([Science Daily](https://www.sciencedaily.com/releases/2014/12/141205094841.htm#:~:text=The%20study%20shows%20that%20being,very%20obese%20men%20and%20women)). This means that the impact of unhealthy eating on school age children in Baltimore could have severe consequences as they age and could be part of the reason why there is such a discrepancy in life expectancy between those living in neighborhoods greatly affected by poverty and those that are not. Many of these more impoverished neighborhoods are also areas in which the rate of free and reduced meals is much higher than the average, meaning that school provided meals could greatly impact the food choices and eating habits of students living in those areas. This is why we believe that some part of our proposed solution should aim to help improve the health and eating habits of school aged children in Baltimore.

Judging by these observations, a policy such as additional education programs in middle school or high school teaching students proper eating habits and how to eat healthily could help students improve their eating habits. 

However, the cause of the eating habits may not be due to the students themselves but rather a lack of income necessary to buy healthier food options. This related to a policy we suggested above, universal basic income; there are also other ways to supply healthy food options such as food distribution centers and special discounts on certain food items, similar to programs such as the WIC program ([WIC](https://www.fns.usda.gov/wic)). In addition, many of these unhealthy food options are provided by the school itself. Many school lunches contain unhealthy calories and quite a few students rely on free and reduced lunches to get one meal a day ([UC Davis Health](https://health.ucdavis.edu/good-food/blog/school-lunches-and-kids.html)). Therefore, schools should increase their funding for providing healthier food options for school lunches.

We have looked into the cost and logistics of providing healthier food options and we found that the Baltimore City Public Schools budget for the 2019 and 2020 school year was the following ([Baltimore City Public Schools](https://www.baltimorecityschools.org/sites/default/files/inline-files/FY21_AdoptedOperatingBudget_051420_Remediated.pdf)):

Expenses by category, all funds, food services - Year by year comparison:

FY 19 Actual: 44,086,784

FY 20 Adopted: 46,087,798

FY 21 Adopted: 45,255,331

Food and Nutrition Services Expenditures - Year by year comparison:

FY 19 Actual: 53,654,833

FY 20 Adopted: 55,304,192

FY 21 Adopted: 54,540,838

 
We estimate that the school would need to set aside $7,000,000 more per year to help acquire healthier food choices for the schools in the Baltimore City Public Schools school district. Some studies have found that having healthier food in school meals actually doesn’t cost more than typical unhealthy food choices while USDA has found that meeting nutritional standards published by the [USDA](https://www.ers.usda.gov/amber-waves/2013/april/the-food-costs-of-healthier-school-lunches/) only costs marginally more than what the school district is already spending, so we believe that the budget increase we have proposed is reasonable to cover all potential additional food costs for healthier choices ([My San Antonio](https://www.mysanantonio.com/news/local_news/article/Menu-can-be-healthy-for-kids-bottom-line-3808172.php))([Cambridge University Press](https://www.cambridge.org/core/journals/agricultural-and-resource-economics-review/article/abs/food-costs-of-healthier-school-lunches/501159B3AB85F8257920BF41E4198DF8)).

 

## UBI 
Upon doing research, we found there were a lot of food distribution centers and food initiatives in place already, that’s why we wanted to propose UBI as a new, unique solution to try. 

__Importance of UBI__

As the analyses above show, as the poverty rate increases the life expectancy rate decreases in Baltimore. Moreover, as the median household income increases the life expectancy rate increases as well. These analyses indicate that our solutions should focus on increasing the disposable income especially for people who are under the poverty threshold. And UBI is a great long-term solution to alleviate povert by allowing people who meet certain criteria to receive a set amount of money on a regular basis, and this could eventually help the life expectancy rate to increase in Baltimore. Operations can change as a result. According to the [Food Ethics Council](https://www.foodethicscouncil.org/app/uploads/2020/06/Food-Policy-on-Trial-on-UBI-Food-Ethics-Council-jurys-verdict-and-summary-1.pdf), one way UBI can help increase the life expectancy is to help people to get better access to good food and healthier diets. As the analysis above shows, free/reduced meals have negative correlations with the life expectancy rate in Baltimore. Thus, people would have better access to healthier food with the help of UBS, and this would increase the life expectancy rate in Baltimore. 

__Potential outcome without UBI__

Since UBS is more of a long term solution, it would take time to see the actual result and thus it would be difficult for the analysis to be retrospective for now. If we hadn’t done the analysis and the organization took no action, the short-term result we might face next year is the misallocation of the available fund by the organization. We would not be able to see any drastic change in life expectancy or poverty rate since both of the variables are long-term variables. However, it is true that organization wouldn’t have a clear idea of why the life expectancy rate is decreasing in Baltimore and what the driving factors are. Thus, the organization might misallocate the available fund instead of focusing on alleviating the poverty since they wouldn’t know that the poverty rate is one of the main reasons for low life expectancy rate in Baltimore. And probably in 5 years, if the organization took no action, there is a high possibility for people in Baltimore to face decreased life expectancy rate. People under the poverty line would suffer continuously since no actions were taken, and that might accelerate the decrease in the life expectancy rate in Baltimore. And data analysis-wise, the negative correlation between the poverty rate and the life expectancy rate might get stronger. 

__Success and Failure examples of UBI__

Different countries and states have experimented with UBI or similar small-scale trials [UBI Case studies](https://www.vox.com/future-perfect/2020/2/19/21112570/universal-basic-income-ubi-map). In Canada, there was a randomized controlled trial in the province of Manitoaba where every household was able to participate and get basic income. After 5 years, there was actually a 8.5% reduction in the hospitalization rate and also a decline in doctor visits. Thus, the program actually helped residents to improve their physical and mental health. However, since the program was funed by the provincial and federal government, it got canceled when a more conservative power took in place. Thus, for a successful implementation of UBI, it would be important to make the program as stable as possible wihtouth being affected by changes in the government. Another concern that UBI might have is the possibility of the recipients’ unwillingness to find jobs. Spain, in 2017, implemented a similar program called “B-MINCOME,” a two-year program that offered $1,968 per month to almost 1000 randomly selected households. This successful program was able to boost life satisfaction and mental health, and surprisingly, it did not affect the participants’ willingness to find jobs. Although, the case in Spain was successful, analysis on job searching rate for participants before and after they receive UBI would be necessary to make the program to be effectively implemented in Baltimore. 


__Potential Timeline:__
- Conduct research to get more accurate cost estimate and population estimate.
- Scrutinize budget to determine how to reallocate funds
- Receive approval from Mayor (and all the other entities involved in the budget process).

The organization should continue to track life expectancy for next couple decades through Baltimore City records.  If life expectancy increases, they know they have succeeded. Moreover, they should track poverty rate as well to see if the decrease in poverty rate helped increase life expectancy in Baltimore. This will tell them that UBI and free/reduced meals is effective.

We will give $450 per person per household (4 people) that makes under $25,100 per year. We chose $450 because there was a trial of UBI in [Stockton, California](https://www.nytimes.com/2020/07/01/us/ubi-california.html)where each individual was given $500. The cost of living is higher in California than Baltimore, so we made the assumption that $450 is an adequate amount. According to the [Federal Poverty Guidelines](https://www.peoples-law.org/federal-poverty-guidelines), the federal poverty threshold for a four person household in 2018 was $25,100. [Poverty statistics from 2016](https://mda.maryland.gov/about_mda/Documents/SNAB/Maryland-Poverty-Profiles_2018_1-15-2018_T.pdf)found that 23.1% of people in Baltimore City were in poverty. This made out to 137,964 people living in poverty in 2016, according to the same article. Thus, we estimated that there are approximately 140,000 people living in poverty currently in Baltimore City. $450/ person makes the total cost estimate out to $63M (140,000 people * $450 = $63M). 
Outside funding will be difficult because UBI needs to be government-funded and outside funding usually pertains to private funding. The government would need to increase their proposed budget and also rearrange their current budget.

## Future Suggestions

The policies we have suggested can be pitched to public entities such as the Baltimore City Health Department, which is already working on various programs to help with food access, and also private entities such as NGOs like Eco City Farms or Food Link, Inc. ([Foodtank](https://foodtank.com/news/2014/11/five-awesome-food-organizations-in-maryland/)). There isn’t necessarily a shift or pivot that needs to happen in order for such changes like we have suggested to occur. Rather, there just needs to be stronger urgency in establishing programs like universal basic income and better assistance with healthy food access. 

To further draw more specific conclusions, more specific data on heart disease and obesity would help to determine which indepdendent variables affect these specific problems the most. 
