# The Happy Fund

* An executive summary/overview of the project and project goals.

* Be sure to explain how this project relates to FinTech and Financial Programming.
* Data Collection, Cleanup & Exploration

In this project we are analysing a new investment portfolio, the Happy Fund, based on the scores of countries taken from the [World Happiness Report](https://worldhappiness.report/). We take the role of a fund manager in the early stages of launching a new investment fund. We compare the historic performance of the portfolio against a world equity index and present a decision on whether to progress with the deep analysis for the new portfolio construction. 

We read in CSV downloads for each year of the World Happiness Report and clean the data to filter out only the top 15 countries, by overall score. The data for all years is then joined together to display in one DataFrame.

Through an API, we collect the data for various country based exchange traded funds (ETFs). This data is cleaned to show only the close prices and all of the ETFs are then joined together in one DataFrame.

Using PKL files, we bring the clean data from the World Happiness Report and the ETFs into a single notebook to calculate performace. 

The portfolio is weighted by the Happiness Score of countries at the beginning of each year. The portfolio is then rebalanced annually, based on the updated scores. 

The iShares MSCI World etf is used as a benchmark to compare the portfolio. 

To clearly present the outcomes, we use the growth of $100 as a measure and a chart to illustrate our findings. With an animated plot graph, we show the changes in Happiness scores over the period. 

## Data Issues

*Some of the countries in the top 15 did not have corresponding ETFs through the API we were using.*
We excluded Iceland, Luxembourg, Costa Rica and Puerto Rico from our data. 

Luxembourg and Puerto Rico only appeared in the top 15 in 2 years. Iceland and Costa Rica are in the top 15 for each year in our dataset and could have a significant impact on the final outcomes.

*The free API is limited to 100 calls.*
We used month end data to limit the calls. The dataset would be more reliable with daily prices.

*The performance is based on historical data.*
We cannot predict the future, however historical trends are a good starting point to analyse the behaviour of an investment.

## Outcomes

INCLUDE SUMMARY AND IMAGES FROM REPORT

## Future releases
Use daily data 
Expand the dataset to include the most recent years
Find ETFs for the missing countries
Research the underlying ETFs and consider alternative investment options 

Monte Carlo?? 
Other investment measures?

Make the performance interactive - be able to change the investment date to rebase the growth of $100

Create a rebalancing tool to automatically re-weight the portfolio each year.

# What's in this folder?

global_market_data_etfs.ipynb - API connection to the list of available etfs through the Global Market Data API

global_market_data_api.ipynb - API pull for chosen etfs in variable ```etf_list``` and creation of pkl file to be used in the main_notebook

world_happiness.ipynb

main_notebook

NOTE - CREATE RESOURCES FILE FOR TIDY UP AND CHECK ALL LINKS REMAIN IN TACT - E.G. PKL FILE CREATE AND SEND TO RESOURCES


# Technologies 

This project was built using python 3.7 with the following libraries:

ADD ALL LINKS AND SHORT EXPLANATION OF EACH 

Pandas
Pickle
functools
Plotly
requests
os
dotenv
json

# Installation Requirements

API for [Global Market Data](https://rapidapi.com/attulab-attulab-default/api/global-market-data/)
Set up free account through RapidAPI and connect to Global Market Data

.env file to hold API key in format:

X-RapidAPI-Key = "insert_key_here"
X-RapidAPI-Host = "insert_host_here"


# Citations

[World Happiness Report](https://www.kaggle.com/datasets/unsdsn/world-happiness)
[Global Market Data](https://rapidapi.com/attulab-attulab-default/api/global-market-data/)


# Contributors 

# License

MIT
