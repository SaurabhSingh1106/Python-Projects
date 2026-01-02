Brevard Claims and AR Analytics (HIPAA Safe)

Domain: US Healthcare Revenue Cycle Management (RCM)
Tools: Python, Pandas, NumPy, Matplotlib
Records Analyzed: 56,900+ claims
Compliance: HIPAA Safe (real patient data not published)


Objective

To analyze claim-level billing, payments, denials and outstanding accounts receivable to identify revenue leakage, payer risk, provider performance and overdue accounts using automated Python analytics pipelines.


Business Questions Answered

1. Which insurance carriers have the highest outstanding accounts receivable
2. How accounts receivable is distributed across aging buckets such as 0 to 30, 31 to 60, 61 to 90, 91 to 120 and 120 plus
3. Which departments generate the highest total charges
4. Which months collected the highest payments
5. Which providers have the highest collection rates
6. Which denial reason codes contribute the most outstanding accounts receivable
7. Which places of service hold the maximum accounts receivable balance
8. Which procedure codes generate the highest insurance payments
9. Which denial reasons have the highest denied voucher counts
10. What is the overall comparison of charges versus payments versus balance



What This Pipeline Does

Cleans and standardizes raw claim Excel files
Handles null values, date formatting and numeric conversions
Creates aging days, aging buckets and collection rate features
Builds payer, provider, department and denial analytics
Generates automated executive dashboards
Saves all charts as PNG for reporting and Power BI usage


Key Insights Sample

Claims Analyzed: 56,900+
Highest Risk Payer: Medicaid Florida
Overdue Bucket: 120 plus days
Top Revenue Department: Brevard Geriatrics
Main Denial Drivers: CO 16, CO 45, CO 256


Data Privacy Notice

Due to HIPAA compliance, original datasets are excluded.
Only anonymized analytics scripts and outputs are published.
