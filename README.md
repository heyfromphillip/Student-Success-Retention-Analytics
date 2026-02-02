# Student Success & Retention Analytics Hub 🎓

## 📌 Project Overview
The **Student Success & Retention Analytics Hub** is a strategic management tool designed to help university administrators improve student outcomes. This project answers three vital questions:
1. **Who is most at risk?** Identifying students likely to drop out before completing their program.
2. **Where are the equity gaps?** Finding disparities in success between "Widening Participation" (WP) students and their peers.
3. **Which courses need intervention?** Pinpointing specific subjects where pass rates and grades are falling below standards.

---

## 🌟 The STAR Journey

### **Situation**
University retention is a complex challenge influenced by academics, geography, and socioeconomic status. With a 2021 dataset of 500 students, the goal was to find the "why" behind student dropouts which were previously hidden in raw records.

### **Task**
My objective was to transform raw demographic and academic records into a single "Source of Truth" to prioritize institutional support and identify at-risk patterns.

### **Action**
I executed a multi-stage data lifecycle to build this solution:
* **Data Engineering (Excel):** Engineered six strategic metrics to add business meaning, including a **WP Indicator** to track equity and a **3-tier Risk Profile** (High, Medium, Low).
* **Data Modeling (Power BI):** Built a star-schema inspired model and created advanced DAX measures like **Retention Rate %** and **WP Retention Gap**.
* **Visual Logic:** Implemented a **Quadrant Performance Matrix** (Scatter Plot) and a **Risk Treemap** to visualize geographic vulnerabilities.


### **Result**
The final dashboard provides high-impact insights for institutional change:
* **Equity Insight:** Identified a **7% Retention Gap** in the Widening Participation (WP) group.
* **Course Optimization:** Pinpointed **Journalism** as the top performer (**70.4%**) and **Nursing** as the highest priority for review (**54.8%**).
* **Geographic Risk:** Discovered a higher density of "High Risk" students in **Rural** areas compared to Urban centers.

---

## 🛠️ Technical Implementation

### **1. Data Preparation (Excel)**
Before importing to Power BI, I created meaningful KPIs:
* **Pass Rate %:** `(Approved Units / Evaluated Units) * 100`.
* **Academic Performance:** Binned GPA into **High (≥3.5)**, **Medium (≥2.5)**, and **Low**.
* **Student Risk:** Categorized based on withdrawal status and pass rates (<75% for "At Risk").
* **WP Indicator:** Flagged students based on parental education, employment, and rural residency.

### **2. Power BI Workflow**
* **Power
