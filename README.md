# Starbucks-Offer-Optimization
- [Introduction](#Introduction)
- [Installation](#Installation)
- [Project Components](#Project-Components)
- [File Descriptions](#File-Descriptions)
- [Instructions](#Instructions)
- [Results](#Result)
- [Licensing, Authors, Acknowledgements](#License)

## Introduction <a name="Introduction"></a>
To increase sales, offers are effective, but they must be used appropriately and viewed as an expense. If the customers would buy anyway, we do not want to send them any kind of offer. Considering that this is a classification problem classification models will be used and performance will be measured by precision, recall, and f1 score. The main objective of this project is to build a model that predicts what offer should be sent to each customer depending on their demographic so that they would react and complete the offer intentionally.

## Installation <a name="Installation"></a>
The following packages and versions are used for this project
| Package  | Version |
| ------------- | ------------- |
|pandas|1.3.4|
|numpy|1.20.3|
|matplotlib|3.4.3|
|scikit-learn|0.24.2|
|seaborn|0.11.2|           

## Project Components <a name="Project-Components"></a>
There are 3 main components in this project.
### 1. Exploratory Data Analysis and Cleaning
- Load the three datasets 
- Clean the datasets
- Handle missing values
- Saved them in csv format for future use

### 2. Feature Engineering
- Create offer_completed,offer_accidentally_completed,offer_ignored and offer_didnotcomplete columns for every offer
- Grouped the columns on customer id to get clear idea what offers the customer has recieved,viewed and completed.
- Merged this data with the customer demographics to train the model
- Saved them in csv format for future use

### 3. Data Visualization
- Used the above the data to visual and answer some business questions
- some more insights about the offers

### 4. Data Preprocessing
- created bins to handle class imbalance
- searched for outliers

### 5. Machine Learning Model
- trained several classifier models to find the best base model on the training data
- Using feature importance, removed unnecessary features
- GridSearchCV to find the optimal hyperparameters



## File Description <a name="File-Descriptions"></a>
This is the high level description of all the files in this project.
```

├── data
│   ├── transcript.json-----------------------# records for transactions, offers received, offers viewed, and offers completed
│   ├── profile.json--------------------------# demographic data for each customer
│   ├── portfolio.json------------------------# containing offer ids and meta data about each offer
│   └── Starbucks_X_test.csv------------------# custoemrs grouped based on demographics
|       Rest of the files are created dynamically
|                 
├── models
|   ├── RandomForestClassifier.pkl-------------------# Pickle file
|   
├── img
|    ├──block_diagram.PNG----------------------------# Block diagram 
|    Rest of the files are screenshots of the results for the blog
|
|
├── Starbucks_Capstone_notebook.ipynb-----------------# Main notebook

```


### Instructions:<a name="Instructions"></a>

1. Make sure to have packages mentioned above before running the notebook

## Result <a name="Result"></a>
Click [here](https://docs.google.com/spreadsheets/d/1Lc3pBF04SjOxjunbaiuLOw6ProiPE68ZOXrZ9BTnHY8/edit#gid=1770578135) to see the results in a google sheet.Blog link [here](https://medium.com/@vmskrsh/starbucks-best-suited-offers-based-on-customer-demographics-8e0a7181a14a)

## Licensing, Authors, Acknowledgements <a name="License"></a>
Reference

   https://pbpython.com/natural-breaks.html
  https://pbpython.com/natural-breaks.html
  https://stackoverflow.com/questions/55104819/display-count-on-top-of-seaborn-barplot
  https://github.com/mariavaghani/Optimizing-App-Offers-With-Starbucks
  https://stackoverflow.com/questions/16476924/how-to-iterate-over-rows-in-a-dataframe-in-pandas

* Starbucks for providing the datasets.
* [Udacity](https://www.udacity.com/) for project goal.
* Chaitanya KC for assistance with the main project goal
* Author: [G.Vamsi Krishna](https://github.com/Krishna5972)
