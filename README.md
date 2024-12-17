# Obesity-predictor-Shiny-app

This repository was created with the aim of showing one of the most useful functionalities of **Shiny** in **R**: give you reactive (i.e., instant) feedback when changing parameters of a model for predicted responses. In this case, we use our **Shiny** app to predict the risk of be categorised as overweight/obese regarding eating habits and phsyical condition. Therefore, it is a **classification task**, which can be tackled using different machine learning algorithms such as the C5.0 algorithm.
As specified in the `.Rmd` file, this data analysis has been performed using data for the estimation of obesity levels in individuals from Mexico, Peru, and Colombia. The official dataset is called "*Estimation of Obesity Levels Based on Eating Habits and Physical Condition*", which can be found in the *UC Irving Machine Learning Repository*. The dataset is built by 17 attributes and 2111 records; nevertheless, after data processing, wrangling, and splitting procedures, the final **training** and **test** datasets were constituted by 1689 observations, and 422 observations respectively. Importantly, **77% of the data was generated synthetically**.

## Variables explanation

The flowwing variables do not exactly match with those appearing in the original dataset because of data processing and wrangling procedures to optimise the model training, but the gist of the variables is the same.

  + `Gender`: 0 - males; 1 - females.
  + `Age`: numeric variable for the age.
  + `Family History with Overweight`: 0 - no family history of overweight; 1 - any familiar with overweight.
  + `Vegetables in your food?`: how many vegetables do you put in your plate usually?
  + `Food between meals` columns: frequency of eating between principal meals.
  + `Smoker`: 0 - no smoker; 1 - smoker.
  + `Physical activity (days)`: how many days do you engage in physical activities?
  + `Time using technological devices`: hours per day using tech devices ranging from 0 to 3.
  + `No alcohol consumption`: 0 - alcohol consumption; 1 - no alcohol consumption (it could be a bit confusing, sorry for not transforming this variable in a more easy-to-understand way).
  + `Active commuting` variables: do you commute to work actively by walking or cycling?
  + `Target`: BMI status, which is the target we want to predict.

## Model training and predictions using our Shiny app
Focusing exclusively in the scope of this repository, we only trained one model using a C5.0 algorithm, which is a decision tree algorithm applied for classification tasks. After that, we observed the agreement between predicted and observed BMI status. Finally, we used our **Shiny** to make predictions and obtained visualizations of the predicted probabilities in real-time.

|     |Insufficient|Normal |Overweight/Obesity|
|------------:|----|---------|---------|
|Insufficient     |38  |11|5|
|Normal         |4  |33|23|
|Overweight/Obesity         |4  |15|289|

<img width="1140" alt="Screenshot 2024-12-17 at 08 57 12" src="https://github.com/user-attachments/assets/7a299c19-f0cd-46da-b14f-f42604b29cb8" />




