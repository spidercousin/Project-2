# Project 2 - GeoValuate: Optimizing Residential Real Estate Predictions through Machine Learning Models

## Project Statement
The real estate market is characterized by pricing volatility influenced by economic conditions, market demand, and localized factors such as neighborhood desirability, school districts, and proximity to amenities. Additionally, geographical attributes like climate, urban density, and regional economic trends significantly impact property pricing and the time required to sell a home.

In response to these challenges, the objective of this project is to develop an AI-powered solution that leverages historical housing market data from the RentCast API to predict housing prices based on information input by users such as desired real estate location and housing attributes. By training a machine learning model with extensive historical data, the project aims to provide buyers and sellers with actionable insights into optimal listing and offer prices. This solution will empower users to make informed decisions aligned with their selling or purchasing goals, enhancing transparency and efficiency in the housing market.

## GeoValuate

GeoValuate is an AI-powered solution designed to revolutionize how buyers and sellers interact with the housing market. Combining advanced machine learning with rich historical data from the RentCast API, GeoValuate predicts housing prices and market performance with exceptional accuracy. GeoValuate is an application designed to evaluate how various factors impact real estate pricing in patterns in different geographical locations. The application relies on historical housing sales data from [ATTOM](https://www.attomdata.com/), [RentCast](https://developers.rentcast.io/reference/value-estimate), [Zillow](https://www.zillowgroup.com/developers/api/zestimate/zestimates-api/), and [Google Places](https://developers.google.com/maps/documentation/places/web-service/overview).

By evaluating factors like property features, neighborhood characteristics, and localized economic conditions, GeoValuate offers tailored guidance on listing and offer prices. It also accounts for broader influences such as seasonal trends and regional market dynamics, enabling users to respond strategically to market volatility.

GeoValuate’s intuitive design and insightful recommendations empower users to make data-driven decisions, whether they aim to sell at the highest possible price or buy a home that aligns with their budget and goals. Its focus on clarity and precision makes GeoValuate an essential navigator in the ever-changing real estate landscape.

## Programming Language and Technology
GeoValuate is written in [Python](https://www.python.org/) using [Visual Studio Code](https://code.visualstudio.com/) and the [JSON](https://www.json.org/json-en.html) data interchange format.

Visualizations are provided through the use of [Matplotlib](https://matplotlib.org/) and [Shapley](https://shap.readthedocs.io/en/latest/example_notebooks/overviews/An%20introduction%20to%20explainable%20AI%20with%20Shapley%20values.html).

Real estate statistics and analysis information were retrieved from [ATTOM](https://www.attomdata.com/), [RentCast](https://developers.rentcast.io/reference/value-estimate), [Zillow](https://www.zillowgroup.com/developers/api/zestimate/zestimates-api/), and geographical information was retrieved from [Google Places](https://developers.google.com/maps/documentation/places/web-service/overview). 

The [Pandas](https://pandas.pydata.org/) and [Numpy](https://numpy.org/) libraries were used to work with the historical real estate and geographical data retrieved from [Google Places](https://developers.google.com/maps/documentation/places/web-service/overview).

## Installation Guide

The contents of the repository should be placed into the desired folder on the user's computer, being sure to maintain the directory structure. 

The application was developed using Python version 3.12.4. Other versions of Python may work, but no guarantee is made. We suggest using a new virtual environment with the correct version of Python.

The following Python packages must be installed to run the application locally:

* Matplotlib
* Numpy
* Pandas
* Jupyterlab (only if the .ipynb file is used. running the .py file does not require Jupyterlab)

These packages may be individually installed into the environment of your choice. You will also need to obtain an API key for the RentCast API and store it as RENTCAST_API_Key in a file named local_keys.env. Alternatively, you may enter your RentCast API key into the code manually, if desired. 

**Project Goals:** 
  1. Make a prediction model that will help determine the best pricing and the best time to buy or sell a home within any given market.
  2. Develop a user interface for the user to input information specific to the housing market they are interested in exploring.
  
**Impacts on Goal:**
  1. Geographic Location
  2. Job Industry
  3. Crime Rates
  4. Interest Rates
  5. Property Taxes
  6. School Rankings
  7. Leisure Activities
  8. Zip Code

## Initial Research Questions

Here are some initial research questions aligned with the project, including a focus on how various factors influence housing pricing and market dynamics:

**Impact of Location and Amenities:**

- How does proximity to schools, attractions, and public transportation impact housing prices?
- What is the relationship between the quality of local schools and the average days a property stays on the market?
- How do neighborhood characteristics, such as crime rates and walkability, influence listing and offer prices?

**Economic and Tax Impacts:**

- How do local property taxes and tax incentives affect housing pricing trends?
- What role do regional economic factors, such as employment rates and average income levels, play in housing market dynamics?

**Temporal and Seasonal Trends:**

- How do seasonal trends and economic cycles influence housing prices and time on the market?
- Are there specific months or quarters where homes are more likely to sell faster or at higher prices?

**Market Dynamics and Competition:**

- How do supply and demand imbalances (e.g., number of homes for sale versus buyers) affect pricing accuracy and days on the market?
- What patterns emerge in bidding wars or underpriced listings and their effect on the market?

**Custom Attributes Analysis:**

- What specific real estate attributes (e.g., number of bedrooms, square footage, lot size) have the strongest predictive value for housing prices?
- How do unique features such as energy-efficient systems or smart home technology impact pricing and marketability?

**Geographical Influences:**

- How do geographical attributes such as climate, coastal proximity, and urban versus rural settings influence pricing models?
- Are there regional differences in housing price volatility, and how do these differences impact the predictability of selling prices and market durations?

These questions aim to guide the data exploration and model development process, ensuring the project addresses key factors influencing the real estate market.

## Project Roadmap:
  1. Get APIs and information on all the "Impact on goals."
  2. Pull in APIs, clean, and transform them into readable information for Machine Learning model.
  3. Write out step by step how Step 2 was done in the remarks on the Jupyter file.
  4. Export clean data in CSV to Machine Learning model.
  5. Run an accuracy report on each model to determine which model should be used for the deliverable.
  6. Pick and optimize the best model for UI implementation.
  7. Prompt users to input information.

## Data Model Implementation - Create Jupyter Notebook for Cleaning and Transformation Process 

**Create a Jupyter Notebook that Contains the Data Transformation Process and Convert it to a CSV File.**
- How did we clean it and how did we train it?
   
## Data Model Optimization

**Discuss the model optimization and evaluation process showing iterative changes made to the model and the resulting changes in model performance by documenting it in either a CSV/Excel table or in the Python script itself.**
- Data Collection Process
- Data Cleanup Process
- Data Normalization Process
- Data Exploration Process
- Description of How We Evaluated the Trained Model(s) Using Testing Data
- The Approach We Took in Achieving the Project Goals

## Data Sources

For Property Data:
  - ATTOM API: [ATTOM](https://api.gateway.attomdata.com/propertyapi/v1.0.0/property/)
  - RentCast API: [RentCast API](https://developers.rentcast.io/reference/value-estimate)
  - Zillow API: [Zillow](https://www.zillowgroup.com/developers/api/zestimate/zestimates-api/)

For Geolocation:
  - Google Places API: [Google Places](https://developers.google.com/maps/documentation/places/web-service/overview)

## Initial Visualization Goals

**Housing Price Prediction**

Graph Type: Line graph or scatter plot displaying the projected days to sell at various price points.

## Results and Conclusions of the Application or Analysis

The preliminary findings showed that the XGBoost, LGBM Regressor, and Gradient Boosting Regressor models performed significantly better than the linear regression models and other models when predicting housing prices. The feature elimination process did not cause the models to perform better in most instances. There was a slight improvement in performance when the 
longitude feature was dropped from the XGBoost model following a number of other features being dropped. From the analysis of the various models, square footage appeared to be the most accurate predictor of housing prices.

## Example Implementation

The code is designed to predict housing pricing based on user inputs and various regional factors. Here is an example implementation.
- Utah Real Estate Predictor: [Sample Prediction Application](https://github.com/hollidaydds/UtahRealEstatePredictor)

<table>
  <tr>
    <td align="center">
      <img src="https://github.com/spidercousin/Project-2/blob/main/Assets/images/image.png" alt="Image description" width="380">
      <br/>      
      <strong>Landing Page</strong>
    </td>
    <td align="center">
      <img src="https://github.com/spidercousin/Project-2/blob/main/Assets/images/image%20(1).png" alt="Image description" width="350">
      <br/>
      <strong>Prediction Page</strong>
    </td>
  </tr>
</table>


## Future Work and Visualizations 

Future work and/or recommended enhancements to this project include:
- Could we further improve the models?
- Our original problem statement that we would like to pursue is how price impacts day on market. So a user would input a price and we would estimate the amount of time it would take to sell.
- We would like to improve upon the sample application to be more user friendly and provide better predictions.

## Link to Presentation
[Presentation Slides](https://www.canva.com/design/DAGY1nsZbv8/1nZlyLxf3r5BfHs5uhu4WA/view?utm_content=DAGY1nsZbv8&utm_campaign=designshare&utm_medium=link&utm_source=editor)

## Contributors
* [Keri Alexander](https://github.com/kerialexander)
* [JD](https://github.com/spidercousin)
* [Ian Hale](https://github.com/hollidaydds)
* [Reis Hymer](https://github.com/Doobles1989)
* [Carson Jones](https://github.com/Deadbones267)
