🛳 Titanic Survival Prediction with Random Forest
This project aims to predict whether a passenger survived the Titanic shipwreck using machine learning. The model is trained on the Kaggle Titanic dataset using the Random Forest Classifier algorithm.

📁 Files
train.csv — Training dataset containing features and survival labels.

test.csv — Test dataset for making predictions.

resultfile.csv — Final predictions submitted for the test data.

titanic_random_forest.py — Main script used for training and predicting.

README.md — Project overview and setup instructions.

📊 Features Used
After preprocessing, the following features are used for model training:

Pclass — Ticket class

Sex — Gender (mapped to 0 or 1)

SibSp — No. of siblings/spouses aboard

Parch — No. of parents/children aboard

Embarked — Port of Embarkation (mapped)

Title — Extracted from name (Mr, Miss, Royal, etc.)

AgeGroup — Binned age group

FareBand — Binned fare

Title — Mapped to numeric

AgeGroup — Mapped to numeric

🛠️ Preprocessing Steps
Drop Irrelevant Columns: Removed Cabin, Ticket, Name, and original Age, Fare.

Handle Missing Values: Filled missing age, embarked, and fare values with default or average values.

Feature Engineering:

Extracted Title from the name and grouped rare titles.

Binned Age and Fare into categorical bands.

Encoding:

Converted categorical variables like Sex, Embarked, Title, AgeGroup, FareBand to numeric formats.

📈 Model Training
Algorithm: Random Forest Classifier (from sklearn)

Data Split: 80% training, 20% validation

Accuracy Achieved: 84.36
