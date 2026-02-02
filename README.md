Project Overview
The "Student Success & Retention Analytics Hub" is a strategic management tool designed to help university administrators improve student outcomes. This project answers three vital questions:
1.	Who is most at risk? 
Identifying students likely to drop out before completing their program.
2.	Where are the equity gaps? 
Finding disparities in success between "Widening Participation" (WP) students and their peers.
3.	Which courses need intervention? 
Pinpointing specific subjects where pass rates and grades are falling below standards.
The Data
The dataset was sourced from Kaggle and contains demographic, socioeconomic, and academic performance metrics for the year 2021.
Key Features:
•	Demographics: Age, Gender, Marital Status, and Residence Location (Urban, Suburban, Rural).
•	Socioeconomic Factors: Parental Education, Income Level, and Regional Economic indicators (GDP, Inflation).
•	Academic Metrics: Units Enrolled, Approved, and Evaluated, alongside GPA-scale Average Grades.
Excel (Data Engineering)
Before importing into Power BI, I performed feature engineering in Excel to create more meaningful business metrics:
Pass Rate %: Calculated as (Approved Units / Evaluated Units) * 100, capped at 100%.
Student Status: Categorized students as "Continued" or "Withdrew".
Academic Performance: Binned GPA scores into "High" (≥3.5), "Medium" (≥2.5), and "Low".
Student Risk Profile: A logic-based risk assessment:
	High: Students who already withdrew.
	Medium: Active students with a Pass Rate < 75% ("At Risk").
	Low: Active students with a Pass Rate ≥ 75%.
WP Indicator: Identified the "Widening Participation" (WP) group based on parental education, employment, and rural residency.
Power BI Workflow
1. Data Transformation (Power Query)
•	Cleaned and profiled the data to ensure accuracy.
•	Standardized text formats and handled null values.
2. Data Modelling & DAX
•	Built a star-schema inspired model.
Key Measures Created:
•	Retention Rate %: Using DIVIDE and CALCULATE to track the percentage of continued students.
•	WP Retention Gap: Measuring the difference in success between WP and Non-WP groups.
•	Average Pass Rate: Aggregate performance across departments.
3. Visualization Strategy
•	KPI Cards: High-level executive summary of retention and risk.
•	Performance Matrix (Scatter Plot): Used a quadrant analysis to compare Pass Rate vs. Average Grade by course.
•	Risk Treemap: A nested visualization showing the distribution of student risk by geographic location.
Key Insights
•	Retention Overview: The current retention rate stands at 49%, with a 7% gap identified in the Widening Participation group.
•	Departmental Performance: Journalism leads with the highest pass rate (70.4%), while Nursing requires the most intervention (54.8%).
•	Geographic Risk: Rural students show a higher density of "High Risk" status compared to Urban counterparts.
