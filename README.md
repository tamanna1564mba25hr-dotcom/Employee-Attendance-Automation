# 📊 Employee Attendance & Performance Tracker
### AI Automation Project using n8n + Power BI

---

## 📌 Project Overview
This project demonstrates an automated **Employee Attendance Tracking System** using **n8n workflow automation** and **Power BI dashboards**.

The system processes employee attendance data stored in **Google Sheets**, applies rule-based logic to categorize employees based on attendance levels, and generates insights that help HR teams monitor workforce productivity.

---

## 🎯 Business Problem
HR departments often track employee attendance manually, which can be time-consuming and prone to errors.

The goal of this project is to:
- Automate attendance monitoring
- Categorize employees based on attendance
- Generate visual insights for HR decision-making

---

## 🗂 Dataset
The dataset is stored in **Google Sheets** and contains the following fields:

- Employee Name  
- Days Present  
- Days Absent  
- Tasks Completed  

### Example Dataset

| Employee Name | Days Present | Days Absent | Tasks Completed |
|---------------|-------------|-------------|----------------|
| Aditi | 22 | 3 | 18 |
| Rahul | 18 | 7 | 10 |
| Simran | 25 | 0 | 20 |
| Aman | 15 | 10 | 8 |
| Neha | 20 | 5 | 14 |
| Karan | 12 | 13 | 6 |

---

## ⚙ Rule-Based Logic
Employee attendance is categorized using simple rule-based logic:

- **High Attendance** → Days Present > 22  
- **Medium Attendance** → Days Present between 15 and 22  
- **Low Attendance** → Days Present < 15  

This logic is implemented using the **Switch Node in n8n**.

---

## 🔄 n8n Workflow Automation
The **n8n workflow** automates the processing of employee attendance data.

### Workflow Steps
1. Google Sheets Trigger – Reads employee data.
2. Set Node – Cleans and prepares the dataset.
3. Switch Node – Applies attendance rules.
4. Set Node – Adds attendance category.
5. Merge Node – Combines categorized data.
6. Google Sheets Node – Saves processed output.

### Workflow Structure
```
Google Sheets Trigger
        ↓
      Set Node
        ↓
    Switch Node
   /     |      \
High   Medium    Low
  ↓       ↓       ↓
 Set     Set     Set
    \     |     /
        Merge
          ↓
    Google Sheets Output
```

---

## 📊 Power BI Dashboard
The processed dataset is imported into **Power BI** to generate visual insights.

### Dashboard Visualizations
- 📊 Bar Chart – Employee attendance comparison
- 🥧 Pie Chart – Distribution of attendance categories
- 📈 KPI Indicators – Total employees and attendance insights

These dashboards help HR managers easily identify attendance patterns and employee performance trends.

---

## 📷 Project Screenshots

### n8n Workflow
![Workflow](workflow-screenshot.png)<img width="1578" height="683" alt="image" src="https://github.com/user-attachments/assets/191fe9ac-2dcc-4a5e-852c-16fd543d2291" />


### Power BI Dashboard
![Dashboard](powerbi-dashboard.png)
<img width="1321" height="728" alt="dashboard" src="https://github.com/user-attachments/assets/d88cf9f9-c9d8-4b72-8be3-18ca651397ee" />

---

## 📈 Key Insights
- Employees are automatically categorized into High, Medium, and Low attendance groups.
- HR teams can quickly identify employees with poor attendance.
- Automation reduces manual effort in tracking attendance data.
- Power BI dashboards make workforce analysis easier.

---

## 🔮 Future HR Insights
This project can be extended with advanced HR analytics features such as:

- Predicting employee performance using AI models
- Automatic HR alerts for low attendance employees
- Integration with employee performance metrics
- Workforce productivity analysis
- Smart HR decision-making dashboards

These enhancements can help organizations make **data-driven HR decisions in the future**.

---

## 🛠 Tools & Technologies
- **n8n** – Workflow automation
- **Google Sheets** – Dataset storage
- **Power BI** – Data visualization
- **GitHub** – Project documentation

---

## 🚀 Project Outcome
- Automated attendance categorization
- Processed employee dataset
- HR insights through visual dashboards
- Improved decision-making using data analytics

---

## 👩‍💻 Author
AI Business Application Project  
Employee Attendance & Performance Tracker
