# Rock_Vs_Mine
🪨 Rock vs Mine Prediction
A machine learning project that predicts whether a sonar signal has bounced off a metal cylinder (Mine) or a rough cylindrical rock (Rock). This project utilizes a Logistic Regression model to classify sonar returns based on the signal strength at different angles.

📌 Overview
Submarines and naval vessels use sonar to detect objects underwater. Distinguishing between rocks and man-made mines is crucial for navigation and safety. This project builds a predictive system that takes sonar data as input and determines the object type.

Model Used: Logistic Regression

Accuracy (Test Data): ~76.2%

Accuracy (Training Data): ~83.4%

📂 Dataset
The project uses the Sonar Dataset (sonar.csv).

Size: 208 samples.

Features: 60 numerical columns representing the energy within a particular frequency band.

Target Labels:

M: Mine (111 samples)

R: Rock (97 samples).

🛠️ Technologies Used
Python

Pandas (Data manipulation)

NumPy (Array processing)

Scikit-Learn (Model training and evaluation)

⚙️ Workflow
Data Loading: The sonar.csv data is loaded into a Pandas DataFrame without a header.

Data Analysis: checked statistical measures and class distribution (M vs R).

🧩Preprocessing:
  Separated features (X) and labels (Y).
  Split data into training (90%) and testing (10%) sets.

Note: stratify = Y was used to maintain the ratio of Rocks to Mines in the split.

Model Training: Trained a Logistic Regression model on the training set.

Evaluation: Calculated accuracy scores for both training and test data.

Prediction System: Built a system to take new input data, reshape it, and predict the object type.

📈 Results:
The model achieved the following accuracy metrics:
Training Accuracy: 83.42%
Test Accuracy: 76.19%

📜 License:
This project is open-source and available under the MIT License.
