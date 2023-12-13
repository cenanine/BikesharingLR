# Bike Sharing Linear Regression Assignment
> A bike-sharing system provides bikes for short-term use, often for a fee or at no cost, allowing users to borrow bikes from computer-controlled docks by entering payment details. These bikes can be returned to any dock within the same system. BoomBikes, a US bike-sharing provider, has faced revenue declines during the Covid-19 pandemic and seeks a sustainable business plan for post-lockdown recovery. They aim to gauge post-quarantine bike-sharing demand nationwide, preparing to meet these needs effectively and differentiate themselves in the market to drive significant profits once the situation improves.
The company wants to know:
Which variables are significant in predicting the demand for shared bikes.
How well those variables describe the bike demands
Our Assignment works on addressing above all, using python. Below are the main steps, we took
Data initialization and understanding
Data Visualization
Data Preparation and Building the Linear Model
Conclusion


## Table of Contents
* [Data initialization and understanding](#data-initialization-and-understanding)
* [Data Visualization](#data-visualization)
* [Build Linear Model](#build-linear-model)
* [Conclusions](#conclusions)
* [Libraries](#libraries)
* [Contact](#contact)


## Data initialization and understanding
- Provide general information about your project here.
- What is the background of your project?
- What is the business probem that your project is trying to solve?
- What is the dataset that is being used?

## data-visualization
- Visualize the data for Categorical and numerical variables
- check the corelation and also the heat map for all the variables
- Analyze the pattern of there's any

## Build Linear Model
- Build the dummy variables for the categoricals variables
- Divide the data into Train and Test sets
- Build the initial model using RFE
- Recursively build the model by manually removing the features until we get the best model

## Conclusions
- We can come up with below equation for the best fitting line to Bike Sharing linear model from the above Coefficient
cnt = 0.1344 + 0.2328 * yr + -0.1067 * holiday + 0.5471 * temp + -0.1531 * windspeed + 0.0994 * mnth_sep + -0.0498 * weekday_sun + -0.2883 * weathersit_Light_snowrain + -0.0806 * weathersit_Misty + 0.0878 * season_summer + 0.1311 * season_winter
- Hypothesis Testing
Hnull - all the co-efficients are 0 
Ho - atleast 1 of the co-efficients are not 0/null
Based on what we build and see, the co-efficients are not 0, so we can reject the null Hypothesis
- We can infer for the company from the below listed variables are used in predicting the significant demand for shared bikes and from above co-efficients,
yr
holiday
temp
windspeed
mnth_sep
weekday_sun
weathersit_Light_snowrain
weathersit_Misty
season_summer
season_winter

- yr, temp, and weathersit_Light_snowrain(weathersit) are very significant(high coeff) in predicting the demand for the bikes

## Libraries
- numpy
- pandas
- matplotlib
- seaborn
- sklearn
- statsmodels.api






## Contact
Created by [@cenanine] - feel free to contact me!


<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->
