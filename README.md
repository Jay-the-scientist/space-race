# Space-Race

## SpaceX Falcon 9 Landing Prediction
This project applies machine learning and data science techniques to build predictive models for SpaceX first stage booster landing outcomes using their launch data. The goal is to help SpaceX and other launch providers optimize their reusability programs.

## Project Description
SpaceX aims to reduce costs through reuse of Falcon 9 first stages. However, landings pose significant challenges and are not always successful. This work develops classification models to predict landing result based on mission parameters. Insights can guide engineering and pricing decisions.

## Installation

Required packages include:
-Pandas 
-NumPy 
-SciPy 
-Scikit-Learn 
-Matplotlib 
-Folium

## Data
Launch records were obtained from SpaceX API and Wikipedia pages. Over 100 entries contained attributes on payload, orbit, site, booster, outcome details.

![Raw Data](images/dataprep/1-rawdata.png)

## Methodology
Data wrangling cleaned and standardized values. EDA explored relationships. Models like Logistic Regression, Decision Trees and Random Forests were implemented in scikit-learn. Hyperparameter tuning optimized performance.

![Structured Dataset](images/dataprep/5-structureddataset.png)

## Results
The Random Forest classifier achieved 84% accuracy on the test set, outperforming other algorithms. Payload mass, booster version and launch site emerged as important predictors. These models provide a quantitative approach to support SpaceX operations.

### I was able to visualize the trends in yearly launch success rate:

![Yearly Launch Success Rate](images/pandasvisualization/6-yearlylaunchsuccessrate.png)

### Then generated an interactive map that displayed the successful and failed launches per launch site

![Successful and Failed Launches Visualized](images/interactivemaps/12-launchlocationsclusteredmarkers-zoom.png)

### And an interactive dashboard that displays the success ratings of each launch site

![All Sites Success Ratings](images/interactivemaps/15-dashboard-all.png)

### And an interactive plot that shows the relation between mission type (success or fail) and payload mass among the different booster versions

![Payload Mass v Mission Type by Booster Version](images/interactivemaps/17-dashboard-payloadmass-vs-boosterversion.png)

