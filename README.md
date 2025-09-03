# 🚀 SpaceX Data Science Capstone Project

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Python](https://img.shields.io/badge/python-3.9%2B-brightgreen.svg)
![Status](https://img.shields.io/badge/status-Completed-success.svg)

---

## 📝 Abstract
This project investigates the success of SpaceX Falcon 9 first-stage landings by applying **data science and machine learning techniques**. Using datasets collected from the SpaceX API and Wikipedia archives, the project explores the relationships between payload characteristics, booster versions, launch sites, and orbit types. Several supervised learning models were developed and evaluated, achieving an accuracy of approximately **85%** using Decision Tree models. The insights gained from this analysis can assist aerospace stakeholders in predicting launch outcomes and optimizing future missions.

---

## 📖 Introduction
SpaceX has revolutionized the aerospace industry with reusable rockets, significantly reducing the cost of space exploration. Predicting the success of Falcon 9 landings is a challenging yet valuable problem that combines engineering, data analysis, and predictive modeling.  
This project is a **capstone for the IBM Data Science Professional Certificate**, demonstrating expertise in:
- Data collection and wrangling  
- Exploratory data analysis (EDA)  
- Machine learning modeling  
- Dashboard visualization

---

## 🎯 Objectives
- Analyze and clean data from multiple sources for accuracy and consistency.  
- Explore key features influencing launch success rates.  
- Train and evaluate machine learning models for predictive accuracy.  
- Build a user-friendly dashboard for visualizing mission statistics.

---

## 🔬 Methodology
### 1️⃣ Data Collection
- Extracted data using the **SpaceX API** for mission details.
- Scraped complementary information from **Wikipedia**.

### 2️⃣ Data Wrangling
- Cleaned missing values and standardized categorical data.
- Engineered new features like "Orbit Class" and "Payload Weight Bins".

### 3️⃣ Exploratory Data Analysis (EDA)
- Used visualization tools like **matplotlib**, **seaborn**, and **plotly**.
- Analyzed patterns in payload mass, booster type, and success probability.

### 4️⃣ Model Development
- Implemented and tested the following algorithms:
  - Logistic Regression  
  - Decision Tree  
  - Support Vector Machine (SVM)  
  - K-Nearest Neighbors (KNN)
- Evaluated models based on:
  - Accuracy  
  - Precision & Recall  
  - Confusion Matrix

### 5️⃣ Dashboard Creation
- Developed a **Plotly Dash dashboard** to interactively visualize launch data.

---

## 📊 Results
| Model                  | Accuracy | Precision | Recall |
|-----------------------|----------|-----------|--------|
| Logistic Regression   | 80%      | 0.78      | 0.80   |
| Decision Tree         | **85%**  | 0.84      | 0.85   |
| Support Vector Machine| 83%      | 0.81      | 0.82   |
| KNN                   | 82%      | 0.80      | 0.81   |

Key findings:
- **Booster Version** significantly impacts landing success.
- **Payload Mass** and **Orbit Type** are strong predictors.
- **Launch Site** location plays a secondary but important role.

---


## 🗂 Repository Structure
SpaceX-Capstone-Project/
├── data/ # Raw and cleaned datasets
├── notebooks/ # Jupyter notebooks for EDA and model training
├── scripts/ # Python scripts for automation
├── dashboard/ # Interactive dashboard code
├── results/ # Reports, figures, and output metrics
└── README.md # Project documentation



---

## ⚙️ Technologies Used
- **Languages:** Python 3.9+
- **Libraries:** pandas, numpy, scikit-learn, matplotlib, seaborn, plotly, dash
- **Tools:** Jupyter Notebook, Git, IBM Watson Studio
- **Deployment:** Plotly Dash (local deployment)

---

## 🚀 Installation & Usage
To run the project locally:

```bash
# Clone the repository
git clone https://github.com/your-username/spacex-capstone.git
cd spacex-capstone

# Create and activate virtual environment
python -m venv venv
source venv/bin/activate   # Mac/Linux
venv\Scripts\activate      # Windows

# Install dependencies
pip install -r requirements.txt

# Launch the dashboard
python dashboard/app.py

