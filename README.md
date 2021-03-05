# Machine Learning for Exoplanet Recognition

### By Erick Hernandez

In this project, I was able to use different Machine Learning models in order to recognize whether an exoplanet gathers the minimum requirements to be considered as one or it was just a false positive (any other celestial body). The dataset used for this project was Kepler Exoplanet Search Results, available at: https://www.kaggle.com/nasa/kepler-exoplanet-search-results

The model I used for this analysis was a Logistic Regression. A Tree Model and a Support Vector Machine were also made as a comparison.

About the Logistic Regression, the selected X variables were:
koi_score - Values the confidence from 0 to 1 for each label (Candidate or False Positive)
koi_period - The time for each planetary consecutive transits
koi_duration - The visualization time since the first sight
ra and dec - Expressed in degrees, they refer to ascension and declination of the body

During the process, a classifier from sklearn library was used in order to fit the splitted data (X and Y in test and train).

After that, the model reported the following values: Training Data Score: 0.92, Testing Data Score: 0.88 meaning the information is highly reliable.

The other models (Tree and SVM) do not show reliable results as the Logistical Regression, this could be result of using several columns in the X variable that do not provide enough information for the model to work properly.

In my conclusion, I learned that the usage of several ML models is necesary in order to identify the most appropiate for out datasets, apart from selecting the correct information as input. Not only the selection of the model is important, but the interpretation of the results becomes crucial to determine its success.  
