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

## Project Roadmap

  1. Get APIs and information on all the "Impact on goals."
  2. Pull in APIs, clean, and transform them into readable information for Machine Learning model.
  3. Write out step by step how Step 2 was done in the remarks on the Jupyter file.
  4. Export clean data in CSV to Machine Learning model.
  5. Run an accuracy report on each model to determine which model should be used for the deliverable.
  6. Pick and optimize the best model for UI implementation.
  7. Prompt users to input information.

## Data Model Implementation

Our model development process was a structured and iterative effort aimed at achieving the project’s goals through data-driven insights and robust model performance. We began with a comprehensive data collection process, ensuring a rich dataset to support model training. This was followed by a thorough data cleanup process to address inconsistencies, outliers, and missing values, laying the foundation for reliable analysis. The dataset was then transformed through a data normalization process, standardizing variables to ensure consistency and comparability across features. Using data exploration techniques, we uncovered patterns, relationships, and potential biases within the dataset, which informed our model design choices. Once trained, the models were rigorously evaluated using testing data, leveraging metrics to assess accuracy, precision, and other performance indicators. This iterative optimization process, embedded directly within our Python script, allowed us to make incremental improvements to the model and achieve the desired outcomes efficiently and effectively.

***Data Collection Process***

The data collection process presented several challenges due to the limitations of the real estate API. Access to several real estate APIs was restricted to real estate professionals or registered businesses, or the number of API calls allowed was limited, requiring careful prioritization of data requests. Additionally, the dataset obtained from the [RentCast API](https://developers.rentcast.io/reference/value-estimate) had a restricted set of fields with incomplete or inaccurate records. Common issues included null fields, incorrect data entries, and numerical anomalies, such as listings with implausible values (e.g., properties listed with 800+ bathrooms). Another anomaly observed was data indicating houses sold in the future, likely due to misconfigured timestamps. These challenges necessitated extensive preprocessing and validation to ensure the integrity and usability of the data for subsequent model development.

***Data Cleanup and Data Normalization Process***

Our team successfully collaborated to optimize a raw data file exported from the [RentCast API](https://developers.rentcast.io/reference/value-estimate). Key steps included:

- Conducting a comprehensive review of each field to identify inconsistencies, outliers, and anomalies.
- Developing and implementing logic to standardize fields into the correct formats.
- Cleaning the dataset by dropping null values and refining fields to enhance comparability.

This streamlined approach improved the dataset's accuracy and usability, enabling more reliable analysis and insights.

***Data Exploration Process***

Following data collection and cleanup, the initial data exploration process focused on understanding the dataset’s structure, identifying patterns, and uncovering insights that could guide model development. The team began by examining the distribution of key variables, such as property prices, sizes, and days on market, to identify trends and potential outliers. Correlation analysis was conducted to understand relationships between features and their potential predictive power. Visualization tools, such as scatter plots, and heatmaps, were employed to uncover underlying patterns and detect anomalies that might affect model performance. The team also conducted a preliminary evaluation of missing data handling, ensuring that imputation or exclusion methods applied during cleanup did not introduce bias. This exploratory phase provided critical insights into the data’s characteristics, informed feature selection, and highlighted areas for further refinement to optimize the model-building process.

***Model Training and Evaluation Process***

To evaluate the performance of our models, we adopted a structured process that ensured fairness and reliability in testing. First, the dataset was split into separate training and testing sets to prevent data leakage and provide an unbiased evaluation. The models were trained exclusively on the training dataset, ensuring that the testing data remained unseen during the training phase. Once the models were trained, they were used to generate predictions on the testing data. These predictions were then compared against the actual target values to assess their accuracy. Evaluation metrics, such as R² and mean squared error (MSE), were calculated to quantify the models’ performance, capturing both the overall fit and prediction accuracy. This iterative evaluation process provided critical feedback, allowing us to refine and optimize the models for better predictive accuracy and reliability.

## Data Model Optimization

***Approach to Model Development***

Our approach to model development was a collaborative and iterative process aimed at optimizing performance and ensuring the best possible results. Each team member independently developed individual models, experimenting with different algorithms, hyperparameters, and feature sets. After the initial model creation phase, the team convened to discuss and compare the performance of these models, using predefined evaluation metrics such as R², mean squared error (MSE), and other relevant indicators. Based on this feedback, we collaboratively refined our models, incorporating shared insights and addressing identified weaknesses. The results of each iteration were meticulously documented directly within the Python scripts, enabling us to track changes in model performance over time. Ultimately, the best-performing models were selected based on their overall performance, balancing accuracy, robustness, and generalizability to achieve our project objectives.

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

In future iterations of the application, the team aims to enhance the user experience and provide more insightful analytics by incorporating additional features and visualizations. One key enhancement is the integration of advanced search features, such as school rankings and proximity to amenities, allowing users to tailor their property searches to specific preferences. Another priority is the addition of a dynamic feature enabling users to estimate the days on market at various price points. This functionality will empower users to make informed decisions by providing insights into how pricing impacts the time it takes to sell a property. Furthermore, we aim to refine our predictive models, improving accuracy and reliability to ensure better support for user decision-making. Expanding on the original problem statement, the team envisions creating an interactive tool where users can input a price and receive an estimated timeline for selling their property. These advancements will be coupled with improvements to the application’s user interface, ensuring a seamless and intuitive experience that aligns with the project’s goals of delivering actionable, data-driven insights.

## Link to Presentation
[Presentation Slides](https://www.canva.com/design/DAGY1nsZbv8/1nZlyLxf3r5BfHs5uhu4WA/view?utm_content=DAGY1nsZbv8&utm_campaign=designshare&utm_medium=link&utm_source=editor)

## Data Sources

For Property Data:
  - ATTOM API: [ATTOM](https://api.gateway.attomdata.com/propertyapi/v1.0.0/property/)
  - RentCast API: [RentCast API](https://developers.rentcast.io/reference/value-estimate)
  - Zillow API: [Zillow](https://www.zillowgroup.com/developers/api/zestimate/zestimates-api/)

For Geolocation:
  - Google Places API: [Google Places](https://developers.google.com/maps/documentation/places/web-service/overview)

## Contributors
* [Keri Alexander](https://github.com/kerialexander)
* [JD](https://github.com/spidercousin)
* [Ian Hale](https://github.com/hollidaydds)
* [Reis Hymer](https://github.com/Doobles1989)
* [Carson Jones](https://github.com/Deadbones267)
