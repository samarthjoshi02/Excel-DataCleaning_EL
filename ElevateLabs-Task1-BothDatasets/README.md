# Elevate Labs Internship — Task 1 (Excel Basics: Data Cleaning & Formatting)

This repository contains **Task 1 deliverables** for the Elevate Labs internship, completed using **two datasets**:
1. Netflix Movies & TV Shows dataset
2. Global Superstore Orders dataset

---

## Objective
Perform data cleaning and formatting in Excel/Google Sheets including:
- Handling missing values
- Removing duplicates
- Standardizing text fields
- Validating data types (date/numeric/categorical)
- Exporting cleaned datasets in **Excel + CSV**
- Adding documentation (`Data_Quality_Notes`)

---

## Datasets Used

### 1) Netflix Movies & TV Shows
- File: `dataset/NetFlix.csv`
- Rows: ~7.7k (meets required 5k–10k range)
- Issues observed: missing values in multiple text fields (director/cast/country/rating/date_added)

### 2) Global Superstore Orders
- File: `dataset/SuperStoreOrders.csv`
- Rows: 51k+
- Issues observed: text consistency + duplicate line-items

---

## Deliverables

### Netflix Deliverables
Located in: `deliverables/netflix/`
- `Raw_Data.xlsx`
- `Cleaned_dataset.xlsx`
- `cleaned_dataset.csv`

### Superstore Deliverables
Located in: `deliverables/superstore/`
- `SuperStore_Raw_Data.xlsx`
- `SuperStore_Cleaned_dataset.xlsx`
- `SuperStore_cleaned_dataset.csv`

---

## Cleaning Steps Performed (Summary)

### Common cleaning operations
1. Imported CSV correctly with headers and delimiter
2. Freeze top row + filters applied
3. Identified missing values (filter + blank checks)
4. Created backup / preserved raw dataset before cleaning
5. Checked duplicates and removed where applicable
6. Trimmed/standardized text fields
7. Validated:
   - Date columns → standardized to `YYYY-MM-DD`
   - Numeric columns → cleaned and converted to numeric data types
8. Added `Data_Quality_Notes` column in cleaned outputs

**Note: Full SuperStoreOrders.csv file not uploaded due to GitHub file size limit; cleaned outputs are provided.**
---

## Interview Questions (Short Answers)

### 1) Deleting missing data vs imputing missing data?
- **Deleting** removes rows/columns and may reduce dataset size and cause bias.
- **Imputing** fills missing values (mean/median/mode/constant) preserving dataset size but introducing assumptions.

### 2) Risks of removing duplicates incorrectly?
- Removing real valid records
- Incorrect totals/insights
- Data integrity issues  
Always keep a raw backup.

### 3) How TRIM and CLEAN help?
- `TRIM()` removes unwanted spaces
- `CLEAN()` removes hidden/non-printable characters  
Improves consistency for analysis, lookup, grouping, and filtering.

### 4) How to validate correct data types?
- Verify format (Date/Number/Text)
- Convert with Excel formatting / Text-to-Columns
- Ensure numeric columns don’t contain symbols or text

### 5) Why keep raw and cleaned data separately?
- Enables auditing/rollback
- Prevents accidental loss
- Industry best practice

---

## Tools Used
- Microsoft Excel / Google Sheets
- CSV Export (UTF-8)
