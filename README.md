# World Equity Happiness Fund

In this project we are 

A fund manager is interested in building a Happiness Investment Porfolio made up of index funds, weighted by their overall rank in the World Happiness Report. 

This analysis will use the World Happiness Report and Global Market Data for country based etfs.

Use a global index as a benchmark to compare against the new portfolio. 

The application will use historic data to look for trends in the happiness index?

How often is the report updated?

# What's in this folder?

global_market_data_etfs.ipynb - API connection to the list of available etfs through the Global Market Data API

global_market_data_api.ipynb - API pull for chosen etfs in variable ```etf_list``` and creation of pkl file to be used in the main_notebook

world_happiness.ipynb

main_notebook

NOTE - CREATE RESOURCES FILE FOR TIDY UP AND CHECK ALL LINKS REMAIN IN TACT - E.G. PKL FILE CREATE AND SEND TO RESOURCES


# Technologies 

This project was built using python 3.7 with the following libraries:

Pandas
Pickle
Replace?? Check library name - functools?
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

# Presentation Requirements

Each project group will prepare a formal, 10-minute presentation that covers:

An executive summary/overview of the project and project goals.

Be sure to explain how this project relates to FinTech and Financial Programming.
Data Collection, Cleanup & Exploration

Describe the source of your data and why you chose it for your project.

Describe the collection, exploration, and cleanup process.

The approach that your group took in achieving the project goals.

Include any relevant code or demonstrations of the financial application or analysis.

Discuss any unanticipated insights or problems that arose and how you resolved them.

The results/conclusions of the financial application or analysis.

Be sure to include relevant images or examples to support your work.

If the project goal was not achieved, talk about the issues and what was attempted to resolve the issues.

Next Steps.

Take a moment to discuss potential next steps for the project.

Discuss any additional questions that came up that you didn't have time to answer: if you had more weeks to work on your project, what would you research next?

# Contributors 

# License

MIT
