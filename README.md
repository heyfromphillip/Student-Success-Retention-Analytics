# Student Success & Retention Analytics Hub 🎓

## 🎯 Project Objective
[cite_start]The "Student Success & Retention Analytics Hub" is a strategic management tool designed to help university administrators improve student outcomes[cite: 2]. This project answers three vital questions:
* [cite_start]**Who is most at risk?** Identifying students likely to drop out before completing their program[cite: 4, 5].
* [cite_start]**Where are the equity gaps?** Finding disparities in success between "Widening Participation" (WP) students and their peers[cite: 6, 7].
* [cite_start]**Which courses need intervention?** Pinpointing specific subjects where pass rates and grades are falling below standards[cite: 8, 9].

---

## 📊 Key Insights & Findings
* [cite_start]**Retention Overview:** The current retention rate stands at **49%**, with a **7% gap** identified in the Widening Participation group[cite: 41].
* [cite_start]**Departmental Performance:** **Journalism** leads with the highest pass rate (**70.4%**), while **Nursing** requires the most intervention (**54.8%**)[cite: 42].
* [cite_start]**Geographic Risk:** **Rural students** show a higher density of "High Risk" status compared to Urban counterparts[cite: 43].

---

## 🛠️ Technical Workflow

### 1. Data Engineering (Excel)
[cite_start]Before importing into Power BI, I performed feature engineering in Excel to create more meaningful business metrics[cite: 17]:
* [cite_start]**Pass Rate %:** Calculated as `(Approved Units / Evaluated Units) * 100`, capped at 100%[cite: 18].
* [cite_start]**Student Status:** Categorized students as **"Continued"** or **"Withdrew"**[cite: 19].
* [cite_start]**Academic Performance:** Binned GPA scores into **"High" (≥3.5)**, **"Medium" (≥2.5)**, and **"Low"**[cite: 20].
* [cite_start]**Student Risk Profile:** Developed a 3-tier assessment (High, Medium, Low) based on withdrawal status and pass rates[cite: 21, 22, 23, 24].
* [cite_start]**WP Indicator:** Identified the "Widening Participation" (WP) group based on parental education, employment, and residency[cite: 25].

### 2. Analytics & UI (Power BI)
* [cite_start]**Data Modeling:** Built a star-schema inspired model with custom measures[cite: 30, 31, 32].
* [cite_start]**DAX Metrics:** Created key measures including **Retention Rate %**, **WP Retention Gap**, and **Average Pass Rate**[cite: 33, 34, 35].
* [cite_start]**Visual Strategy:** * **KPI Cards:** High-level summary of retention and risk metrics[cite: 37].
    * [cite_start]**Performance Matrix:** Used quadrant analysis to compare **Pass Rate vs. Average Grade** by course[cite: 38].
    * [cite_start]**Risk Treemap:** Visualized the distribution of student risk by geographic location[cite: 39].



---

## 🚀 How to Use
1. **Download** the `Retention_dashboard.pbix` file from this repository.
2. **Open** it in Power BI Desktop to explore interactive filters.
3. **Navigate** using the custom Sidebar Panel to filter by Course, Gender, or Employment status.
4. **Reset** all views instantly using the **"Clear all slicers"** button at the bottom of the panel.
