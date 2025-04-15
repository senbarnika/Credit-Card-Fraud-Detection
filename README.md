💳 Credit Card Fraud Detection</br>

This project aims to detect fraudulent credit card transactions using machine learning techniques. Given the highly imbalanced nature of the dataset, special attention is paid to data preprocessing and evaluation metrics to ensure accurate detection of fraudulent activities.</br>

![image](https://github.com/user-attachments/assets/91278b78-99ee-49ef-8010-0b7f051ece8f)

📂 Table of Contents</br>

Project Overview</br>
Dataset</br>
Data Preprocessing</br>
Exploratory Data Analysis</br>
Modeling</br>
Model Evaluation</br>
Conclusion</br>

📌 Project Overview</br>

The objective is to build a classification model capable of accurately identifying fraudulent credit card transactions. The project explores various machine learning algorithms and addresses the challenges posed by the imbalanced dataset.</br>

📊 Dataset</br>

Source: Kaggle Credit Card Fraud Detection Dataset</br>
Description: Contains transactions made by European cardholders in September 2013.</br>
Size: 284,807 transactions with 31 features.</br>
Imbalance: Only 492 transactions (0.172%) are fraudulent.</br>

🛠️ Data Preprocessing

Handling Missing Values: Verified and confirmed the absence of missing values.</br>
Feature Scaling: Applied standardization to the 'Amount' feature.</br>
Class Imbalance: Utilized Synthetic Minority Over-sampling Technique (SMOTE) to balance the dataset.</br>

📈 Exploratory Data Analysis</br>

Class Distribution: Visualized the imbalance between fraudulent and non-fraudulent transactions.</br>
Correlation Analysis: Examined correlations between features to identify potential multicollinearity.</br>
Feature Distributions: Plotted distributions to understand feature behavior.</br>

🤖 Modeling</br>

Implemented and compared the following machine learning algorithms:

Logistic Regression</br>
Decision Tree Classifier</br>
Random Forest Classifier</br>

*Each model was trained on the balanced dataset obtained after applying SMOTE.*

⚙️ Model Evaluation</br>

Evaluated model performance using the following metrics:

Confusion Matrix: To visualize true vs. predicted classifications.</br>
Precision: Measures the accuracy of positive predictions.</br>
Recall: Measures the ability to find all positive instances.</br>
F1-Score: Harmonic mean of precision and recall.</br>
ROC Curve: Illustrates the diagnostic ability of the binary classifier.</br>

*Emphasis was placed on minimizing false negatives to ensure fraudulent transactions are not overlooked.*

✅ Conclusion</br>

This project successfully demonstrates the application of machine learning techniques to detect fraudulent credit card transactions. Starting with a highly imbalanced dataset, comprehensive data preprocessing steps—including feature scaling and the application of SMOTE for oversampling—were employed to prepare the data for modeling. Exploratory Data Analysis provided insights into feature distributions and correlations, informing the selection of appropriate models.​

Three classification algorithms—Logistic Regression, Decision Tree, and Random Forest—were implemented and evaluated using metrics such as precision, recall, F1-score, and confusion matrix. Special emphasis was placed on minimizing false negatives to ensure that fraudulent transactions are accurately identified. Among the models tested, the Random Forest Classifier achieved the highest performance, balancing the trade-off between precision and recall effectively.​

The findings underscore the importance of addressing class imbalance and selecting suitable evaluation metrics in fraud detection tasks. Future enhancements could include exploring advanced algorithms, incorporating real-time detection capabilities, and integrating additional features to further improve model performance.​


