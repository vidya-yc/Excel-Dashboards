🏥 Hospital Emergency Room Dashboard (Excel + Power BI)

This is an end-to-end dashboard project designed to analyze emergency room performance metrics using Power BI, with data preprocessing done in Excel.

📌 Project Objective

To create a dynamic and interactive Hospital Emergency Room Analysis Dashboard that provides actionable insights to improve operational efficiency and decision-making in patient care.

🎯 Key KPIs & Visualizations

Patient Admission Status: Number of admitted vs. not admitted patients

Patient Age Distribution: Age groups segmented for better demographic insights

Timeliness: Percentage of patients attended within 30 minutes

Gender Analysis: Distribution of patients by gender

Department Referrals: Most referred departments

⚙️ Technical Stack

Excel: Data cleaning and preprocessing

Power BI: Data modeling, DAX calculations, and dashboard development

🧬 DAX Highlights

Age Group Calculation:

=IF([Patient Age]>=70,"70-79",
  IF([Patient Age]>=60,"60-69",
  IF([Patient Age]>=45,"45-59",
  IF([Patient Age]>=30,"30-44",
  IF([Patient Age]>=15,"15-29",
  IF([Patient Age]>=5,"05-14","0-4"))))))

Patient Wait Time Category:

=IF([Patient Waittime]<30, "Within Time", "Delay")

🗕️ Calendar Table Formula (Power Query)

= List.Dates(#date(2023,01,01),731,#duration(1,0,0,0))

📊 Final Output

An insightful Power BI dashboard that enables hospital administrators and stakeholders to:

Monitor patient inflow and service timeliness

Identify critical age demographics

Improve resource allocation based on referral trends

