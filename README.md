# Project Overview
Security Operations Centres(SOCs) are reproving in identifying and reducing cyber threats. However the volume of incidents and wariness makes it more difficult for analysts to efficiently triage and respond. This project aims to amplify SOC efficiency by devolving a machine learning model to classify cybersecurity incidents from True Positive(TP), Benign Positive(BP), False Positive (FP) categories. By utilizing the GUIDE dataset, the model is designed to hold-up guided response systems, improving the all over security posture of enterprise environments.

# Data
Training data has 9516837 rows and 45 Columns
Testing data has 4147992 rows and 46 Columns
The data is collected from various sources including network devices, security information and event management systems, and threat
intelligence feeds.

# Model Building
Three Models are build in this project
1. Random Forest 
2. Decision Tree
3. XGBoost
The models are trained on the training data and evaluated on the testing data.
The following steps were taken to build the models:
1. Initial Inspection
Explored the Both train and test dataset with 45 and 46 features
respectively and incident labels(TP,BP,FP).
2. Exploratory Data Analysis:
Visualized class distributions and pointed out an imbalance like
TP,FP,BP. Also visualized various other factors like “Counts of
category by Incident Grade”, “Counts of Entity by incident
grade”. Below is the few visualization obtained from test and
train data.
3. Data Preprocessing
  1. Removing the Null Values
  2. Feature Engineering
  3. Encoding Categorical Variables
4. Data Splitting 
Train-validation split(80-20) graded by the target variable to maintain
class balance.
5. Model Development
Trained various advance models like Random Forest Classifier,Decision tree classifier and XGBoost on both train and test data.
6. Evaluation Metrics
• Recall: Ensured recognition of all true positive
• Precision: More focused on reducing false positives
• Macro_F1 score: Equal and balanced measures of precision and recall among all classes

# Conclusion
The Developed model achieves robust classification performance with a precison of
0.87 and macro F1-Score of 0.84 using XGBoost, outperforming the other two
advance models. This key automates incident triage effectively decreasing the
burden on SOC analysts and enabling it for more fast and accurate threat response.
This model speed up the way for enhanced cybersecurity operation and upgrade
organizational resilience against threats.