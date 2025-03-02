# User Behavior Analysis and Path Mining Project

## **Project Overview**
This project focuses on analysing user behaviour data to gain actionable business insights, improve customer segmentation and predict customer churn. Using a range of data mining and statistical techniques, the project aims to increase customer engagement, improve conversion rates and optimise marketing strategies.

## **Objectives**
- Use demographic, behavioural and transactional data to build a comprehensive **customer profile**.
- Perform **exploratory data analysis (EDA)** to identify key indicators and discover hidden data patterns.
- Visualise **customer behaviour paths** to identify churn points and improve the overall user experience.
- Perform **customer segmentation** through cluster analysis to identify different customer groups and tailor marketing strategies.
- Predict **customer churn** using supervised learning models to develop corresponding retention strategies.
- Provide **data-driven business insights** to support marketing and product development decisions.

---

## 📥 **Data Description & Key Indicators**
The analysis utilizes the following data attributes to address business questions and drive insights:

| **Feature** | **Description** |
|-------------|-----------------|
| `User_ID` | Unique identifier for each user |
| `Age` | Age of the user |
| `Gender` | Gender of the user |
| `Location` | Suburban, rural, or urban |
| `Income` | User's income level |
| `Interests` | User interests (sports, fashion, technology, etc.) |
| `Last_Login_Days_Ago` | Days since last login |
| `Purchase_Frequency` | User's purchase frequency |
| `Average_Order_Value` | Average value of orders |
| `Total_Spending` | Total spending amount |
| `Product_Category_Preference` | Preferred product categories |
| `Time_Spent_on_Site_Minutes` | Session duration on the platform |
| `Pages_Viewed` | Number of pages viewed per visit |
| `Newsletter_Subscription` | Newsletter subscription status |

---

## **Project Structure**
```
User_Behavior_Analysis
├── 📁 Data                                  # Data files (raw, cleaned, processed)
│   ├── user_personalized_features.csv       # Raw user behavior data
│   ├── cleaned_data.csv                     # Processed and cleaned data
├── 📁 Notebooks                             # Jupyter Notebooks for step-by-step analysis
│   ├── EDA.ipynb                            # Exploratory Data Analysis
│   ├── Cluster Analysis.ipynb                   # User segmentation and clustering
│   ├── Chure Prediction Model.ipynb         # Churn prediction modeling
├── 📁 Plots                                # Visualization outputs (Charts, Diagrams)
├── 📄 README.md                              # Project documentation
└── 📄 Report.pdf                             # Final project report with insights and recommendations
```

---

## **Technologies & Libraries**
- **Programming Language:** Python 3.10.14 
- **Data Manipulation:** Pandas, NumPy  
- **Machine Learning:** Scikit-Learn, XGBoost 
- **Visualization:** Matplotlib, Seaborn, plotly
- **Clustering Algorithms:** K-Means
- **Visualization Tools:** Power BI, Tableau

---

## **Methodology & Steps**

### **1. Data Preprocessing
- Handle missing values and outliers (if any)

### **2. Exploratory Data Analysis (EDA)**
- Analyse demographic characteristics (age, gender, income, location) and behavioural indicators (log-in frequency, purchase frequency, website browsing, etc.).
- Determine correlations between characteristics and detected outliers, so as to prepare for feature engineering.
- Visualise key indicators to understand user distribution and behaviour trends.

### **3. Feature Engineering**
- Encode categorical variables (Gender, Location, Interests, Product_Category_Preference)
- Scale numerical features (Income, Total_Spending, Average_Order_Value)
- Create new features:
  - **Activity Score:** Based on login frequency and session duration

### **4. User Segmentation (Clustering)**
- Apply **K-Means** and **Hierarchical Clustering** using features like Purchase_Frequency, Average_Order_Value, and Engagement Ratio
- Interpret clusters and develop **user personas** such as "High-Value Customers", "Potential Buyers", and "Infrequent Users"
- Visualize clusters with scatter plots and radar charts

### **5. Churn Prediction Modeling**
- Define churn label based on `Last_Login_Days_Ago` and `Purchase_Frequency`
- Train different machine learning models (Random Forest, XGBoost) to predict churn probability
- Analyze feature importance and interpret results with **SHAP values**

### **6. Business Insights & Visualization**
- Create **Sankey diagrams** to analyze user behavior paths from browsing to purchase
- Develop **conversion funnel visualizations** highlighting key drop-off points
- Use **dashboard tools** (Power BI/Tableau) to present insights interactively

---

## 📈 **Sample Visualizations**
- 📊 **Age vs. Total Spending Scatter Plot**: Identifies spending trends across age groups  
- 🗺️ **Geographical Heatmap**: Visualizes purchasing patterns across locations  
- 🕸️ **Sankey Diagram**: Maps user behavior paths from browsing to checkout  
- 📉 **Churn Risk Distribution**: Highlights high-risk users for targeted retention strategies  

---

## 📢 **Business Insights & Recommendations**
- 🎯 **High-Value Users (20%)** contribute to **65% of total revenue** → Prioritize with exclusive offers.
- 🛒 **Potential Buyers** browse frequently but seldom purchase → Implement targeted promotions and reminders.
- 📬 **Non-subscribers** with high spending potential → Encourage newsletter sign-ups for better engagement.
- 🚪 **Churn-risk users** show inactivity beyond 30 days → Recommend re-engagement campaigns.

---

## 🏗️ **How to Run the Project**
1. Clone the repository:
```bash
git clone https://github.com/your-username/user_behavior_analysis.git
cd user_behavior_analysis
```
2. Install dependencies:
```bash
pip install -r requirements.txt
```
3. Place your dataset in the `data/` directory as `raw_data.csv`.
4. Run the Jupyter Notebooks under `notebooks/` in sequence for analysis.
5. Review the visual outputs in the `visuals/` folder and the final insights in `report.pdf`.

---

## 📝 **Future Enhancements**
- Integrate **real-time behavior tracking** for dynamic churn prediction and recommendations.
- Explore **deep learning approaches** (RNNs, Transformers) for sequential user behavior modeling.
- Expand to include **social media sentiment analysis** for holistic user profiling.
- Develop a **web-based dashboard** for live data monitoring and business reporting.

---

## 👨‍💻 **Contributors**
- Kartikey Bartwal – Data Scientist & Data Provider 

---

## 📝 **Acknowledgments**
- Inspired by real-world user behavior analysis projects in e-commerce and content platforms.  
- Data sourced from Kaggle: https://www.kaggle.com/datasets/kartikeybartwal/ecommerce-product-recommendation-collaborative/data.   

---
