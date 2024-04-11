# Zillow Housing Time Series Market Analysis Phase-4-project
![Alt text](<timepic.png>)

## Moringa Phase 4 Project Submission

#### GROUP 4:

- Student name: Kenneth Karanja
- Student name: Pete Njagi
- Student name: James Koli (Group Leader)
- Student name: Tom Mwabire
- Student name: Paul Maina
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

We, a pioneering data science firm based in Kenya named KenyaData Insights, have embarked on an ambitious project commissioned by a local investment firm. Our objective is to leverage historical Zillow housing data to forecast future trends in the US housing market. This endeavor aims to serve Kenyans and the diaspora eyeing opportunities to buy, rent, or invest in US real estate, offering them invaluable insights for informed decision-making.

## Overview

Our analysis will delve into processing and analyzing historical Zillow data to discern meaningful patterns and trends in housing prices across various regions and property types in the USA. We aim to identify key factors influencing housing prices and incorporate them into a sophisticated time series forecasting model. This model will aid in predicting future housing market trends, providing a solid foundation for strategic real estate investment planning.

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

## Hypotheses

i. **Hypothesis on Regional Housing Price Trends:**
   - Null Hypothesis (H0): There is no significant difference in housing price trends across different US regions.
   - Alternative Hypothesis (H1): Housing price trends vary significantly across different US regions.

ii. **Hypothesis on Property Type and Housing Prices:**
   - Null Hypothesis (H0): Housing prices do not significantly differ by property type.
   - Alternative Hypothesis (H1): Different property types exhibit significant variations in housing prices.

iii. **Hypothesis on Economic Indicators and Housing Prices:**
   - Null Hypothesis (H0): Economic indicators do not significantly influence housing prices.
   - Alternative Hypothesis (H1): Housing prices are significantly affected by various economic indicators.

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

## Regression Analysis

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

<img src="/images/6.png" alt="drawing" width="500"/>

<img src="/images/7.png" alt="drawing" width="500"/>

<img src="/Images/NotebookExports/8.png" alt="drawing" width="500"/>


## Setup for Jupyter Notebook

To set up a Jupyter Notebook for analyzing the data:

1. Install Anaconda which includes Jupyter Notebook, Python, and other data science packages. Visit [Anaconda's website](https://www.anaconda.com/products/distribution) and download the installer for your operating system.
2. After installation, launch Anaconda Navigator and start Jupyter Notebook, or open a terminal (or command prompt) and type `jupyter notebook` to start the Jupyter Notebook server.
3. Create a new Python notebook from the Jupyter dashboard.
4. Import the required libraries (e.g., pandas, matplotlib, seaborn, Statsmodels) at the beginning of your notebook.
5. Load your dataset using pandas, for example: `df = pd.read_csv('path_to_your_data.csv')`.
6. Proceed with your data analysis and visualization.

For more detailed instructions, you can refer to the [official Jupyter documentation](https://jupyter.readthedocs.io/en/latest/).
