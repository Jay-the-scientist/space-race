# Space-Race

## SpaceX Falcon 9 Landing Prediction
This project applies machine learning and data science techniques to build predictive models for SpaceX first stage booster landing outcomes using their launch data. The goal is to help SpaceX and other launch providers optimize their reusability programs.

## Project Description
SpaceX aims to reduce costs through reuse of Falcon 9 first stages. However, landings pose significant challenges and are not always successful. This work develops classification models to predict landing result based on mission parameters. Insights can guide engineering and pricing decisions.

## Data
Launch records were obtained from SpaceX API and Wikipedia pages. Over 100 entries contained attributes on payload, orbit, site, booster, outcome details.

## Methodology
Data wrangling cleaned and standardized values. EDA explored relationships. Models like Logistic Regression, Decision Trees and Random Forests were implemented in scikit-learn. Hyperparameter tuning optimized performance.

## Results
The Random Forest classifier achieved 84% accuracy on the test set, outperforming other algorithms. Payload mass, booster version and launch site emerged as important predictors. These models provide a quantitative approach to support SpaceX operations.
