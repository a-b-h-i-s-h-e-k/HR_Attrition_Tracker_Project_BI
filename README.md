
# HR Attrition Tracker 📊

An advanced Power BI project to visualize and analyze employee attrition patterns using the IBM HR Analytics dataset.

## 🔧 Project Overview

You're consulting for an HR team trying to reduce employee attrition. Your goal is to deliver an interactive dashboard that shows:
- Attrition patterns by Department, Job Role, Education
- Employee satisfaction insights
- High-risk employee segmentation
- Drill-through details by Job Role

---

## 🗂 Dataset

**Source**: IBM HR Analytics Employee Attrition  
**File Used**: HR_data.csv  
**Records**: 1470  
**Columns**: 35 (demographics, job info, satisfaction, performance, etc.)

---

## 💡 Key Features

### ✅ Power BI Skills Used
- Power Query: Conditional logic, reference tables
- Data Modeling: Star schema with fact & dimension tables
- DAX Measures: RANKX, SWITCH, segmentation
- Visualization: Tree maps, cards, matrix, heat maps, drill-throughs

### ✅ Calculated Columns
- `AgeGroup`: Young, Mid-Age, Senior, Veteran
- `SalaryLevel`: Low, Medium, High, Very High (based on quartiles)
- `HighRiskFlag`: Based on low job & environment satisfaction

### ✅ DAX Measures
- Attrition Count & Rate
- Average Satisfaction Score
- High Risk %
- Department Attrition Rank
- Attrition by JobRole (Dynamic Segmentation)
- Estimated Attrition Cost

---

## 📈 Dashboard Visuals

| Visual Type     | Purpose                                    |
|------------------|---------------------------------------------|
| Bar Chart        | Attrition by Department, JobRole            |
| Line Chart       | Attrition by YearsAtCompany (trend)         |
| Tree Map         | Attrition % by AgeGroup or JobRole          |
| Heat Map (Matrix)| Satisfaction scores by Dept and Role        |
| Cards            | KPIs: Attrition Rate, High Risk %, Avg Sat |
| Slicers          | AgeGroup, SalaryLevel, EducationField       |
| Drill-Through    | Details by JobRole                          |

---

## 🔍 Predictive Insights

- Identify which roles or departments have the highest risk of attrition
- Correlate satisfaction with risk %
- Simulate cost of attrition using DAX

```DAX
Estimated Attrition Cost = [Attrition Count] * 10000
```

---

## 📂 Folder Structure

```
├── HR_data.csv
├── HR_Attrition_Tracker.pbix
└── README.md
```

---

## 🚀 Getting Started

1. Open the `.pbix` file in Power BI Desktop
2. Load `HR_data.csv` if needed
3. Review the Data Model and DAX logic
4. Interact with slicers, visuals, and drill-through pages

---


