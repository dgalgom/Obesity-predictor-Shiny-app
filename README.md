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

