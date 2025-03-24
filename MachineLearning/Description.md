# Description of folder MachineLearning


## `energydata_complete.xlsx`
The data set is at 10 min for about 4.5 months. 
The house temperature and humidity conditions were monitored with a ZigBee wireless sensor network. 
Each wireless node transmitted the temperature and humidity conditions around 3.3 min. 
Then, the wireless data was averaged for 10 minutes periods. 
The energy data was logged every 10 minutes with m-bus energy meters. 
Weather from the nearest airport weather station (Chievres Airport, Belgium) was downloaded
from a public data set from Reliable Prognosis (rp5.ru), 
and merged together with the experimental data sets using the date and time column. 
Two random variables have been included in the data set for testing the regression models 
and to filter out non predictive attributes (parameters).

## `FRED_US_GDP_Quarterly.csv`
BEA Account Code: A191RC
Gross domestic product (GDP), the featured measure of U.S. output, is the market value of the goods and services
produced by labor and property located in the United States.For more information, see the Guide to the
National Income and Product Accounts of the United States (NIPA) and the Bureau of Economic Analysis.

## `CPI_USD_Quarterly.csv`
The Consumer Price Index for All Urban Consumers: All Items (CPIAUCSL) is a price index of a basket of goods 
and services paid by urban consumers. Percent changes in the price index measure the inflation rate between a
ny two time periods. The most common inflation metric is the percent change from one year ago. 
It can also represent the buying habits of urban consumers. This particular index includes roughly 88 percent 
of the total population, accounting for wage earners, clerical workers, technical workers, self-employed, 
short-term workers, unemployed, retirees, and those not in the labor force.
The CPIs are based on prices for food, clothing, shelter, and fuels; transportation fares; service fees 
(e.g., water and sewer service); and sales taxes. Prices are collected monthly from about 4,000 housing 
units and approximately 26,000 retail establishments across 87 urban areas.


## `winequality-red.csv` and `winequality-white.csv`
Two datasets are included, related to red and white vinho verde wine samples, from the north of Portugal. 
The goal is to model wine quality based on physicochemical tests
(see [Cortez et al., 2009], http://www3.dsi.uminho.pt/pcortez/wine/).
The two datasets are related to red and white variants of the Portuguese "Vinho Verde" wine.
For more details, consult: http://www.vinhoverde.pt/en/ or the reference [Cortez et al., 2009].
Due to privacy and logistic issues, only physicochemical (inputs) and sensory (the output) variables 
are available (e.g. there is no data about grape types, wine brand, wine selling price, etc.).
These datasets can be viewed as classification or regression tasks.
The classes are ordered and not balanced (e.g. there are munch more normal wines than
excellent or poor ones). Outlier detection algorithms could be used to detect the few excellent
or poor wines. Also, we are not sure if all input variables are relevant. So
it could be interesting to test feature selection methods. 

## `breast_cancer_wisconsin_merge.csv`
Features are computed from a digitized image of a fine needle aspirate (FNA) of a breast mass.
They describe characteristics of the cell nuclei present in the image. 
A few of the images can be found at http://www.cs.wisc.edu/~street/images/
Separating plane described above was obtained using Multisurface Method-Tree (MSM-T) 
[K. P. Bennett, "Decision Tree Construction Via Linear Programming." Proceedings of the 4th Midwest Artificial 
Intelligence and Cognitive Science Society, pp. 97-101, 1992], a classification method which uses linear 
programming to construct a decision tree.  Relevant features were selected using an exhaustive 
search in the space of 1-4 features and 1-3 separating planes.
