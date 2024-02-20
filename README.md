# VitaBridge Solutions 🌱 
Welcome to VitaBridge Solutions! We're dedicated to unraveling the secrets of longevity through insightful economic and health analyses.

**Co-Founders:** Jasleen, Vanilla, Seethalakshmi

"Fast forward to your best life" ✈️

## Research Questions 🌟
1. On average do developed or developing countries live longer?
2. Do countries with high gdp spend more on health (%) expenditure?
3. Do countries that spend more on health (%) expenditure have less diseases?
4. How do diseases affect longevity?


## Analysis 💡


## Funding Ask 💵
We are looking for $2M in funding which will go to;
- Research and Development (R&D): ($600,000)
- Technology Infrastructure: ($400,000)
- Talent Acquisition and Training: ($300,000)
- Marketing and Outreach: ($500,000)
- Operational Expenses: ($200,000)

## Links 🌐 
- presentation
- dataset 


----------------------------------------------------------------------------------------------------------------------------

# 7_Project 1 Life Expectancy

## Dataset:
Life Expectancy (WHO)
The dataset was downloaded from Kaggle, organized by KUMARRAJARSH to explore on factors influencing life expectancy.
- [Life Expectancy WHO Dataset](https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who/data)
- 2939 rows, 22 columns including the header

 ## Data Cleaning 
 
 There are total of 193 countries, and we have filtered out 11 places that were missing major data. 

![Country_1_year](https://github.com/jazzy-github222/VitaBridge-Solutions/raw/e40246b6faa9ede924cb82261ac5f992340cc984/Screenshots/Country_1_year.jpg)
 
 ## Data Limitation

The dataset covers the year 2000 to 2015, excluding recent events like the global COVID-19 pandemic, which has significant impact on health infrastructure worldwide. 
Looking into the columns, we noticed missing data of 41 countries, including nations like the USA, UK, and New Zealand, posing a notable limitation. While merging with another dataset might fill the gap, population can be influenced by factors like immigration, which add complexity and potential distortions when analyzing its relationship with life expectancy.

Nonetheless, even though the dataset provides alcohol consumption data recorded per capita for aged 15+, its scope is limited to the volume of pure alcohol consumed. This restricts the ability to establish meaningful correlations between alcohol consumption and life expectancy. Further research incorporating variables such as the type of alcohol consumed, like red wine, beer, hard liquor, or the context of consumption, like social occasions and cultural practices may yield better insights into this relationship. 

![Data_Limitation_screen](https://github.com/jazzy-github222/VitaBridge-Solutions/raw/e40246b6faa9ede924cb82261ac5f992340cc984/Screenshots/Data_Limitation_screen.jpg)

## Research Question 1: On average, do people in developed or developing countries live longer?

The purpose of the analysis is to see if developed and developing countries have different life expectancy.
The Jupyter Notebook file related to this part of the analysis is: [country_status_vs_life_expect.ipynb](https://github.com/jazzy-github222/VitaBridge-Solutions/blob/da052162d319e64e0a2040d5c0bad47043ed5cc0/country_status_vs_life_expect.ipynb).

In our findings, we observe that people in developed countries tend to live longer than those in developing countries. 
Developed nations: 77 to 80 years
Developing nations: 65 to 70 years 
We also note a positive trend of increasing life expectancy over the years in both Developed and developing countries. 

![Life_Expect_GrowthByYear_bold](https://github.com/jazzy-github222/VitaBridge-Solutions/raw/e40246b6faa9ede924cb82261ac5f992340cc984/Screenshots/Life_Expect_GrowthByYear_bold.jpg)

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
![PESTEL_Full1](https://github.com/jazzy-github222/VitaBridge-Solutions/raw/e40246b6faa9ede924cb82261ac5f992340cc984/Screenshots/PESTEL_Full1.jpg)

Research Question: Do countries with a higher GDP spend more on the healthcare of their citizens? - Big Picture

Since the dataset is arranged by the 193 countries, over the span of 15 years (2000-2015), we have found the average of the GDP and the percentage expenditure throughout the years to complete the analysis. In order to answer the research question, a scatterplot was used to see the big picture of the data. It was found that there is a positive correlation between a country's GDP and their percentage health expenditure. The data exemplified that as there is more money for a country to spend, there is an increase in the amount spent of healthcare.

Consideration:

With the dataset, there are some considerations to be made. The way in which the data is set up, the percentages for health expenditure are over 100 percent. Since the data is an accumulation over the years, the percentages could be signficantly higher as compared to previous years and therefore is significantly over 100 percent. 

Research Question: Do countries that spend more on healthcare have less disease? - Analyzing immunization rates 

In order to tackle the research question, the dataset was sorted into the countries spending the most and the least on healthcare. When looking at data, we pulled out the immunization rates of the top 5 and bottom 5 countries, and sorted by the percentage expenditure and the immunization rates for Hepatitus B, Diphteria and Polio. Additionally, the life expectancy of each of the ten countries were also added to the table in order to make the comparisons. Through the utilization of a bar graph, we displayed the immunization rates among the top and bottom countries for each of the above-mentioned diseases. The graph demonstrated the consistency in immunization rates for the top countries, and the inconsistent immunization for the bottom countries.

Analysis: 

The top five countries versus the bottom five countries have approximately 20 years of difference when it comes to life expectancy. With the graph depicting the immunization rate, we can see that the higher rates of immunization is directly linked to higher life expectancy. The countries spending less on health still have high rates of immunization, however, the life expectancy is still approximately 20 years less than the top five countries. 
One highlight in the data is that the top 5 countries are also seeing rates of less immunization like Canada and Sweden for Hep. B. A hypothesis that can be made is that these countries may have gotten to a point where these diseases are no longer a threat and therefore immunization is not necessary.  
As immunization is a vital factor to life expectancy but additional factors also need to be considered such as quality of life, diet, availability/access to immunization/medical, environmental factors and variables are also needed to be looked at to see if life expectancy can be increased. In conclusion, we can see that prioritization on immunization of citizens is vital in improving life expectancy and the more consistency in immunization rates significantly improves the life expectancy of the country's citizens.

