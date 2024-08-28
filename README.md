# Bike Sharing Assignment Notebook


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information


### Problem Context

This company BoomBikes provides bike rental service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system. 

The company wants to accelerate its revenue and prepare themselves to cater to the people's needs and to stand out from other service providers and make huge profits.

### Problem Outcome

Build a multiple linear regression model for the prediction of demand for shared bikes.

 - Which variables are significant in predicting the demand for shared bikes.

 - How well those variables describe the bike demands

### Bike Ride Set  
It contains the number of bike rides booked for days with different parameters (weather condition, temperature etc.)for the day for all loans issued through the time period 2007 t0 2011.

### Data Dictionary
The data dictionary that describes the meaning of the columns present in the dataset.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions

### **Model without constant**

|Predictor Name| Predictor Constant|
|-|-|
|temperature    |0.67189|
|year           |0.236900|
|WINTER         |0.178648|
|SUMMER         |0.117481|
|SEPTEMBER      |0.111056|
|SPRING         |0.055794|
|LIT_RAIN       |-0.278983|
|windspeed      |-0.101548|
|is_holiday     |-0.093459|
|MIST           |-0.069726|

- Model Efficiency 
    - Train: 0.819
    - Test: 0.782


### **Model with constant**

|Predictor Name| Predictor Constant|
|-|-|
|temperature  |  0.570769 |
|const        |  0.226132 |
|year         |  0.228910 |
|WINTER       |  0.139117 |
|SEPTEMBER    |  0.106905 |
|SUMMER       |  0.090651 |
|LIT_RAIN     | -0.235328 |
|windspeed    | -0.187000 |
|humidity     | -0.175596 |
|is_holiday   | -0.097453 |
|MIST         | -0.050318 |

- Model Efficiency 
    - Train: 0.837
    - Test: 0.805

### Top 3 contributors:

- Temperature of the day

- Year

- Season being WINTER


<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used

- Data Analysis Library
    - pandas
    - numpy
    - statsmodels
    - sklearn
- Visualization Libraries 
    - matplotlib
    - seaborn

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project was inspired by...
- References if any...
- This project was based on [this tutorial](https://www.example.com).


## Contact
Created by [@githubusername] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->