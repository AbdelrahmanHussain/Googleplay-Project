# 📱 Google Play Store Apps Data Cleaning & Preprocessing

## 📌 Introduction
The Google Play Store hosts millions of applications, and the data associated with these apps offers significant potential for analysis.  
Developers, researchers, and businesses can leverage this data to:
- Understand market trends
- Optimize their applications
- Maximize user engagement  

In this project, I focused on **data cleaning and preprocessing** for the Play Store Apps dataset.  
The main goal was to fix inconsistencies, handle missing values, detect outliers, and prepare the dataset for further analysis or machine learning tasks.

---

## 
Dataset Description
The dataset contains various details about apps on the Google Play Store.  

| Column Name       | Description                                                                 |
|-------------------|-----------------------------------------------------------------------------|
| **App**           | Name of the application                                                     |
| **Category**      | Category the app belongs to                                                 |
| **Rating**        | Overall user rating (as when scraped)                                       |
| **Reviews**       | Number of user reviews                                                      |
| **Size**          | Size of the app (as when scraped)                                           |
| **Installs**      | Number of user installs/downloads                                           |
| **Type**          | Whether the app is Paid or Free                                             |
| **Price**         | Price of the app (as when scraped)                                          |
| **Content Rating**| Age group the app is targeted at (e.g., Everyone, Mature 21+, etc.)         |
| **Genres**        | App can belong to multiple genres                                           |
| **Android Version** | Minimum Android version required                                          |

---

## 🛠️ Data Cleaning Tasks

The following cleaning and preprocessing tasks were performed:

1. **Fix `Rating`**  
   - Converted to numeric values  
   - Handled invalid or missing ratings  

2. **Fix `Size`**  
   - Converted sizes from strings (e.g., "10M", "1.2k") to numeric (in MB)  

3. **Fix `Price`**  
   - Removed currency symbols  
   - Converted price column to float  

4. **Fix `Category`**  
   - Standardized category names  
   - Removed invalid or duplicate entries  

5. **Fix `Android Version`**  
   - Extracted numeric version values  
   - Handled missing or invalid entries  

6. **Handle Missing Values**  
   - Imputed or dropped rows with missing data based on context  

7. **Outlier Detection & Handling**  
   - Detected extreme values in columns like `Reviews`, `Installs`, and `Price`  
   - Treated them using statistical methods (IQR, z-score)  

8. **General Fixes**  
   - Removed duplicates  
   - Ensured consistent formatting across all columns  

---

## 📈 Insights & Outcomes
- The dataset is now clean, consistent, and ready for analysis or machine learning.  
- Preprocessing allowed extraction of meaningful insights such as:
  - Distribution of app ratings
  - Relationship between installs and reviews
  - Market trends by category and content rating  

---

## 🚀 Next Steps
- Perform **Exploratory Data Analysis (EDA)**  
- Apply **Machine Learning models** for predictions (e.g., predicting rating or installs)  
- Visualize trends with charts and dashboards  

---

## 📂 Repository Structure
