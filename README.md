# Layoffs Data Cleaning Project

##  Overview
This project focuses on cleaning a real-world dataset of company layoffs.  
The original dataset contained around 2400 records, and after cleaning it contains approximately 1000 records.

The cleaning process was done entirely using **SQL** on MySQL, covering tasks like removing duplicates, cleaning text fields, converting dates, and handling missing values.

---

## Cleaning Process
- Created a staging table to copy the original data.  
- Removed duplicate rows using `ROW_NUMBER()` with `PARTITION BY`.  
- Cleaned text fields using `TRIM()`, `LIKE`, and `UPDATE`.  
- Standardized industry and country names (e.g., "Crypto%" and "United States").  
- Converted date strings to DATE type using `STR_TO_DATE()`.  
- Converted empty values to NULL.  
- Filled missing industry values using self-joins within the same table.  
- Dropped the temporary column `row_num` after cleaning.

---

##  Tools Used
- **MySQL Workbench**  


---

## ⚖️ License
This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.
