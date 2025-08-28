💳 **Credit Card Fraud Detection: A Machine Learning Approach** </br>

This project addresses the critical challenge of credit card fraud detection by leveraging advanced machine learning techniques to build a robust classification model. Given the highly skewed nature of financial transaction datasets, this initiative prioritizes a meticulous approach to data preprocessing and a rigorous evaluation framework to ensure the reliable identification of fraudulent activities.</br>

<img width="1408" height="736" alt="Gemini_Generated_Image_m385a0m385a0m385" src="https://github.com/user-attachments/assets/560b36d6-83f5-4bba-a4ab-8fb91a7c8633" /> </br>



🎯 **Project Objectives** </br>

The primary goal of this project is to engineer and deploy a predictive model that can accurately discern fraudulent from legitimate credit card transactions. The methodology encompasses a comprehensive pipeline, from data ingestion and exploratory analysis to model training, evaluation, and optimization. A core focus is mitigating the challenges posed by class imbalance, which is characteristic of fraud detection problems.</br>

📊 **Dataset and Analysis**</br>

The analysis is based on a dataset of European credit card transactions from September 2013. The dataset comprises 284,807 transactions with 31 features, including 'Time', 'Amount', and a set of anonymized principal components (V1-V28). The dataset is notably imbalanced, with only 492 fraudulent transactions, representing a mere 0.172% of the total.</br>

📂 **Descriptive Statistics**</br>

A granular examination of the data reveals significant differences in transaction amounts between fraudulent and valid transactions.</br>

| Metric | Fraudulent Transactions | Valid Transactions |
| :--- | :--- | :--- |
| **Count** | 492 | 284,315 |
| **Mean Amount** | $122.21 | $88.29 |
| **Std Dev** | $256.68 | $250.10 |
| **Min Amount** | $0.00 | $0.00 |
| **Max Amount** | $2125.87 | $25691.16 |

This table clearly indicates that while the mean fraudulent transaction amount is higher, there's a wider range in valid transaction values.

🛠️ **Data Engineering and Preprocessing** </br>

1) To prepare the dataset for modeling and address the inherent imbalance, a series of strategic preprocessing steps were executed. </br>

2) Handling Missing Values: A preliminary check confirmed the absence of missing values, ensuring data integrity.</br>

3) Feature Scaling: The 'Amount' feature was standardized to a common scale to prevent it from disproportionately influencing model training.</br>

4) Class Imbalance Mitigation: The Synthetic Minority Over-sampling Technique (SMOTE) was applied to generate synthetic data points for the minority class (fraudulent transactions), thereby creating a balanced training dataset. This step is critical for preventing the model from being biased toward the majority class.</br>

🤖 **Model Implementation and Evaluation**</br>
A robust Random Forest Classifier was selected as the primary modeling algorithm due to its proven performance in handling complex, high-dimensional datasets. The model was trained on the preprocessed data and its performance was rigorously evaluated using a suite of metrics.</br>

📈 **Exploratory Data Analysis**</br>

Class Distribution: Visualized the imbalance between fraudulent and non-fraudulent transactions.</br>
Correlation Analysis: Examined correlations between features to identify potential multicollinearity.</br>
Feature Distributions: Plotted distributions to understand feature behavior.</br>

🤯 **Modeling**</br>

Implemented and compared the following machine learning algorithms:

Logistic Regression</br>
Decision Tree Classifier</br>
Random Forest Classifier</br>

*Each model was trained on the balanced dataset obtained after applying SMOTE.*

⚙️ **Model Evaluation**</br>

Evaluated model performance using the following metrics:

Confusion Matrix: To visualize true vs. predicted classifications.</br>
Precision: Measures the accuracy of positive predictions.</br>
Recall: Measures the ability to find all positive instances.</br>
F1-Score: Harmonic mean of precision and recall.</br>
ROC Curve: Illustrates the diagnostic ability of the binary classifier.</br>

*Emphasis was placed on minimizing false negatives to ensure fraudulent transactions are not overlooked.*

🎭 **Performance Metrics**</br>

The following table summarizes the key performance metrics of the Random Forest Classifier on the test set.

| Metric | Value |
| :--- | :--- |
| **Accuracy** | 99.95% |
| **Precision** | 97.53% |
| **Recall** | 85.27% |
| **F1-Score** | 91.00% |
| **Matthews Correlation Coefficient (MCC)** | 85.76% |

The high accuracy indicates the model's overall correctness. The precision score shows that when the model predicts a transaction as fraudulent, it is correct 97.53% of the time. The recall score, at 85.27%, signifies the model's ability to correctly identify 85.27% of all actual fraudulent transactions. The F1-Score provides a balanced measure of both precision and recall, while the MCC confirms a strong correlation between predicted and true classifications.</br>
 
🤔 **Confusion Matrix**</br>

The confusion matrix provides a detailed breakdown of the model's predictions,  which is crucial for understanding its performance on both classes.</br>

| | **Predicted Normal** | **Predicted Fraud** |
| :--- | :--- | :--- |
| **True Normal** | 56,861 (True Negative) | 3 (False Positive) |
| **True Fraud** | 23 (False Negative) |

The matrix reveals that out of 56,864 normal transactions, the model correctly identified 56,861, with only 3 false positives. More importantly, out of 98 fraudulent transactions, the model successfully identified 75, with only 23 being missed (false negatives). This low number of false negatives is a critical success factor, as it minimizes the risk of undetected fraud.</br>

🎨 **Data Visualization with Power BI**</br>

In addition to the core machine learning model, a dynamic dashboard was engineered using Power BI to provide a comprehensive, visual representation of the transactional data. This dashboard offers a layered perspective on the dataset, extending beyond a simple analysis of fraudulent transactions.</br>

<img width="1854" height="1235" alt="image" src="https://github.com/user-attachments/assets/09eced91-94aa-4335-b583-b170ff8668e7" />
<img width="1859" height="880" alt="image" src="https://github.com/user-attachments/assets/69f6e4fd-7d65-419d-a445-003fe8fe533e" />


The dashboard includes visualizations detailing:</br>

1) Customer Demographics: Defaulted customers are segmented by education, gender, marital status, and age, providing insights into risk profiles.</br>

2) Credit Limit Analysis: The distribution of credit limits is visualized against various demographic factors, helping to identify potential correlations between credit behavior and customer attributes.</br>

3) Data-Driven Insights: The interactive nature of the dashboard allows stakeholders to explore different facets of the data, such as the relationship between age and default behavior, or how credit limits vary across different educational and marital status groups.</br>

4) This visual component complements the predictive model by offering a strategic, business-oriented view of the data, enabling data-driven decision-making beyond just fraud detection.</br>

✅ **Conclusion**</br>

This project successfully demonstrates the application of machine learning techniques to detect fraudulent credit card transactions. Starting with a highly imbalanced dataset, comprehensive data preprocessing steps—including feature scaling and the application of SMOTE for oversampling—were employed to prepare the data for modeling. Exploratory Data Analysis provided insights into feature distributions and correlations, informing the selection of appropriate models.​

Three classification algorithms—Logistic Regression, Decision Tree, and Random Forest—were implemented and evaluated using metrics such as precision, recall, F1-score, and confusion matrix. Special emphasis was placed on minimizing false negatives to ensure that fraudulent transactions are accurately identified. Among the models tested, the Random Forest Classifier achieved the highest performance, balancing the trade-off between precision and recall effectively.​

The findings underscore the importance of addressing class imbalance and selecting suitable evaluation metrics in fraud detection tasks. Future enhancements could include exploring advanced algorithms, incorporating real-time detection capabilities, and integrating additional features to further improve model performance.​


