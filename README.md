# Stroke Prediction
Author: Priscilla Cole

# The Challenge
- According to the World Health Organization (WHO) stroke is the 2nd leading cause of death globally. This dataset is being used to predict whether a patient is more likely to have a stroke based on certain other parameters.

# Data Source and Information
- This data is comprised of 5110 observations and 12 attributes and is sourced from Kaggle.
- Link: https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset

## Data Dictionary
- id: Unique identifier to protect confidentiality 
- gender: Gender of individual; Male or Female
- age: age of individual
- hypertension: hypertension history of the patient; 1 if patient has hypertension and 0 if not.
- heart_disease: does the patient have heart disease? 1 if patient has heart disease and 0 if not.
- ever_married: has the patient ever been married?
- work_type: work type of the patient; private, self-employed, govt_job, children, other
- residence_type: residence type of the patient; urban or rural
- avg_glucose_level: average glucose level in the blood of the patient
- bmi: body mass index of patient
- smoking_status: smoking history of the patient; never smokes, smokes, formerly smoked
- stroke: our target; 1 if patient had a stroke and 0 if patient did not have a stroke

# Methods
- This data was loaded and copied for machine learning and exploratory visualizations. After thoroughly examining and cleaning our data, a series of univariate and multivariate visuals were created. Both univariate and multivariate visuals were used so that we could compare things like gender on a singular level (were there more males or females represented in the dataset); but also to explain characteristics when placed with another variable (like did men or women have hypertension more). Our target variable and features were defined and did our vaildation split. After performing necessary preparatory steps for machine learning, two classification models were created. The performance metrics of the two initial models were ran and then the best perofmrning model underwent PCA analysis as well. The performance with PCA was compared to the model's regular performance via a classification report. Based on those results, I was able to confidently pick the best production model to run. 

# EDA
- ![image](https://user-images.githubusercontent.com/110208019/197235324-9df03915-053b-418e-8080-7b5ba23207b7.png)
- This histogram was used to show the age distribution among patients. We can see that everything was evenly distributed from infant to eldery. 
- ![image](https://user-images.githubusercontent.com/110208019/197235526-e0726cc3-89ed-4b4d-ac59-b3bb6fa24a25.png)
- This histogram was used to see which gender had hypertension when compared to the other. We see that men were more likely to have high hypertension than women. 
- ![image](https://user-images.githubusercontent.com/110208019/197235847-0216b722-fe27-475f-9b14-7ee43cbe74d4.png)
- Correlation heatmaps are always a good visualization because it gives a look at the correlation between the target and the numerical features at the same time. This heatmap showed us that there was a positive correlation between the target and the features shown (except for the unique identifier, which was not included).

# Final Recommendations
- After considering several models and some feature engineering, the KNN model classifier with no PCA is the production model that was chosen. I picked this model because not only did it run the metrics faster than the others, it also produced the best results to answer our question. 
- 
# Contact Information
- Please feel free to contact me should you have any further questions or comments. I can be reached at priscillaecole@yahoo.com 

## Source
- This dataset was used from Kaggle
- link: https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset


