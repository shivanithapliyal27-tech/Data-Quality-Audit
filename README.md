# Data Quality Audit Using Python and Pandas

## Project Overview

This project focuses on performing a Data Quality Audit using Python, Pandas, NumPy, and Google Colab. The Sample Superstore dataset is used to identify potential data quality issues, including missing values, duplicate records, and unusual numeric values.

The objective is to improve data reliability and prepare the dataset for further analysis and reporting.

## Objectives

- Inspect dataset structure, columns, and data types.
- Identify and analyze missing values.
- Detect duplicate records.
- Perform data range and consistency checks.
- Create a data quality issue log.
- Generate a repeatable quality checklist.
- Export cleaned data and audit results.

## Tools and Technologies

- Python
- Pandas
- NumPy
- Google Colab
- Microsoft Excel
- GitHub

## Dataset

The project uses the Sample Superstore dataset. The primary analysis is performed on the **Orders** sheet, which contains sales, customer, product, quantity, discount, and profit information.

## Project Methodology

### 1. Data Loading and Inspection
Loaded the Orders sheet into a Pandas DataFrame and inspected its dimensions, columns, data types, and statistical summary.

### 2. Missing Values Analysis
Calculated missing-value counts and percentages for each column to identify incomplete records.

### 3. Duplicate Records Detection
Identified exact duplicate rows and reviewed them before removal.

### 4. Data Range Checks
Checked selected numeric columns, including Sales, Quantity, Discount, and Profit, for values requiring further investigation.

### 5. Issue Log Creation
Created an issue log containing selected issue types, counts, severity labels, and recommended actions.

### 6. Data Cleaning
Created a separate dataset copy with exact duplicate rows removed while preserving the original source data.

### 7. Exporting Results
Exported audit summaries, the cleaned sample, and the quality checklist as CSV files.

## Key Deliverables

- `Data_Quality_Audit.ipynb` — Google Colab notebook containing the Python code.
- `Cleaned_Sample.csv` — dataset copy with exact duplicate rows removed.
- `Data_Quality_Issue_Log.csv` — summary of identified issues and recommended actions.
- `Missing_Values_Audit.csv` — missing-value counts and percentages.
- `Data_Range_Audit.csv` — numeric range summary.
- `Data_Quality_Checklist.csv` — repeatable data quality checks.
- `Data_Quality_Audit_Project_Report_4_Pages.docx` — detailed project report.

## Key Considerations

- Missing values should be handled according to business requirements.
- Duplicate records should be reviewed before removal.
- Negative profit may represent a genuine business loss.
- Negative sales may reflect returns or adjustments.
- A REVIEW status indicates that an issue needs investigation; it does not automatically mean the data is incorrect.

## Conclusion

This project demonstrates how Python and Pandas can be used to perform a structured data quality audit. The workflow identifies potential issues, documents findings, and generates reusable audit outputs. These checks help prepare datasets for more reliable business analysis and reporting.

## Future Improvements

- Add date validation and category consistency checks.
- Validate relationships between workbook sheets.
- Implement additional business-specific validation rules.
- Maintain a detailed correction log.
- Automate the audit process for new datasets.

## Repository Structure

```text
Data-Quality-Audit/
├── README.md
├── Data_Quality_Audit.ipynb
├── Data_Quality_Audit_Project_Report_4_Pages.docx
├── Cleaned_Sample.csv
├── Data_Quality_Issue_Log.csv
├── Missing_Values_Audit.csv
├── Data_Range_Audit.csv
└── Data_Quality_Checklist.csv
