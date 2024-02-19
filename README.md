# 7_Project 1 Life Expectancy

## Dataset:
Life Expectancy (WHO)
The dataset was downloaded from Kaggle, organized by KUMARRAJARSH to explore on factors influencing life expectancy.
- [Life Expectancy WHO Dataset](https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who/data)
- 2939 rows, 22 columns including the header

 ## Data Cleaning 
 
 There are total of 193 countries, and we have filtered out 11 places that were missing major data. 

![Country_1_year](https://github.com/vanillatyy1/7_Project_1_part/raw/80a229799078dc80f69ce42895370dab2c11a6f5/Screenshots/Country_1_year.jpg)
 
 ## Data Limitation

The dataset covers the year 2000 to 2015, excluding recent events like the global COVID-19 pandemic, which has significant impact on health infrastructure worldwide. 
Looking into the columns, we noticed missing data of 41 countries, including nations like the USA, UK, and New Zealand, posing a notable limitation. While merging with another dataset might fill the gap, population can be influenced by factors like immigration, which add complexity and potential distortions when analyzing its relationship with life expectancy.

Nonetheless, even though the dataset provides alcohol consumption data recorded per capita for aged 15+, its scope is limited to the volume of pure alcohol consumed. This restricts the ability to establish meaningful correlations between alcohol consumption and life expectancy. Further research incorporating variables such as the type of alcohol consumed, like red wine, beer, hard liquor, or the context of consumption, like social occasions and cultural practices may yield better insights into this relationship. 

![Data_Limitation_screen](https://github.com/vanillatyy1/7_Project_1_part/raw/80a229799078dc80f69ce42895370dab2c11a6f5/Screenshots/Data_Limitation_screen.jpg)

## Research Question 1: On average, do people in developed or developing countries live longer?

The purpose of the analysis is to see if developed and developing countries have different life expectancy.
The Jupyter Notebook file related to this part of the analysis is: country_status_vs_life_expect.ipynb.

In our findings, we observe that people in developed countries tend to live longer than those in developing countries. 
Developed nations: 77 to 80 years
Developing nations: 65 to 70 years 
We also note a positive trend of increasing life expectancy over the years in both Developed and developing countries. 

### Top 5 v.s. Bottom 5

| Country                 | Country_status | Avg. Population | Avg. Life Expectancy | Adult Mortality Rates | Avg. Infant Deaths |
|-------------------------|----------------|-----------------|----------------------|-----------------------|---------------------|
| Japan                   | Developed      | 97,384          | 82.53750             | 57.1250               | 2.8750              |
| Sweden                  | Developed      | 5,514,868       | 82.51875             | 59.1875               | 0.0000              |
| Iceland                 | Developed      | 186,178         | 82.44375             | 49.3750               | 0.0000              |
| Switzerland             | Developed      | 5,913,242       | 82.33125             | 55.7500               | 0.0000              |
| France                  | Developing     | 27,581,733      | 82.21875             | 73.1250               | 2.9375              |
| ...                     | ...            | ...             | ...                  | ...                   | ...                 |
| Malawi                  | Developing     | 6,700,263       | 49.89375             | 424.4375              | 37.1250             |
| Angola                  | Developing     | 10,147,099      | 49.01875             | 328.5625              | 83.7500             |
| Lesotho                 | Developing     | 1,200,528       | 48.78125             | 550.0625              | 4.5000              |
| Central African Republic| Developing     | 2,016,546       | 48.51250             | 333.0625              | 16.5000             |
| Sierra Leone            | Developing     | 3,336,265       | 46.11250             | 357.8125              | 27.5625             |

In fact, the top five and bottom five countries in terms of average life expectancies reveals a sharp contrast of nearly forty years. 
While developed nations like Japan and Sweden boast life expectancies surpassing eighty-two years, the bottom five countries, all of which are developing nations, see life expectancies plummet to as low as 46 - 49 years.

This drastic contrast underscores the profound disproportion in healthcare access and quality between developed and developing nations. 

## External factors: Developed v.s. Developing Countries
![PESTEL_Full](https://github.com/vanillatyy1/7_Project_1_part/raw/80a229799078dc80f69ce42895370dab2c11a6f5/Screenshots/PESTEL_Full.jpg)


