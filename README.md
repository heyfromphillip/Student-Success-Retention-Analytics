# Student Success & Retention Analytics Hub 🎓

## 🎯 Project Objective
The "Student Success & Retention Analytics Hub" is a strategic management tool designed to help university administrators improve student outcomes. This project answers three vital questions:
**Who is most at risk?** Identifying students likely to drop out before completing their program.
**Where are the equity gaps?** Finding disparities in success between "Widening Participation" (WP) students and their peers.
**Which courses need intervention?** Pinpointing specific subjects where pass rates and grades are falling below standards.


---

## 📊 Key Insights & Findings
**Retention Overview:** The current retention rate stands at **49%**, with a **7% gap** identified in the Widening Participation group.
**Departmental Performance:** **Journalism** leads with the highest pass rate (**70.4%**), while **Nursing** requires the most intervention (**54.8%**).
**Geographic Risk:** **Rural students** show a higher density of "High Risk" status compared to Urban counterparts.

<img width="659" height="364" alt="image" src="https://github.com/user-attachments/assets/7337bb02-4f44-4c59-8035-5418db35abae" />

---

## 🛠️ Technical Workflow

### 1. Data Engineering (Excel)
Before importing into Power BI, I performed feature engineering in Excel to create more meaningful business metrics:
* **Pass Rate %:** Calculated as `(Approved Units / Evaluated Units) * 100`, capped at 100%.
* **Student Status:** Categorized students as **"Continued"** or **"Withdrew"**.
* **Academic Performance:** Binned GPA scores into **"High" (≥3.5)**, **"Medium" (≥2.5)**, and **"Low"**.
* **Student Risk Profile:** Developed a 3-tier assessment (High, Medium, Low) based on withdrawal status and pass rates.
* **WP Indicator:** Identified the "Widening Participation" (WP) group based on parental education, employment, and residency.

### 2. Analytics & UI (Power BI)
**Data Modeling:** Built a star-schema inspired model with custom measures.
**DAX Metrics:** Created key measures including **Retention Rate %**, **WP Retention Gap**, and **Average Pass Rate**.
**Visual Strategy:** * **KPI Cards:** High-level summary of retention and risk metrics.
    * **Performance Matrix:** Used quadrant analysis to compare **Pass Rate vs. Average Grade** by course.
    * **Risk Treemap:** Visualized the distribution of student risk by geographic location.



---

## 🚀 How to Use
1. **Download** the `Retention_dashboard.pbix` file from this repository.
2. **Open** it in Power BI Desktop to explore interactive filters.
3. **Navigate** using the custom Sidebar Panel to filter by Course, Gender, or Employment status.
