![Chicago Traffic](https://github.com/6cats1dog/Chicago_Car_Crashes/blob/main/Chicago%20Traffic.jpg)
# Chicago Car Crashes

In this phase 3 project we build a classifier to predict the primary contributory cause of a car accident, given information about the car, the people in the car, the road conditions etc. We view the audience as a Vehicle Safety Board who's interested in reducing traffic accidents.

The goal of this project was to produce predictive model that would facilitate the analysis of the primary causes for car crashes. Using data provided by the City of Chicago the aim was to the information provided from the Chicago Data Portal and identify patterns and trends that can be implemented with satisfactory results. The goal is to reduce the instances of crashes with preventive measures informed by the predictive model.

### Data Setup and Cleaning:
The Traffic Crashes data comes from the Chicago Data Portal in which we can access a number of specific points regarding crash incidents such as the location and time information, road conditions, lighting, and driving behaviors. Most of the focus of this project was obtained bby working with the Primary Contributory cause, which are those factors that were believed to have contributed to the accidents in the first place. There was a substantial amount of data which can be accessed at  https://data.cityofchicago.org/Transportation/Traffic-Crashes-Crashes/85ca-t3if

Data Exploration:
In exploring the data, the majority of focus was on looking at the causatory factors involved in accidents which lead to major injury and in specific fatalities. Given the severe resulting nature of these accidents, it was believed to be the most pertinent and the most impactful features to explore to hopefully help the City of Chicago reduce the amount of these types of incidents. We were ble to obtain ample information regarding the specific primary causes of these accidents based on conditions such as the dirving behavior and the physical condition of the driver, namely those that were under the influence. Four of the top five causes for fatal crashes were a result of a driver behaving in an aggressive and reckless manner, with the most fatalities attributed to the physical condition of the driver and failing to yield to the right of way. 

### Data Modeling:
In order to prepare our data for modeling, the primary causatory factors where combined into three catagories: Improper/Aggressive Driving, Reckless Driving Behavior, and External Factors/ Others. Reckless driving behavior included behavior that can be labeled as very dangerous to the driver and others, such as impaired driving and exceeding the authorized speed limit. Improper/Aggressive Driving outlined behabviors such as turning right on red, and failing to yield to right of way. External Factors/Others included items such weather, distractions outside of the car and driving ability of the indiviual

Multiclass classification models were used in order to try to classify these incidents. The models K-Nearest Neighbors, Decision Trees, Random Forest, Gridsearch, and XGBoost were used. The best multiclass model used for our data was our K-Nearest Neighbor, which had an accuracy of roughly 63%

### Conclusion
From the information derived from classification and exploring trends supported by modeling, we believe that the City of Chicago should implement factors that will help reduce the amount of reckless driving behavior seen. For example, it may be beneifical to add more sobriety checkpoints on the weekends when there seems to be more fatal accidents than any other day of the week. Also using speed markers that make drivers aware of their speed or red light cameras at busy intersections could reduce the amount of fatal accidents related to failing to yield to the right-of-way and failure to reduce speed to avoid an accident. These free factors are the greatest in contributing to fatal accidents.

### Future Work
Future work that will be useful is to continue to test our models with both historical data (data before 2015) and current crash incident data. This will allow us to continuously evaluate our models based on the data received and can help review whether the implementations recommended above proved effective in reducing fatal accidents and had a trickle down effect to less severe incidents. The City of Chicago could also coordinate with other large cities such as Los Angeles and New York City to see if there are factors that Chicago may be missing that can help improve driver's safety. It may also be beneficial to look at other cities with low fatality resulting accidents and see if any preventive measure they have in place can be scaled to a city such as Chicago and obtain a reduction of accidents.

### Data Used:
* Traffic_Crashes_-_Crashes.csv.zip

