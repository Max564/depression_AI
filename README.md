# depression_AI
URL dataset
https://www.kaggle.com/datasets/adilshamim8/student-depression-dataset?resource=download

depression AI Modeling
This is try to make AI model That can predict depression for Students with this dataset
Features:
ID: Unique identifier for each student
Demographics: Age, Gender, City
Academic Indicators: CGPA, Academic Pressure, Study Satisfaction
Lifestyle & Wellbeing: Sleep Duration, Dietary Habits, Work Pressure, Job Satisfaction, Work/Study Hours
Additional Factors: Profession, Degree, Financial Stress, Family History of Mental Illness, and whether the student has ever had suicidal thoughts

categrize data: gender, city, sleep duration, dietary habits, degree
numrical data = age, CGPA, AP, Study Satisfaction, work pressure, job satisfaction, work/study hours, Financial stress, family mental illness, suicidal thoughts.

after the clean:

layer Structure:
Input layer with 64 neurons (ReLU activation)
Dropout layer (20% rate) for regularization
Hidden layer with 32 neurons (ReLU activation)
Output layer with 1 neuron (sigmoid activation)

Optimizer: Adam is a good default choice (adaptive learning rate)
Loss Function: Correctly using binary_crossentropy for binary classification
Metrics: Tracking accuracy is standard for classification

Performance Analysis:
Training Accuracy: 89.12% (good)
Validation Accuracy: 83.26% (reasonable)
Gap Analysis:
~6% difference between train/val accuracy suggests slight overfitting
Val loss (0.4314) > Train loss (0.2601) confirms this


This model performs well (89% train accuracy) but could improve in generalization (val accuracy: 83%).


