# Quality-Control-Testing-and-Analytics
This project demonstrates an end-to-end data analytics workflow using Excel for data preparation and Power BI for visualization and storytelling.


## 📑 Table of Contents

- [Project Overview](#project-overview)
- [Tools and Methodology](#tools-and-methodology)
  - [Excel (Data Preparation & Cleaning)](#excel-data-preparation--cleaning)
  - [Power BI (Visualization & Insights)](#power-bi-visualization--insights)
  - [Dashboard](#dashboard)
- [Key Insights](#key-insights)
  - [Pass vs. Fail Distribution](#pass-vs-fail-distribution)
  - [Regional Performance Variations](#regional-performance-variations)
  - [Analyst-Linked Variability](#analyst-linked-variability)
  - [Impact of Production Targets](#impact-of-production-targets)
  - [Equipment Reliability](#equipment-reliability)
  - [Raw Materials from Unauthorized Vendors](#raw-materials-from-unauthorized-vendors)
- [Recommendations](#recommendations)
  - [Strengthening Staff Management & Training](#strengthening-staff-management--training)
  - [Review Production Targets](#review-production-targets)
  - [Enhance Equipment Maintenance](#enhance-equipment-maintenance)
  - [Vendor Validation & Procurement Control](#vendor-validation--procurement-control)
  - [Implement Regional Quality Harmonization](#implement-regional-quality-harmonization)
  - [Promote a Culture of Quality First](#promote-a-culture-of-quality-first)
  - [Process Improvement](#process-improvement)
- [Conclusion](#conclusion)
- [Contact](#contact)


## Project Overview

This project was developed to analyze Quality Control (QC) test results across multiple products, regions, and analysts. The primary objective was to identify patterns in pass/fail outcomes, uncover potential risks, and provide actionable recommendations for management.

Disclaimer: The data used in this project is entirely fictitious and has no connection to any real company.


## Tools and Methodology

Excel (Data Preparation & Cleaning)

•	Dataset stored as QC_Testing_Data.xlsx


•	Cleaned columns: Batch ID, Product Name, Region, Analyst, Test Name, Result (Pass/Fail), Date

Performed initial checks:
   - Ensured dates were real date formats
   - Confirmed no duplicate batch IDs and null values
   - Standardized Pass/Fail labels

Ensured the dataset was structured for analysis in Power BI.

### Power BI (Visualization & Insights)

•	Connected cleaned Excel dataset to Power BI.

•	Created calculated DAX measures:

•	Total Batches = COUNTROWS(QC_Data)

•	Pass Count = CALCULATE(COUNTROWS(QC_Data), QC_Data[Result] = "Pass")

•	Fail Count = CALCULATE(COUNTROWS(QC_Data), QC_Data[Result] = "Fail")

•	Pass % = DIVIDE([Pass Count], [Total Batches], 0)

•	Fail % = DIVIDE([Fail Count], [Total Batches], 0)

•	Distinct Products = DISTINCTCOUNT(QC_Data[Product_Name])

### Designed an interactive dashboard:

•	KPI Cards: Total Batches, Pass %, Fail %, Distinct Products

•	Pass vs Fail Overall (Donut Chart)

•	Pass count vs Fail count by Region (Clustered Column Chart)

•	Trend Over Time (Line Chart)

•	Management Note: Key risks (staff gaps, targets, poor maintenance, unauthorized vendors)

•	Failure Rate by Test (Clustered Column Chart)

•	Pass Count vs Fail Count by Analyst (Stacked Bar Chart)

•	Pass % by Product (Matrix)

•	Pass vs Fail by Batch (Stacked Column Chart)

•	Added slicer for Region, Production Name, and Month to make it interactive.

### Dashboard

<img width="624" height="351" alt="QC Analysis Dashboard" src="https://github.com/user-attachments/assets/7f928b8c-31c9-45fb-be75-8b9d881bde32" />


## Key Insights


### Pass vs. Fail Distribution


    •	High Failure Rate: 55.33% of batches failed QC tests, signaling potential risks in compliance and product reliability.

    •	A significant number of batches failed critical QC tests, especially in Weight, Purity, Viscosity, and pH, which are essential for product safety and consistency.

### Regional Performance Variations


    •	Certain regions (e.g., Port Harcourt) reported higher failure rates, suggesting inconsistent practices in staff supervision, adherence to SOPs, or equipment reliability.

### Analyst-Linked Variability

   
    •	Analysts handling higher workloads showed higher failure rates, likely due to fatigue, rushed testing, and training gaps.

### Impact of Production Targets


    •	Failure spikes coincide with periods of high production pressure, indicating that outrageous targets are pushing staff to compromise quality checks.

### Equipment Reliability


    •	Failures in Viscosity and Strength tests suggest inadequate calibration and poor maintenance of QC instruments, increasing inconsistent results and rejections.

### Raw Materials from Unauthorized Vendors


    •	Batches with low Purity and out-of-specification results point toward possible procurement of raw materials from unvalidated suppliers.

    •	Using unauthorized vendors introduces variability, contamination risks, and non-compliance with GMP (Good Manufacturing Practices), undermining overall product quality.


## Recommendations

### Strengthening Staff Management & Training


    •	Standardize QC processes across all regions through refresher training and SOP alignment.

    •	Rotate analysts to prevent fatigue and improve skills distribution.

    •	Monitor staff performance with supportive, rather than punitive, approaches.

### Review Production Targets


    •	Set realistic batch production targets that prioritize quality over speed.

    •	Incorporate quality KPIs (e.g., pass rate, avoid repeat test) into staff evaluations.

### Enhance Equipment Maintenance


    •	Establish a strict preventive maintenance and calibration program.

    •	Ensure downtime for equipment servicing is respected.

    •	Create rapid reporting systems for faulty equipment.

### Vendor Validation & Procurement Control


    •	Procure raw materials only from authorized, validated, and audited vendors.

    •	Maintain a Vendor Qualification Program to regularly assessing suppliers.

    •	Link material traceability to test results to quickly identify supplier-related failures.

### Implement Regional Quality Harmonization


    •	Share best practices from high-performing sites with weaker ones.

    •	Create a central Quality Review Committee to track, investigate, and address recurring failures.

### Promote a Culture of Quality First


    •	Reaffirm that compliance and patient safety outweigh production targets.

    •	Recognize and reward teams consistently meeting quality standards.


### Process Improvement

    •	Focus on tests with the highest failure rates (e.g., viscosity, weight, purity) for root cause investigation.

## Conclusion

The QC Testing results confirm that failures stem not only come from testing errors but also from organizational weaknesses across staff management, production pressure, equipment reliability, and raw material sourcing. If left unchecked, these issues may expose the company to regulatory risks, increased costs, loss of market credibility, and potential patient safety concerns.

By addressing these areas holistically, especially enforcing vendor validation, reviewing production targets, and investing in staff training and equipment upkeep, the company can significantly reduce failures, Improve and strengthen compliance with regulatory standards, reduce waste, enhance customer trust and protect its long-term reputation.








##   Contact
👤 **Samuel Adeyemi Oyemomi**  
Quality Control & Data Analytics Professional || Skilled in Lab Testing, SQL, Excel, Power BI

📞 Phone: **+2348066370376**  
📧 samueloyemomi@gmail.com; successintelligencehub@outlook.com  
🌐 [LinkedIn](https://www.linkedin.com/in/samuel-oyemomi) | [GitHub](https://github.com/oyemomisamuel)

