# 📊 Eating Out vs Health -- Power BI Project

## 📌 Project Overview

This project analyzes how eating out frequency impacts health indicators
like BMI, cholesterol, blood pressure, and overall health score using
Power BI.

------------------------------------------------------------------------

## 🎯 Objectives

-   Analyze eating habits vs health outcomes
-   Identify high-risk groups
-   Provide actionable insights using dashboards

------------------------------------------------------------------------

## 🛠️ Step-by-Step Implementation

### 1. Data Import & Cleaning

-   Load CSV into Power BI
-   Check data types
-   Handle missing/null values
-   Convert categorical fields properly

### 2. Data Modeling

-   Keep single table or create:
    -   Demographics
    -   Lifestyle
    -   Health
-   Create relationships if split

### 3. Create DAX Measures

-   Avg_BMI = AVERAGE(BMI)
-   Avg_Health_Score = AVERAGE(Health_Score)
-   Diabetes\_% = DIVIDE(COUNTROWS(FILTER(Data, Diabetes="Yes")),
    COUNTROWS(Data))
-   High_Risk_Count = COUNTROWS(FILTER(Data, Health_Score \< 50))

### 4. KPI Cards

-   Avg Eat-Out Frequency
-   Avg Health Score
-   \% Diabetes
-   \% Hypertension

### 5. Visualizations

-   Bar: Eat-Out Frequency vs Avg BMI
-   Stacked Column: Eat-Out Type vs Cholesterol
-   Scatter: Calories vs Health Score
-   Line: Eat-Out vs Health Score (Age)
-   Pie: Eat-Out Type Distribution

### 6. Conditional Formatting

-   Health Score \< 50 → Red
-   Cholesterol → Green/Yellow/Red

------------------------------------------------------------------------

## 📊 Dashboard Layout

### Page 1: Overview

-   KPI Cards (Top)
-   Pie Chart (Left)
-   Bar Chart (Right)

### Page 2: Trends

-   Scatter Plot (Center)
-   Line Chart (Bottom)

### Page 3: Demographics

-   Stacked Column (Top)
-   Filters/Slicers (Side)

------------------------------------------------------------------------

## 💡 Insights

-   High eating frequency → higher BMI
-   Fast food → lower health score
-   Exercise reduces negative impact

------------------------------------------------------------------------

## 🚀 Tools Used

-   Power BI
-   DAX
-   Data Modeling
