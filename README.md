# Zillow Housing Time Series Market Analysis Phase-4-project
![Alt text](<timepic.png>)

## Moringa Phase 4 Project Submission

#### GROUP 4:

- Student name: Kenneth Karanja
- Student name: Pete Njagi
- Student name: James Koli (Group Leader)
- Student name: Tom Mwabire
- Student name: Paul Mwangi
- Student name: Lee Ndung'u
- Student name: Edwin Mwenda

Scheduled project review date/time: April 12th 2024
# Forecasting Housing Market Trends for Real Estate Investment Strategy
![Alt text](<zillow.png>)

#### Important Project Files:

1. Group4.ipynb (Main Jupyter document)
2. Presentation.pdf (Presentation)
3. zillow_data.csv (Main Data)
4. Optional Project Pdf

## Business Problem

The primary business problem is the lack of visibility and understanding of the US housing market among Kenyan investors. Additionally, there is a need to identify regions that offer promising investment opportunities within the low-cost housing segment. Another challenge is ensuring the accuracy and relevance of predictions amidst periods of market instability, such as the 2008 housing market crash. Therefore, the project aims to address these challenges by providing comprehensive data analysis and forecasting to guide investment decisions effectively.

## Overview

Our client, a distinguished real estate investment firm based in Kenya, is dedicated to facilitating Kenyan investors' access to the thriving US housing market. Specializing in low-cost housing investments, they cater to the needs of local Kenyans and diaspora members looking to diversify their investment portfolios. Through rigorous data analysis and strategic insights, the firm empowers investors with the knowledge required to navigate the complexities of the US real estate market successfully. By democratizing access to wealth-building opportunities and fostering financial inclusion, they contribute to the economic growth and prosperity of Kenya while enabling individuals to secure their financial futures.


## Business Stakeholders

The primary stakeholders for this project include:

- Kenyans looking to invest in the US housing market
- Kenyan diaspora planning to buy or rent properties in the USA
- Real estate investment firms
- Financial analysts focusing on real estate investments
- Policy makers interested in foreign investments

This project seeks to empower our stakeholders with precise forecasts and strategic insights into the US real estate market, facilitating optimal investment decisions.

## Business Objective

Our key objectives are:

- Developing an accurate time series forecasting model using Zillow data.
- Providing market trend analysis to identify promising investment opportunities.
- Offering actionable investment strategies based on model insights.
- Enhancing the decision-making process for buyers, renters, and investors.
- Strengthening the investment portfolio of our clients through data-driven insights.

Through this initiative, we aim to bridge the gap between Kenyan investors and the US real estate market, ensuring lucrative and informed investment choices.

# Data Understanding

The data source for our analysis is primarily the `zillow_data.csv` file, which encompasses historical housing price data across various US regions. 

#### `zillow_data.csv` (Main data source)
* **Source**: Zillow's publicly available dataset.
* **Contents**: This dataset includes monthly housing prices across different US regions, spanning from April 1996 to April 2018. It covers details such as region name, city, state, metro area, and county, alongside the housing prices for each month.

Our analysis will focus on understanding the trends, patterns, and factors influencing these housing prices, thereby enabling us to forecast future market trends effectively.

#### Univariate Analysis
**Housing Prices in USD = unit of analysis**

**Unique identifiers:**
- RegionID
- RegionName (ZIP code)
- City
- State
- Metro
- CountyName
- SizeRank

### Data Visualizations
<img src="/images/1.png" alt="drawing" width="500"/>

The graph shows property counts by county. Maricopa, Los Angeles, and Jefferson top the list. Middlesex, Jackson, and Harris follow closely. Cook, Montgomery, Washington, and Orange also have significant counts. Counts range from around 200 to over 250

<img src="/images/2.png" alt="drawing" width="500"/>

The graph displays property counts by state. California (CA) has the highest count. New York (NY) and Texas (TX) follow closely. Pennsylvania (PA), Florida (FL), and Ohio (OH) also have substantial counts. Illinois (IL), New Jersey (NJ), Michigan (MI), and Indiana (IN) complete the list

<img src="/images/3.png" alt="drawing" width="500"/>

The graph shows ROI of property in the top 10 states. DC, HI, and CA have the highest ROI. Other states, like SD, CO, and MA, also show significant ROI. NY, WA, VT, and FL complete the list with varying ROI levels

<img src="/images/4.png" alt="drawing" width="500"/>

The scatter plot illustrates ROI against the top 10 states. CA, NY, and TX exhibit the highest ROIs. PA, FL, and OH also show notable ROIs. Additionally, IL, NJ, MI, and IN complete the list, each with varying ROI levels.

<img src="/images/5.png" alt="drawing" width="500"/>

The scatter plot demonstrates ROI against the top 10 counties. Los Angeles, Jefferson, and Orange counties exhibit the highest ROIs. Washington, Montgomery, and Cook also show notable ROIs. Additionally, Harris, Jackson, Middlesex, and Maricopa complete the list, each with varying ROI levels.

### ARIMA & Modelling

![image](https://github.com/PeteZDj/Phase-4-Group-Project/assets/151729172/399a3b3a-fd0b-4370-b811-9a2e926058b7)


To meet the normality assumptions, the residuals must not be correlated and have a normal distribution. For this case:

The residuals are normally distributed because, as the qq-plot on the bottom left illustrates, they follow a linear trend line.
There are minimal correlations with their lagged version, as indicated by the correlogram plot on the bottom left. This indicates that our series doesn't exhibit any clear seasonality.
The residuals are positively distributed, as indicated by the bell curve on the histogram.

## Testing the model's performance

![image](https://github.com/PeteZDj/Phase-4-Group-Project/assets/151729172/23b8bc09-b7b3-4dda-95ee-3f4442581336)

The testing forecasting model performance graph above illustrates the accuracy and reliability of our forecasted returns. By comparing the observed returns (blue line) with the prediction series (red line), we can assess how well our model captures the underlying patterns and trends in the data. The close alignment between the two lines indicates that our forecasting model effectively captures the dynamics of the time series data, suggesting its robust performance in predicting future returns.

### Model Evaluation

![image](https://github.com/PeteZDj/Phase-4-Group-Project/assets/151729172/cd92e879-8502-4ed5-a414-12116fdab11f)

The forecasted values (depicted by the red line) in the graph above show a consistent trend in home price movements over time, aligning closely with the actual observed values (represented by the blue line). This indicates the model's effectiveness in capturing the underlying patterns in the data, providing valuable insights for stakeholders. Such accurate forecasts are crucial for making informed decisions regarding investments or understanding market trends within the 85035 area.

### Conclusion & Recommendations

![image](https://github.com/PeteZDj/Phase-4-Group-Project/assets/151729172/46ee45ee-9b5b-472f-abc7-af877223a43c) 

With the exception of the 85035 zipcode; every zipcode has an encouraging projected price because they are all in the green.

We can determine our top five recommendations and their anticipated return on investment after three years based on the graph above.

Zip code 94804: This area's housing prices have been steadily rising, and a high return on investment is expected. Its stable market dynamics and favourable price trends make it a good fit for our client's investment portfolio.

Zip code 75217 With its promising combination of affordability and appreciation potential, this area represents an excellent opportunity for our client. Our analysis shows a positive trajectory in housing prices, indicating a high ROI potential.

Zip code 19143: This zipcode demonstrates resilience in the face of market fluctuations, with consistent growth and promising investment opportunities. Its affordability and upward price trends make it an appealing option for our client looking for long-term returns.

Zip code 60628: This area has strong growth potential despite fluctuations in the overall market, especially in low-cost housing segments. Given the current favourable market conditions and anticipated growth, it is highly recommended for our client's investment plan.

Zip code 48227: This area offers our client an appealing investment opportunity because of its stability in the market and affordability. It has the potential to yield substantial returns over time due to its steady increase in housing prices and bright future prospects.

After that, the investor has the option to invest in any of the zip codes listed above, with the exception of 85035, which offers a negative return on investment.


In conclusion, our thorough examination of the US housing market, with an emphasis on affordable housing investment opportunities, offers our Kenyan real estate investment firm client insightful information. By using rigorous data preprocessing, time series modelling, and exploratory data analysis, we have predicted future results and found encouraging trends for a number of zip codes. Our research showed that although housing prices fluctuated in some areas, they consistently increased in other areas, providing favourable returns on investment.

For example in our case, the zipcode 94804 turned out to be the best suggestion with the highest estimated return on investment. In addition, we were able to formulate well-informed recommendations that were customised to our client's investment goals thanks to our analysis of the dynamics of the housing market, which included price trends, seasonality, and market stability. By using these insights, our client's investment portfolio can be diversified, resources can be wisely allocated to take advantage of profitable opportunities, and returns can be maximised.

In order to maximise long-term profitability and adjust to shifting market conditions, it will be essential to regularly review investment strategies and keep a close eye on market trends. Our client can confidently and precisely navigate the ever-changing US real estate market by incorporating data-driven decision-making processes into their investment strategy, setting themselves up for long-term success and sustainable growth.



