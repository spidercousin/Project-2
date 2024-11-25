# Project Housing Prediction Sales Analysis Alpha - 2

## Project Statement
The real estate market is characterized by pricing volatility influenced by economic conditions, market demand, and localized factors such as neighborhood desirability, school districts, and proximity to amenities. Additionally, geographical attributes like climate, urban density, and regional economic trends significantly impact property pricing and the time required to sell a home.

In response to these challenges, the objective of this project is to develop an AI-powered solution that leverages historical housing market data from the ATTOM API to predict housing prices based on user-inputted real estate and housing attributes. By training a machine learning model with extensive historical data, the project aims to provide buyers and sellers with actionable insights into optimal listing and offer prices. This solution will empower users to make informed decisions aligned with their selling or purchasing goals, enhancing transparency and efficiency in the housing market.

## The Housing Prediction Sales Analysis Tool
The Housing Prediction Sales Analysis Tool is an application designed to evaluate how various factors impact real estate pricing in patterns in various locations impact energy consumption. The application relies on historical housing sales data from [ATTOM] (https://www.attomdata.com/) and historical geographical data from [Need Source Here](https://www.)

## Programming Language and Technology
The Housing Prediction Analysis Tool is written in [Python](https://www.python.org/) using [Visual Studio Code](https://code.visualstudio.com/) and the [JSON](https://www.json.org/json-en.html) data interchange format.

Visualizations are provided through the use of [Matplotlib](https://matplotlib.org/) and [Prophet](https://pypi.org/project/prophet/).

Energy statistics and analysis information were retrieved from [EIA](https://www.eia.gov/opendata/browser/) and weather information was retrieved from [Open-Meteo](https://open-meteo.com/en/docs/historical-weather-api).

The [Pandas](https://pandas.pydata.org/) and [Numpy](https://numpy.org/) libraries were used to work with the historical real estate and geographical data retrieved from the [U.S. Energy Information Administration] (https://api.gateway.attomdata.com/propertyapi/v1.0.0/property/) and [Geoapify](https://www.geoapify.com/) APIs.

## Installation Guide

The contents of the repository should be placed into the desired folder on the user's computer, being sure to maintain the directory structure. 

The application was developed using Python version 3.12.4. Other versions of Python may work, but no guarantee is made. We suggest using a new virtual environment with the correct version of Python.

The following Python packages must be installed to run the application locally:

* matplotlib
* numpy
* pandas
* prophet
* jupyterlab (only if the .ipynb file is used. running the .py file does not require jupyterlab)

These packages may be individually installed into the environment of your choice. You will also need to obtain an API key for the ATTOM API and store it as ATTOM_API_Key in a file named local_keys.env. Alternatively, you may enter your ATTOM API key into the code manually, if desired. Additionally, you will need to obtain an API key from Geoapify and store it in your local_keys.env file as geo.

**Project Goals:** 
  1. Make a prediction model that will help determine the best pricing and the best time to buy or sell a home within any given market.
  2. Develop a user interface for the user to input information specific to the housing market they are interested in exploring.
  
**Impacts on Goal:**
  1. Geo-location
  2. Job industry
  3. Crime rates
  4. Intrest rate
  5. Property taxes
  6. Schools
  7. Leisure activities

  ## Initial Research Questions

Here are some initial research questions aligned with the project, including a focus on how various factors influence housing pricing and market dynamics:

-Impact of Location and Amenities:

How do proximity to schools, attractions, and public transportation impact housing prices?
What is the relationship between the quality of local schools and the average days a property stays on the market?
How do neighborhood characteristics, such as crime rates and walkability, influence listing and offer prices?
Economic and Tax Impacts:

-How do local property taxes and tax incentives affect housing pricing trends?
What role do regional economic factors, such as employment rates and average income levels, play in housing market dynamics?
Temporal and Seasonal Trends:

-How do seasonal trends and economic cycles influence housing prices and time on the market?
Are there specific months or quarters where homes are more likely to sell faster or at higher prices?
Market Dynamics and Competition:

-How do supply and demand imbalances (e.g., number of homes for sale versus buyers) affect pricing accuracy and days on the market?
What patterns emerge in bidding wars or underpriced listings and their effect on the market?
Custom Attributes Analysis:

-What specific real estate attributes (e.g., number of bedrooms, square footage, lot size) have the strongest predictive value for housing prices?
How do unique features such as energy-efficient systems or smart home technology impact pricing and marketability?
Geographical Influences:

-How do geographical attributes such as climate, coastal proximity, and urban versus rural settings influence pricing models?
Are there regional differences in housing price volatility, and how do these differences impact the predictability of selling prices and market durations?

These questions aim to guide the data exploration and model development process, ensuring the project addresses key factors influencing the real estate market.

## Project Roadmap:
  1. Get APIs and information on all the "Impact on goals."
  2. Pull in APIs, clean and transform them into readable information for ML model.
  3. Write out step by step how step 2 was done in the remarks on the jupyter file.
  4. Export clean data in CSV to ML model.
  5. Run accuracy report on each model to determine which model should be used for the deliverable.
  6. Pick and optimize the best model for UI implementation.
  7. Prompt user to input information
      Area Code
      Schools

## Data Model Implementation - Create jupyter notebook for cleaning and transformation process (25 Points)

 1. **Create a Jupyter notebook that contains the data transformation process and convert it to a csv file.**
   How did we clean it and how did we train it
   
## Data Model Optimization (25 Points)
1. **Discuss the model optimization and evaluation process showing iteragitve changes made to the model and the resulting changes in model performance by documenting it in either a CSV/Excel table or in the Python script itself.**
- Data Collection Process
- Data Cleanup Process
- Data Exploration Process
- Description of How we Evaluated the Trained Model(s) Using Testing Data
- The Approach we Took in Achieving the Project Goals

  
## Data Sources

For Property Data:
  - ATTOM API: [ATTOM](https://api.gateway.attomdata.com/propertyapi/v1.0.0/property/)

For Geolocation:
  - Geoapify API: [https://www.geoapify.com/]

## Initial Visualization Goals

**Housing Price Prediction**

Graph Type: Line graph or scatter plot displaying the projected days to sell at various price points.

## Results and Conclusions of the Application or Analysis
NEED TO UPDATE THIS

## Application Output Examples

The code is designed to predict housing pricing based on user inputs and various regional factors. The sample output for this visualization will look like the following plot:
![image](https://NEED TO UPDATE THIS)

Additionally, the code is designed to run a Prophet model based on the 5-year historical trend to predict average days on market for various housing pricepoints. The sample Prophet model output looks like this:

![image](https://NEED TO UPDATE THIS)

## Future Work and Visualizations

Future work and/or recommended enhancements to this project include:
- Any additional questions that surfaced
- What our group might research next if more time was available
- A plan for future development

**NEED TO UPDATE THIS.**

Graph Type: NEED TO UPDATE THIS

## Link to Presentation
https://www.canva.com/design/NEED TO UPDATE THIS

## Contributors
* [Keri Alexander](https://github.com/kerialexander)
* [JD](https://github.com/spidercousin)
* [Ian Hale](https://github.com/hollidaydds)
* [Reis Hymer](https://github.com/Doobles1989)
* [Carson Jones](https://github.com/Deadbones267)
