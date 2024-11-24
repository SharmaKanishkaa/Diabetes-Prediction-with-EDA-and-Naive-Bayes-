# 🍩 **Diabetes Prediction with EDA and Naive Bayes**

This project is designed to predict whether a patient has diabetes based on various health attributes using machine learning. The dataset contains medical data from patients, including both dependent and independent variables that help determine diabetes risk.

---

## 📋 **Dataset Overview**  

The dataset consists of **768 observations** and **8 numerical independent variables** that are used to predict the presence or absence of diabetes (dependent variable). The target variable `Outcome` takes the value of **1** for a positive diabetes diagnosis and **0** for a negative diagnosis.

### **Columns**  
| **Feature**               | **Description**                                      |  
|---------------------------|------------------------------------------------------|  
| `Pregnancies`             | Number of times the person has been pregnant.        |  
| `Glucose`                 | Plasma glucose concentration during an oral glucose tolerance test. |  
| `BloodPressure`           | Diastolic blood pressure (mm Hg).                    |  
| `SkinThickness`           | Triceps skin fold thickness (mm).                    |  
| `Insulin`                 | 2-Hour serum insulin (mu U/ml).                      |  
| `BMI`                     | Body mass index (weight in kg / height in m²).       |  
| `DiabetesPedigreeFunction`| A function that scores the genetic predisposition to diabetes. |  
| `Age`                     | Age of the patient.                                  |  
| `Outcome`                 | Target variable indicating diabetes status (1 for positive, 0 for negative). |

---

## 📊 **Exploratory Data Analysis (EDA)**  

1. **Data Preprocessing:**  
   - The data was cleaned by handling any missing values and ensuring no discrepancies in the data.
   
2. **Visualizations:**  
   - Generated multiple plots to visualize the data and relationships between features:  
     - **Histograms** to visualize the distribution of each feature.
     - **Box plots** to check for outliers.
     - **Correlation matrix heatmap** to visualize the relationships between the features.
     - **3D plot** for a deeper understanding of how different features interact in relation to the `Outcome` variable.  

---

## 🧠 **Modeling with Naive Bayes**  

1. **Initial Accuracy:**  
   - The model was first trained using **Naive Bayes** and yielded an accuracy of **78%**.  
   
2. **Model Improvement with Cross-Validation:**  
   - The model was further optimized using **K-Fold Cross-Validation**, which improved the accuracy to **80%**.  

---

## 🎯 **Results**  

- **Naive Bayes Accuracy:** 78%  
- **After K-Fold Cross-Validation:** 80%  

While the Naive Bayes model provides a good baseline accuracy of 78%, utilizing K-fold cross-validation improves the model's robustness and accuracy, providing more reliable results.

---

## 🛠️ **Tools and Techniques**  

- **Libraries Used:** `pandas`, `NumPy`, `Matplotlib`, `Seaborn`, `sklearn`  
- **Model:**  
  - **Naive Bayes Classifier:** A probabilistic classifier based on Bayes' theorem, suitable for predicting binary outcomes like diabetes status.  
  - **K-Fold Cross-Validation:** A technique for improving the reliability of the model by splitting the dataset into multiple training and testing sets.

---

## ✨ **Key Takeaways**  

- **EDA** plays a crucial role in understanding the dataset's distribution and relationships between variables, allowing for better model optimization.
- **Naive Bayes** offers a simple yet effective approach for binary classification tasks, especially when working with normally distributed data.
- **K-Fold Cross-Validation** is essential for improving model accuracy and ensuring that the model generalizes well to unseen data.
