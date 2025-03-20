# Freezing-of-Gait-Detection

FOG is a condition often experienced by individuals with Parkinson's disease,
where they temporarily feel unable to move, particularly while walking. Detecting
these episodes is crucial for improving patient safety and mobility.
Symptoms:-  
• Sudden stopping while walking.                                                                                       
• Difficulty starting to walk, often described as a "frozen" sensation.  
• Short, shuffling steps.  

# Objective 

The primary objective of this project is to develop a comprehensive ensemble
learning model for analyzing and predicting freezing of gait (FOG) in patients with
Parkinson's Disease. By integrating various data types—including medical records,
movement patterns, and sensor data—this model aims to identify patterns and
key indicators that signal FOG episodes. The use of ensemble learning techniques
allows for improved prediction accuracy by combining the strengths of multiple
algorithms, thereby enhancing the model's ability to capture the complex
interplay of factors contributing to FOG. Ultimately, this project seeks to provide
insights that could lead to better management and treatment strategies for
patients experiencing FOG.

# DATASETS USED FOR IMPLEMENTATION:  
1.Daphnet Dataset -  
The dataset comprises 3 wearable wireless acceleration sensors recording 3D
acceleration at 64 Hz. The sensors are placed at the ankle (shank), on the thigh
just above the knee, and on the hip.

1.Mendley Dataset-
Sensors used – Accelerometers: (X,Y,Z axes on L,R shank, arm , waist)
Gyroscopes: (X,Y,Z axes on L,R shank, arm , waist)
Electromyography (EMG): Placed on muscles involved in gait
Electroencephalography (EEG): Electrodes placed on the scalp.
Skin Conductance Sensors: Measures the electrical conductance
of the skin

# METHODOLOGY
1.Dataset collection  
2.Exploratory Data Analysis/Data pre-processing (handling missing values , balancing the data, removing  
outliers , removing duplicates in the data , normalization/standardization )  
3.Dividing data into train and test( 80:20 ,70:30,60:40,50:50 respectively)  
4.Approaches used :-  
• Bagstacking(5 lightGBM base models, random forest meta learner )  
(using k—fold cross validation)    
• Bagstacking ( lightgbm , logistic regression , SVM , Random Forest are  
the base models , and Random forest as the meta learner ) (using k—fold  
cross validation)  
• Using models like lightgbm , svm , random forest , XGboost individually  
to compare the results (k-fold cross validation is used for robust training )  
5.Final evaluation using evaluation metrics like Accuacy , precesion , recall , F1
score , MAP (Mean absolute prediction ) etc...
