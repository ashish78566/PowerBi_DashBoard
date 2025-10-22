# 🧑‍💼 HR Analytics Dashboard  

## 📊 Project Overview  
The **HR Analytics Dashboard** is an interactive Power BI report designed to analyze employee attrition trends, workforce demographics, and compensation insights.  
The objective is to help HR teams identify the key factors driving attrition and support data-driven decisions for employee retention and organizational improvement.

---

## 🧠 Business Objectives  
- Combine multiple HR datasets into a unified **Employee Master Table**  
- Build a **data model** linking all relevant dimensions (Department, JobRole, Education, Salary Band, etc.)  
- Perform **data transformation** using Power Query  
- Create DAX measures for:  
  - Total Employees  
  - Attrition Count & Rate  
  - Average Age  
  - Average Salary  
  - Average Years of Service  
- Design an **interactive dashboard** with gender, department, and salary filters for deeper insights  

---

## ⚙️ Tech Stack  
- **Power BI** – Data Modeling | DAX | Visualization  
- **Power Query** – Data Cleaning & ETL  
- **Excel/CSV** – HR Data Sources  
- **DAX (Data Analysis Expressions)** – KPIs & Calculations  

---

## 📁 Folder Structure  
HR Analytics Dashboard/
│
├── Dashboard/
│ ├── HR_Analytics_Dashboard.pbix
│ ├── Screenshot 2025-10-22 122441.png
│ └── README.md
│
├── Datasets/
│ ├── Employee_Data.xlsx
│ ├── Department.csv
│ ├── JobRole.csv
│ └── Education.xlsx

yaml
Copy code

---

## 🖼️ Dashboard Preview  

### HR Analytics Power BI Dashboard  

Here’s a preview of the dashboard 👇  

![Dashboard Preview](https://github.com/ashish78566/PowerBi_DashBoard/blob/main/HR%20Analytics%20Dashboard/Dashboard/Screenshot%202025-10-22%20122441.png)

---

## 💡 Key Insights  
- **Total Employees:** 1,470  
- **Attrition Count:** 237  
- **Attrition Rate:** 16.1%  
- **Average Age:** 37 years  
- **Average Salary:** 6.5K  
- **Average Years of Service:** 7 years  
- **Top Departments by Attrition:** Sales, Research & Development  
- **Highest Attrition by Education:** Life Sciences (38%)  
- **Age Group Most Affected:** 26–35 years (highest attrition count)  
- **Salary Band Most Affected:** ≤5K  

---

## 🧩 Key DAX Measures  
```DAX
Total Employees = COUNTROWS(Employee)

Attrition Count = CALCULATE(COUNTROWS(Employee), Employee[Attrition] = "Yes")

Attrition Rate = DIVIDE([Attrition Count], [Total Employees], 0)

Average Age = AVERAGE(Employee[Age])

Average Salary = AVERAGE(Employee[MonthlyIncome])

Average Years = AVERAGE(Employee[YearsAtCompany])
🏆 Business Takeaways
Younger employees (26–35 years) show the highest attrition — focus on engagement & growth plans.

Most attrition occurs in Sales and Research departments.

Employees with ≤5K salary have significantly higher turnover rates.

Overall attrition rate (16.1%) indicates a moderate retention challenge requiring targeted strategies.

Data-driven HR insights can guide recruitment, retention, and development policies.

🔗 Project Repository
📁 View HR Analytics Dashboard on GitHub

👨‍💻 Author
Ashish
Data Analyst | Power BI Developer | Business Insights Enthusiast
