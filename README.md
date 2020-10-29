# Dataset: U.S. Traffic Accidents
We explored data on U.S. accidents from 2016 to 2019 with approximately 3 million recorded accidents. The dataset includes accidents in the 49 contiguous states. 
The dataset was collected in real time and includes factors associated with the accidents, such as location, time, weather and environmental conditions and severity of accidents, among others.
We used US Census Data for our population density analysis and Google Maps API for its plotting.

Citations: 

Moosavi, Sobhan, Mohammad Hossein Samavatian, Srinivasan Parthasarathy, and Rajiv Ramnath. “A Countrywide Traffic Accident Dataset.”, 2019.
Moosavi, Sobhan, Mohammad Hossein Samavatian, Srinivasan Parthasarathy, Radu Teodorescu, and Rajiv Ramnath. "Accident Risk Prediction based on Heterogeneous Sparse Data: New Dataset and Insights." In proceedings of the 27th ACM SIGSPATIAL International Conference on Advances in Geographic Information Systems, ACM, 2019.

# Initial Questions
How severe* are the accidents in terms of impact on traffic?
What states have the most accidents/least accidents? What about cities? Does population density factor in?
Does time play a role? Across the year, seasons, months, days, or hours? If so, to what extent?
Does weather play a role? If so, to what extent? What other environmental factors contribute to accidents?

# Data-Cleaning Process
We reduced the number of variables to analyze by dropping columns that either had null values or were not relevant to the questions we wanted to answer.
Then we reduced our analysis to the past three recorded years, dropping all of 2016 except for the month of December to account for our Seasons analysis.
We simplified time by dropping the minutes and keeping the hours to analyze traffic accidents by hours of the day.
We grouped seasons into the following categories: Winter (Dec, Jan, Feb); Spring (Mar, Apr, May); Summer (Jun, Jul, Aug); Fall (Sept, Oct, Nov).
We grouped weather conditions into six broad categories: Clear, Rain, Fog, Snow, Sleet, Wind.

# Traffic Accidents and Severity
In general, we saw a steady increase in the number of accidents per year countrywide. 
Next, we looked into the severity of all accidents. 
Note: Severity level =  impact on traffic; a number between 1 and 4, where 1 indicates the least impact on traffic (i.e., short delay and 4 indicates high impact on traffic).
As shown, most accidents fall into moderate to slightly high impact on traffic, with most accidents (67%) falling into severity level 2.

# Traffic Accidents Across States and Cities
California surpassed other states significantly in the number of accidents across three years.
Interestingly, of the top 10 cities with the most accidents across three years, only one city in California is on the list. Three cities in Texas are on the list. 

# Traffic Accidents vs Population Density
States with a higher population density also had higher rates of accidents. 
Looking further into the most populous state, California, we saw that counties with higher population densities also had higher rates of accidents. 

# Conclusions
The number of accidents is directly related to the density of the populations, with more accidents happening in the most densely populated states. These accidents tend to be moderately severe in terms of impact on traffic.
Accidents tend to occur mostly during morning and evening rush hours with a notable peak in the number of accidents during those hours; for some cities with more traffic, this peak is more obvious. 
Extreme weather could be causing approximately 13% of accidents in the US, although wet road accidents were not directly studied in this analysis.

This is further demonstrated by the correlation analysis, which shows a correlation between humidity and the number of accidents. 
In general, human factors is a more likely cause of accidents as seen by our population density and time analyses, which lead us to conclude that the more cars are on the road, the more likely traffic accidents will occur. 
