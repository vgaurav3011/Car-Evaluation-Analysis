# Car-Evaluation-Analysis

![alt-text](https://raw.githubusercontent.com/vgaurav3011/Car-Evaluation-Analysis/master/assets/index.jpeg)

## Business Understanding

- Car Evaluation for different features becomes an important tool for recommendation to the users as per their requirements, and needs to be designed as a tool that can help in developing closer relationships between the automobile industry and its customers.
- It is useful in identifying cusotmer bases and loyalties as well as can be used for customer segmentation as per needs and income classes.

## Data Understanding

- The data contains 1728 rows and 7 columns with descriptions as follows:
  - buying: Buying Level or Capacity of the customer (Very High:vhigh, High:high, Low:low, Medium:med)
  - maint: Maintainence Level (Very High:vhigh, High:high, Low:low, Medium:med)
  - doors: Number of doors in the car (2, 3, 4 and 5 or more)
  - lug_boot: Luggage Boot Size in the car (small, med, big)
  - safety: Safety Level of Car (high, med, low)
  - class: Unacceptable, Acceptable, VeryGood, Good

## Data Preparation

- The data is a classic multi-class classification task with multiple classes of cars available as the final evaluation
- The data does not have any missing values
- The data does not have repetitive columns
- The data is fully categorical with even the final target variable is also in form of a category
- Label Encoding and mapping is used to make continous labels for the majorly ordinal data


## Modelling and Evaluation

- Random Forest Classifier surpasses its counterparts MLP and Logistic Regression with an accuracy of 93.5% on the data.
- Logistic Regression comes down to 70 percent in accuracy score with many false negatives present in the prediction.
- This is an expected behaviour since LR works for binary classifications and does not converge well for multiple classes since it bases on the theory of probability estimates of the classes that can clash.
- MLP classifier fails to converge to optimal performance.
- Accuracy Score is used as the metric for evaluation.

## Deployment

- The app is deployed as a Streamlit Web Application with the following options:
  - Exploratory Data Analysis:
    - 5 point summary
    - Countplot of classes
    - Column Selection
   - Prediction:
    - Logistic Regression
    - MLP Classifier
    - Random Forest Classifier
    - Custom Data Entry
- To run the web app follow the instructions: <br/>
  `git clone <repo-URL>
  `
  
  <br/>
  
  `streamlit run app.py`
  
  ![alt-text](https://raw.githubusercontent.com/vgaurav3011/Car-Evaluation-Analysis/master/assets/dashboard.gif)
  
  
