# SaifullahSaleem-Fake-News-Detection-Exploring-Diff-ML-Techniques


## **1. Introduction**  
The internet has enabled rapid access to information, but verifying its authenticity remains a challenge. Fake news and deceptive articles negatively impact trust in media and influence public behavior, including voting patterns. This project aims to tackle this issue using machine learning for text classification, developing an application that categorizes news articles as genuine or fake.  

Given the rising prevalence of fake news, tools for detection and combatting misinformation are essential. Such systems benefit media outlets, individuals, and governing bodies by reducing the time and resources needed for verification. Additionally, they foster better decision-making and improve media literacy in an era dominated by social media.  

This project applies machine learning models, including Decision Tree Classifier, Passive Aggressive Classifier, XGBoost, Support Vector Machines (SVM), and Random Forest, to categorize news articles. After extensive preprocessing, tokenization, and vectorization of text data, these models were trained to differentiate between real and fake news. The Passive Aggressive Classifier achieved the highest accuracy of 93.16%, making it the final model used. A separate front-end interface was also developed, allowing users to input news content and receive real-time predictions.  

## **2. Objective**  
The project's primary objective is to develop a reliable machine learning system that classifies news articles into two categories: real and fake. The system aims to achieve high accuracy through rigorous preprocessing and model training strategies. Additional objectives include enhancing usability by implementing a user-friendly front-end interface, ensuring seamless real-time predictions. By integrating high model accuracy with simplicity, this project aims to establish an effective solution for countering fake news.  

## **3. Workflow Overview**  
### **Importing Libraries**  
- Listing the required libraries.  
- Brief explanation of their necessity.  

### **Data Preprocessing**  
- Description of dataset (size, features, and labels).  
- Handling missing values.  
- Removing duplicates or irrelevant columns.  
- Encoding categorical variables, if applicable.  

### **Data Visualization**  
- Presenting insights from Exploratory Data Analysis (EDA) using visualizations:  
  - Distribution of real vs. fake news.  
  - Most common words in the dataset.  

### **Vectorization of Data**  
- Converting text data into numerical format using TF-IDF vectorization.  

### **Model Implementation and Accuracy Analysis**  
- Brief descriptions of applied models.  
- Accuracy scores and confusion matrices.  
- Discussion of reasons for accuracy scores.  

### **Comparison of Accuracy Scores**  
- Analyzing differences in model performances.  
- Detailed accuracy comparison and reasoning.  

### **Choosing the Best Model**  
- Justification for selecting the most accurate and efficient model.  

### **Model Saving and Loading**  
- Storing the trained model and using it for predictions.  

### **Front-End Development**  
- Tools used (Flask).  
- Functionalities (e.g., text input for news, real-time predictions).  
- Backend integration with the Passive Aggressive Classifier.  

## **4. Models Applied**  
### **4.1. Decision Tree Classifier**  
- **Accuracy:** 80.3%  
- **Reasons for Accuracy:**  
  - Prone to overfitting.  
  - High variance due to noisy text data.  
  - Lacks ensemble learning benefits.  
  - Limited decision boundaries for non-linear data.  

### **4.2. Passive Aggressive Classifier**  
- **Accuracy:** 93.16%  
- **Reasons for Accuracy:**  
  - Handles real-time updates efficiently.  
  - Works well with high-dimensional sparse data.  
  - Balances flexibility and stability.  
  - Robust against noise and incomplete data.  

### **4.3. Extreme Gradient Boosting (XGBoost)**  
- **Accuracy:** 87%  
- **Reasons for Accuracy:**  
  - Requires extensive hyperparameter tuning.  
  - May overfit on high-dimensional text data.  
  - Struggles with noisy text data.  
  - Designed for more complex objectives.  

### **4.4. Support Vector Machines (SVM)**  
- **Accuracy:** 80.43%  
- **Reasons for Accuracy:**  
  - Imbalanced dataset affected classification.  
  - Struggles with non-linear patterns in text data.  
  - Hyperparameter tuning affects performance.  
  - Computationally expensive for large datasets.  

### **4.5. Random Forest Classifier**  
- **Accuracy:** 90.13%  
- **Reasons for Accuracy:**  
  - Uses ensemble learning to improve generalization.  
  - Handles missing data and outliers effectively.  
  - Works well with high-dimensional text data.  
  - Reduces overfitting by averaging multiple trees.  

## **5. Comparison of Accuracy Scores**  
| Model | Accuracy (%) |  
| --- | --- |  
| Decision Tree | 80.43% |  
| Passive Aggressive | 93.16% |  
| XGBoost | 86.07% |  
| SVM | 83.43% |  
| Random Forest | 93.13% |  

### **5.1. Analysis of Accuracy Scores**  
#### **5.1.1. Passive Aggressive and Random Forest (Highest Accuracy)**  
- Passive Aggressive Classifier excels in handling sparse and high-dimensional data, making it ideal for fake news detection.  
- Its ability to perform incremental learning allows it to adapt to new data in real time.  
- Random Forest performs well due to ensemble learning, reducing overfitting and increasing generalization.  

## **6. Conclusion**  
This project successfully developed a machine learning-based fake news detection system, achieving high accuracy using the Passive Aggressive Classifier. The model effectively distinguishes between real and fake news using advanced text preprocessing, feature extraction, and classification techniques. Additionally, a Flask-based front-end allows users to interact with the system for real-time predictions.  

Future work could explore deep learning approaches, such as transformers, to further improve accuracy. Moreover, integrating a credibility score or explanation feature could enhance transparency and user trust.  

This project demonstrates the potential of AI in addressing societal challenges, ensuring the reliability of information in an era of widespread misinformation.

