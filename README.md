 Operations Analytics using AI
##  Project Overview
This project demonstrates how **Artificial Intelligence can be applied to Operations Analytics** to support better decision-making in supply chain and inventory management.

Using **machine learning techniques**, the notebook analyzes operational data to **predict product demand and identify potential stock shortages**. Based on the prediction results, the system generates **automated reorder recommendations** to help operations managers take proactive actions.

This lab illustrates how **data-driven decision making** can improve operational efficiency and reduce the risk of inventory shortages.

---

##  Objectives

* Apply **AI and Machine Learning** to operations analytics
* Perform **data preprocessing and preparation**
* Train a **Decision Tree Regression model** to predict demand
* Evaluate the model using performance metrics
* Generate **inventory shortage risk levels**
* Provide **automated reorder recommendations**

---

## Tools & Technologies Used

The following tools and technologies were used in this project:

* **Python**
* **Jupyter Notebook**
* **Pandas** – Data manipulation and analysis
* **NumPy** – Numerical operations
* **Matplotlib** – Data visualization
* **Scikit-learn** – Machine learning modeling

 **AI Tool Used:** ChatGPT was used for assistance in structuring code, explanations, and documentation.

---

##  Project Structure

```
Lab24-Operations-Analytics-AI/
│
├── Lab_24_Operations_Analytics_using_AI.ipynb
├── README.md
```

---

##  Project Workflow

### 1️. Import Required Libraries

Libraries for data handling, visualization, machine learning, and evaluation were imported.

Examples:

* Pandas
* NumPy
* Matplotlib
* Scikit-learn modules

---

### 2️. Data Preparation

Operational data such as:

* Product ID
* Product Category
* Inventory Level
* Demand
* Supply Lead Time

was prepared and organized for analysis.

---

### 3️. Data Preprocessing

Before training the model:

* Categorical variables were encoded using **LabelEncoder**
* Data was split into **training and testing sets**
* Features and target variables were defined

---

### 4️. Model Training

A **Decision Tree Regressor** model was trained to predict product demand.

```
DecisionTreeRegressor()
```

This model learns patterns from historical operational data.

---

### 5️. Model Evaluation

Model performance was evaluated using:

* **Mean Absolute Error (MAE)**
* **Mean Squared Error (MSE)**
* **R² Score**

These metrics help measure prediction accuracy.

---

### 6️. Risk Classification

Based on predicted demand and inventory levels, products were classified into:

* 🔴 **High Risk**
* 🟠 **Medium Risk**
* 🟢 **Low Risk**

This helps identify potential inventory shortages.

---

### 7️. Reorder Recommendation System

The notebook generates operational recommendations:

| Risk Level  | Action            |
| ----------- | ----------------- |
| High Risk   | Urgent Reorder    |
| Medium Risk | Plan Reorder Soon |
| Low Risk    | Monitor Normally  |

Example logic:

```python
def reorder_action(risk):
    if risk == "High Risk":
        return "Urgent Reorder"
    elif risk == "Medium Risk":
        return "Plan Reorder Soon"
    else:
        return "Monitor Normally"
```

---

## 📊 Expected Output

The final dataset includes:

* Product ID
* Predicted Demand
* Shortage Risk Level
* Reorder Action Recommendation

This helps businesses **prevent stockouts and optimize inventory management**.

---

##  How to Run the Project

1. Clone the repository

```
git clone https://github.com/your-username/Lab24-Operations-Analytics-AI.git
```

2. Open the notebook

```
Lab_24_Operations_Analytics_using_AI.ipynb
```

3. Run all cells in **Jupyter Notebook or Google Colab**

---

##  Learning Outcomes

After completing this lab, you will understand:

* How **AI supports operations analytics**
* How to **build predictive models for business decisions**
* How machine learning can improve **inventory and supply chain planning**
---
##  Author
Harshita
