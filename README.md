# Liver_Cancer_prediction
          Liver_Cancer_prediction using Machine Learning

Liver is the vital internal organ inside the human body, which eliminates toxics and preserves protein and vitamins.
Liver disorder can cause serious health issues. Most researchers found that machine learning contributes greatly in the early diagnosis of liver disorder.
We have proposed various machine learning methods to predict liver cancer on the basis of clinical dataset provided.

![image](https://user-images.githubusercontent.com/87700405/184545354-c143b925-289e-483b-b0f8-53f23f38d52e.png)

This dataset is contained of 79 features and 4437 rows of data.

   There are mainly two valid target classes that can be considered for machine learning, those are “Alive” and “Deceased” other than this feature PATIENT_STATUS also contains null and invalid class which are being removed during cleaning process.
   
                 Data Cleaning
 
   In machine learning, Data Preparation is an important step which includes the cleaning and merging of a data which identified or collected during collection process. The data can be combined or collected from multiple sources and even sometimes with different formats. Pre-processing can include data cleaning, integration check, transforming data and reducing data to relevant data. We started cleaning process with removing null and then unwanted class from target class from PATIENT_STATUS column of the dataset.
   
Then we replaced string value to numeric like Yes to 1 and No to 0, Male to 1 and Female to 0 and Alive to 1 and Deceased to 0 then we tried to fill all the null or missing values & selected feature percentage greater than 80% with their respective mean values. 

              Data Visualization

The target class for this study is considered as PATIENT_STATUS feature and their respective count.
   ![image](https://user-images.githubusercontent.com/87700405/184547800-0f18e2d6-7f76-4afc-8a22-53b541acf3ac.png)
   
                
![image](https://user-images.githubusercontent.com/87700405/184547823-adc66fbb-52e5-443c-9643-6336f9fb2d60.png)

 Histogram Plot

The correlation between target class and rest of the features.
![image](https://user-images.githubusercontent.com/87700405/184548037-14a9713d-fadb-4be4-8ec0-98ec9db09b89.png)





              C.	Model Building and Prameter Tuning 


Before proceeding to classification, we have to split the dataset and convert all the string features to numeric values.
  
              Feature Selection
 
   The feature selection is done using Extra Trees Regressor and Recursive Feature Elimination where we have selected important features for the Random Forest classifier.
   we are able to predict liver cancer patient with an accuracy of 71% which is highest among other classifiers. We also performed machine learning with Decision Tree and Random Forest for cancer prediction and accuracy achieved 69% for both these models. 
