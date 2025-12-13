# Retail Sales Dataset – Data Cleaning & Analysis

This project focuses on transforming a raw retail sales dataset into a structured and analysable format using Microsoft Excel. The final workbook includes cleaned data, applied formulas, filtered insights, and lookup functions to produce meaningful business information.

---

## Project Files

**Raw Dataset**

This file contains the unprocessed data.

[Download Raw Dataset](./retail_sales_dataset.xlsx)


**Final Project Workbook**

This version includes all cleaning steps, calculations, and analysis.

[Download Final Project Workbook](./retail_sales_dataset_Project.xlsx)

---

##       ────  retail_sales_dataset_sheet  ────


## 1. Data Preparation

### Converted Raw Data into an Excel Table

The first step was converting the raw columns (A–H) into an Excel Table, which provides automatic formatting, dynamic formula ranges, easier filtering and sorting, and a consistent overall structure.

**Screenshot:**
![Excel Table Screenshot](./screenshots/T1.1.jpg)

---

## 2. Data Sorting & Filtering

### Customer Age Sorted (Largest → Smallest)

Sorting age data helps highlight the demographic distribution and identify older or higher-value customer segments.

**Screenshot:**
![Excel Table Screenshot](./screenshots/T1.2.jpg)

---

## 3. Analytical Calculations

### Total Commission

Calculated using Excel’s SUM function in cell P10.

` =SUM(<commission_range>)`
```excel
=SUM(I.:.I)
```

**Screenshots:**
![Excel Table Screenshot](./screenshots/T1.3.jpg)
![Excel Table Screenshot](./screenshots/T1.3_1.jpg)
---

### Average Commission

Calculated using AVERAGE function to determine the typical commission value across all entries in cell P11.

` =AVERAGE(<commission_range>)`
```excel
=AVERAGE(I.:.I)
```

**Screenshot:**
![Excel Table Screenshot](./screenshots/T1.4.jpg)

---

## 4. Additional Analysis

### Total Sales (Filtered by Product Category)
*Result:* £156,905.00

To calculate the total sales for a specific product category, the following SUMIFS formula was used:

```excel
=SUMIFS(I.:.I, F.:.F, "Electronics")
```

***Screenshot:**

![Excel Table Screenshot](./screenshots/T1.SUMIFS.jpg)

### Average Commission (Customers Aged > 30)
Result: £444.37

To find the average commission for customers over 30 years old, the following AVERAGEIFS formula was used:

```excel
=AVERAGEIFS(I.:.I, E.:.E, ">30")
```

**Screenshot:**
![Excel Table Screenshot](./screenshots/T1.AVERAGEIFS.jpg)

### Number of Customers Under Age 25
*Result:* 149

To count all customers younger than 25, the COUNTIF function was used:

```excel
=COUNTIF(E.:.E, "<25")
```

**Screenshot:**
![Excel Table Screenshot](./screenshots/T1.COUNTIF.jpg)

---

## 5. Lookup Functions used (VLOOKUP & XLOOKUP)

### XLOOKUP
Used when flexibility was required:

- Can search both directions
- Can return multiple columns
- Easier to maintain
- No column index issues

### VLOOKUP
Used for straightforward vertical lookups when:

- Data flowed left → right
- Only one value needed
- Simplicity was preferred

*XLOOKUP* is suited for flexible lookups, while *VLOOKUP* is ideal for quick one-direction lookups.

**Screenshots:**

*XLOOKUP:*
![Excel Table Screenshot](./screenshots/XLOOKUP.jpg)

*VLOOKUP:*
![Excel Table Screenshot](./screenshots/VLOOKUP.jpg)

---

## Conclusion

This retail sales project demonstrates how raw data can be transformed into clean, structured, and insightful information using Excel. Through a combination of tables, filters, formulas, and lookup functions, the dataset now provides clear answers to sales performance, customer demographics, and commission trends.

---

**Future improvements may include adding:**
- PivotTables
- Interactive dashboards
- Automated charts
- Advanced category segmentation

This completes the full version of the Retail Sales Dataset Project.

---

##     ────  Student_scores_sheet  ────


# Student Score Dataset

This task analyses student performance using filtering, formulas, and conditional formatting.

### **1) Filter & Sort to Show Best Students in Each Subject**
Applied filtering and descending sorting on each subject column to identify the top performers.


**Screenshots:**
*Best student in **English***
![Excel Table Screenshot](./screenshots/T2.1.English.jpg)

*Best student in **Math***
![Excel Table Screenshot](./screenshots/T2.1.Math.jpg)

*Best student in **Science***
![Excel Table Screenshot](./screenshots/T2.1.Science.jpg)

---

### **2) Calculate Average for All Students (Column E)**
Formula used:

```excel
=AVERAGE(B2:D2)
```

**Screenshot:**
![Excel Table Screenshot](./screenshots/T2.2.jpg)

---

### **3) Highest Score Using MAX Function (Column F)**

Formula used:
```excel
=MAX(B2:D2)
```

**Screenshot:**
![Excel Table Screenshot](./screenshots/T2.3.jpg)

### **4) Filter & Sort to Show Best Student by Average**
Sorted Column E (Average) from largest to smallest to identify the highest-performing student.


**Screenshot:**
![Excel Table Screenshot](./screenshots/T2.4.jpg)

### **5) Filter & Sort to Show Best Student by Highest Score**
Sorted Column F (Highest Score) from largest to smallest.

**Screenshot:**
![Excel Table Screenshot](./screenshots/T2.5.jpg)

### **6) Conditional Formatting – Highlight Highest & Lowest Averages**

Applied conditional formatting rules to Column E:
- Green for the highest average
- Red for the lowest average

**Screenshot:**
![Excel Table Screenshot](./screenshots/T2.6.jpg)

---
