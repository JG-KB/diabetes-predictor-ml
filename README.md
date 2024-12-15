# Diabetes-predictor-ML

Presentation Link: https://docs.google.com/presentation/d/1xWjblsn67Rd9C_NS568wlAKU4kz-Vnx8hmAK-SH7rYw/edit?usp=sharing

## **Overview:**

Diabetes is a chronic disease that affects how your body turns food into energy. In america over 34 million people have diabetes, and 90-95% of them have type 2 diabetes. In this analysis we will be using a dataset from the Behavioral Risk Factor Surveillance System (BRFSS) in conducted 2015 with over 70,000 participants and 18 different features to predict whether a person has diabetes.

In this project we examined 8 different models to predict whether a person has diabetes. We started with a simple logistic regression model, and then moved on to more complex models such as random forests and gradient boosting. After tuning the hyperparameters of the random forest and gradient boosting models, we found that the gradient boosting model performed the best.

In the end, we were able to achieve an accuracy of 75% on the test set, precision of 75%, and an AUC of 0.83.

## **Data:**

The dataset contains 70,000 observations and 18 features. The features are as follows:
**AgeMean:** The average age of the participant.

**Gender:** The gender of the participant.

**HighCholesterol:** Whether the participant has high cholesterol.

**CholesterolCheck:** Whether the participant has had their cholesterol checked in the past year.

**BodyMassIndex:** The body mass index of the participant.

**SmokerStatus:** Whether the participant is a smoker.

**HeartDiseaseHistory:** Whether the participant has had a heart disease in the past.

**PhysicalActivity:** Whether the participant has had physical activity in the past month.

**DailyFruitIntake:** Does the participant eat fruit daily.

**DailyVegetableIntake:** Does the participant eat vegetables daily.

**HeavyAlcoholConsumption:** Whether the participant has had heavy alcohol consumption in the past month.

**GeneralHealth:** A self reported 1-5 of the general health of the participant.

**PoorMentalHealthDays:** The number of days the participant has poor mental health in the past month.

**PoorPhysicalHealthDays:** The number of days the participant has poor physical health in the past month.

**DifficultyWalking:** Whether the participant has difficulty walking.

**StrokeHistory:** Whether the participant has had a stroke in the past.

**HighBloodPressure:** Whether the participant has high blood pressure.

**DiabetesDiagnosis:** Whether the participant has been diagnosed with diabetes.

## **Model Selection:**

We looked at 8 different models to predict whether a person has diabetes. SVM, Log Regression, Decision Tree, KNN, Random Forest, Extra Trees, Gradient Booster, AdaBoost.

Our inital results were:

Logistic Regression Training Accuracy: 0.747
Logistic Regression Test Accuracy: 0.746

SVM Training Accuracy: 0.747
SVM Test Accuracy: 0.745

Decision Tree Training Accuracy: 0.972
Decision Tree Test Accuracy: 0.658

K-Nearest Neighbors Training Accuracy: 0.798
K-Nearest Neighbors Test Accuracy: 0.716

Random Forest Training Accuracy: 0.972
Random Forest Test Accuracy: 0.728

Extremely Random Trees Training Accuracy: 0.972
Extremely Random Trees Test Accuracy: 0.712

**Gradient Boosting Training Accuracy: 0.754**
**Gradient Boosting Test Accuracy: 0.753**

AdaBoost Training Accuracy: 0.754
AdaBoost Test Accuracy: 0.753

## **Model Tuning:**

Before removing any features, we found feature importance to be:

| Feature | Importance |
|---------|------------|
| GeneralHealth | 0.4102 |
| HighBloodPressure | 0.2325 |
| BodyMassIndex | 0.1213 |
| AgeMean | 0.1016 |
| HighCholesterol | 0.0695 |
| HeartDiseaseHistory | 0.0165 |
| DifficultyWalking | 0.0128 |
| HeavyAlcoholConsumption | 0.0105 |
| CholesterolCheck | 0.0095 |
| Gender | 0.0075 |
| PoorPhysicalHealthDays | 0.0024 |
| StrokeHistory | 0.0023 |
| PoorMentalHealthDays | 0.0017 |
| PhysicalActivity | 0.0005 |
| DailyVegetableIntake | 0.0005 |
| SmokerStatus | 0.0003 |
| DailyFruitIntake | 0.0002 |

## **Results:**

In the end, we were able to achieve an accuracy of 75% on the test set, precision of 75%, and an AUC of 0.83.
![Recieving Operating Characteristic Curve](image.png)

