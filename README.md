# Predicting Healthcare Employee Attrition Using Machine Learning  

## Abstract  

### Background  
Global healthcare personnel shortages are forecasted to reach 14 million by 2030, largely due to employee attrition [1]. High attrition rates impose significant financial burdens on hospitals, degrade patient care quality, and lead to understaffing, which negatively affects the mental health and productivity of remaining employees [2]. Predicting healthcare employee attrition is a critical yet complex challenge.  

### Objective  
This study aims to develop and evaluate multiple machine learning (ML) classifiers to predict whether a healthcare employee is likely to leave their job and to identify significant factors contributing to attrition.  

### Methods  
- **Dataset**: Simulated data of 1,500 healthcare employees with 30 features from IBM Watson [3].  
- **Baseline Model**: Classification and Regression Tree (CART) model, chosen for its simplicity and interpretability.  
- **Additional Models**:  
  - Tree-based models: Random Forest, Bagged Trees, XGBoost, CatBoost  
  - Support Vector Machines (SVM)  
  - Logistic Regression with L1 and L2 Regularization  
- **Evaluation Metrics**: AUC, F1 Score, and Recall.  
- **Feature Importance**: Determined using the Borda Count System, which aggregates weighted votes across the top five features identified by each model to rank feature significance [4].  

### Results  
- **Best-Performing Model**: Logistic Regression with L2 Regularization  
  - AUC: 0.93 (30% improvement over baseline)  
  - F1 Score: 0.69 (50% improvement over baseline)  
  - Recall: 0.79 (70% improvement over baseline)  
- **Key Features Identified**:  
  - Marital status (single)  
  - Overtime  
  - Age  
  - Years of working  

### Conclusion  
Machine learning classifiers, particularly Logistic Regression with L2 Regularization, effectively predict healthcare employee attrition and identify significant contributing factors. These insights can help healthcare organizations design targeted interventions to prevent attrition and address workforce challenges.  

**Limitations**:  
- The dataset is simulated and based on the U.S. healthcare system, limiting its generalizability to other regions such as Canada.  
- Real hospital data is needed to validate model performance.  
- Incorporating additional features, such as time-series data, may further enhance accuracy and robustness.  

### References  
1. “Why do people stay in healthcare?,” National Center for Biotechnology Information, Jul. 01, 2022. [Online]. Available: https://pmc.ncbi.nlm.nih.gov/articles/PMC9243774/ [Accessed: Nov. 25, 2024].
2. “Employee turnover rates in the healthcare industry,” DailyPay, Nov. 18, 2023. [Online]. Available:https://www.dailypay.com/resource-center/blog/employee-turnover-rates-in-the-healthcare-industry/ [Accessed: Nov. 25, 2024].
3. J. P. Miller, "Employee Attrition for Healthcare," Kaggle, [Online]. Available: https://www.kaggle.com/datasets/jpmiller/employee-attrition-for-healthcare. [Accessed: Nov. 26, 2024].
4.	Y. Saeys, T. Abeel, and Y. Van de Peer, "Robust Feature Selection Using Ensemble Feature Selection Techniques," in Machine Learning and Knowledge Discovery in Databases, W. Daelemans, B. Goethals, and K. Morik, Eds., Lecture Notes in Computer Science, vol. 5212, Berlin, Heidelberg: Springer, 2008, pp. 313–325. doi: 10.1007/978-3-540-87481-2_21.


---  
This repository contains code, analysis, and documentation for the study. For more details, see the [Methods](#methods) and [Results](#results) sections. Contributions and discussions are welcome to extend this work further.  
