# 📊 User Behavior Analysis and Path Mining Project

## 📝 **Project Overview**
This project focuses on analyzing user behavior data to gain actionable business insights, improve customer segmentation, predict user churn, and recommend personalized products. By leveraging various data mining techniques, the project aims to enhance user engagement, increase conversion rates, and optimize marketing strategies.

## 🎯 **Objectives**
- Develop comprehensive **user profiles** using demographic and behavioral data.
- Perform **user segmentation** via clustering to identify key customer groups.
- Predict **user churn** to proactively retain valuable customers.
- Design an **item recommendation system** tailored to user preferences.
- Visualize **user behavior paths** to identify key drop-off points in the user journey.
- Provide **data-driven business insights** to inform marketing and product strategies.

---

## 📥 **Data Description & Key Indicators**
The analysis utilizes the following data attributes to address business questions and drive insights:

| **Feature** | **Description** | **Usage in Analysis** |
|-------------|-----------------|-----------------------|
| `User_ID` | Unique identifier for each user | Tracking and user-specific analysis |
| `Age` | Age of the user | Demographic segmentation, age-based preference analysis |
| `Gender` | Gender of the user | Gender-specific targeting and recommendations |
| `Location` | Suburban, rural, or urban | Geographical segmentation and preference analysis |
| `Income` | User's income level | Purchasing power assessment, pricing strategies |
| `Interests` | User interests (sports, fashion, technology, etc.) | Personalized content and product recommendations |
| `Last_Login_Days_Ago` | Days since last login | Engagement analysis and churn prediction |
| `Purchase_Frequency` | User's purchase frequency | Shopping habit analysis and loyalty segmentation |
| `Average_Order_Value` | Average value of orders | Promotion and pricing strategy optimization |
| `Total_Spending` | Total spending amount | Lifetime value (LTV) analysis and segmentation |
| `Product_Category_Preference` | Preferred product categories | Customized recommendation systems |
| `Time_Spent_on_Site_Minutes` | Session duration on the platform | Engagement level measurement |
| `Pages_Viewed` | Number of pages viewed per visit | Browsing behavior and interest analysis |
| `Newsletter_Subscription` | Newsletter subscription status | Targeted marketing and engagement strategies |

---

## 🗂️ **Project Structure**
```
📦 user_behavior_analysis
├── 📁 data                # Data files (raw, cleaned, processed)
│   ├── raw_data.csv       # Raw user behavior data (to be filled by user)
│   ├── cleaned_data.csv   # Processed and cleaned data
├── 📁 notebooks           # Jupyter Notebooks for step-by-step analysis
│   ├── eda.ipynb          # Exploratory Data Analysis
│   ├── segmentation.ipynb # User segmentation and clustering
│   ├── churn_model.ipynb  # Churn prediction modeling
│   ├── recommendation.ipynb # Personalized recommendation system
├── 📁 scripts             # Python scripts for data processing and modeling
├── 📁 visuals             # Visualization outputs (charts, diagrams)
├── 📄 requirements.txt    # Project dependencies
├── 📄 README.md           # Project documentation
└── 📄 report.pdf          # Final project report with insights and recommendations
```

---

## 🛠️ **Technologies & Libraries**
- **Programming Language:** Python 3.x  
- **Data Manipulation:** Pandas, NumPy  
- **Machine Learning:** Scikit-Learn, XGBoost, LightGBM  
- **Visualization:** Matplotlib, Seaborn, Plotly  
- **Clustering Algorithms:** K-Means, Hierarchical Clustering  
- **Recommendation System:** Content-based filtering  
- **Model Interpretation:** SHAP, LIME  
- **Visualization Tools:** Power BI, Tableau *(optional for dashboards)*

---

## 📊 **Methodology & Steps**

### 🚀 **1. Exploratory Data Analysis (EDA)**
- Analyze demographic data (Age, Gender, Location, Income)
- Explore user engagement metrics (Last_Login_Days_Ago, Time_Spent_on_Site_Minutes, Pages_Viewed)
- Examine purchasing patterns (Purchase_Frequency, Average_Order_Value, Total_Spending)
- Visualize product and category preferences with respect to user interests

### 🧹 **2. Data Preprocessing & Feature Engineering**
- Handle missing values and outliers
- Encode categorical variables (Gender, Location, Interests, Product_Category_Preference)
- Scale numerical features (Income, Total_Spending, Average_Order_Value)
- Create new features:
  - **Activity Score:** Based on login frequency and session duration
  - **Engagement Ratio:** Pages viewed per minute on the platform
  - **Spending Capacity:** Ratio of Total_Spending to Income

### 🧭 **3. User Segmentation (Clustering)**
- Apply **K-Means** and **Hierarchical Clustering** using features like Purchase_Frequency, Average_Order_Value, and Engagement Ratio
- Interpret clusters and develop **user personas** such as "High-Value Customers", "Potential Buyers", and "Infrequent Users"
- Visualize clusters with scatter plots and radar charts

### 🔍 **4. Churn Prediction Modeling**
- Define churn label based on `Last_Login_Days_Ago` and `Purchase_Frequency`
- Train machine learning models (Random Forest, XGBoost) to predict churn probability
- Analyze feature importance and interpret results with **SHAP values**

### 📦 **5. Personalized Recommendation System**
- Use `Product_Category_Preference` and `Interests` for content-based product recommendations
- Develop a ranking system to recommend top categories/products for each user segment
- Evaluate recommendation relevance through engagement metrics

### 📢 **6. Business Insights & Visualization**
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
