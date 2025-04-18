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

## `car.data.csv`
Car Evaluation Database was derived from a simple hierarchical decision model originally developed for 
the demonstration of DEX, M. Bohanec, V. Rajkovic: Expert system for decision making. 
Sistemica 1(1), pp. 145-157, 1990.). The model evaluates whether a car is (unacceptable, acceptable, good, very good).

## `bank-full.csv`
The data is related with direct marketing campaigns (phone calls) of a Portuguese banking institution. 
The classification goal is to predict if the client will subscribe a term deposit (variable y).
bank-full.csv with all examples and 17 inputs, ordered by date (older version of this dataset with less inputs). 
Input variables:
* bank client data:
1 - age (numeric)
2 - job : type of job (categorical: "admin.","unknown","unemployed","management","housemaid","entrepreneur","student",
                                    "blue-collar","self-employed","retired","technician","services") 
3 - marital : marital status (categorical: "married","divorced","single"; note: "divorced" means divorced or widowed)
4 - education (categorical: "unknown","secondary","primary","tertiary")
5 - default: has credit in default? (binary: "yes","no")
6 - balance: average yearly balance, in euros (numeric) 
7 - housing: has housing loan? (binary: "yes","no")
8 - loan: has personal loan? (binary: "yes","no")
* related with the last contact of the current campaign:
9 - contact: contact communication type (categorical: "unknown","telephone","cellular") 
10 - day: last contact day of the month (numeric)
11 - month: last contact month of year (categorical: "jan", "feb", "mar", ..., "nov", "dec")
12 - duration: last contact duration, in seconds (numeric)
* other attributes:
13 - campaign: number of contacts performed during this campaign and for this client (numeric, includes last contact)
14 - pdays: number of days that passed by after the client was last contacted from a previous campaign (numeric, -1 means client was not previously contacted)
15 - previous: number of contacts performed before this campaign and for this client (numeric)
16 - poutcome: outcome of the previous marketing campaign (categorical: "unknown","other","failure","success")

## `bank-additional-full.csv`
This dataset is based on "Bank Marketing" UCI dataset (please check the description at: http://archive.ics.uci.edu/ml/datasets/Bank+Marketing).
The data is enriched by the addition of five new social and economic features/attributes (national wide indicators from a ~10M population country), 
published by the Banco de Portugal and publicly available at: https://www.bportugal.pt/estatisticasweb.
This dataset is almost identical to the one used in [Moro et al., 2014] (it does not include all attributes due to privacy concerns). 
Using the rminer package and R tool (http://cran.r-project.org/web/packages/rminer/), we found that the addition of the five new social and economic 
attributes (made available here) lead to substantial improvement in the prediction of a success, 
even when the duration of the call is not included. Note: the file can be read in R using: d=read.table("bank-additional-full.csv",header=TRUE,sep=";")
* social and economic context attributes
16 - emp.var.rate: employment variation rate - quarterly indicator (numeric)
17 - cons.price.idx: consumer price index - monthly indicator (numeric)     
18 - cons.conf.idx: consumer confidence index - monthly indicator (numeric)     
19 - euribor3m: euribor 3 month rate - daily indicator (numeric)
20 - nr.employed: number of employees - quarterly indicator (numeric)
