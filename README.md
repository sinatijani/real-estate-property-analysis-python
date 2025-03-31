# US Real Estate Data: Comprehensive Data Cleansing and Preparation

## Project Overview

This project focused on the comprehensive cleaning and preparation of a US real estate dataset to ensure its suitability for analytical purposes, particularly within a real estate agency context. The primary objective was to transform a raw, inconsistent dataset into a clean, reliable resource for subsequent analysis.

## Data Cleansing and Preparation Methodology

* **Initial Data Assessment:**
    * Loaded the dataset into a Pandas DataFrame for initial inspection.
    * Identified significant data quality issues, including a high volume of duplicate records (approximately 86% of the dataset) and redundant address information.
    * Extracted essential location data (city and state) from the "full address" column.
* **Duplicate Record Removal:**
    * Eliminated duplicate records based on address, price, size, and sold date criteria.
    * Resulted in a cleaned DataFrame ("df4") free of address duplicates and null values in key columns.
* **Outlier Management:**
    * Identified and addressed price outliers using statistical methods and visualizations (charts).
    * Applied the Interquartile Range (IQR) method to determine appropriate outlier thresholds.
    * Generated a refined dataset ("df5") with mitigated price outliers.
* **Missing Value Imputation:**
    * Imputed missing values in numerical columns (beds, baths, size) using median values.
    * Retained missing "sold date" values to indicate unsold properties, recognizing their analytical value.
* **Final Data Validation:**
    * Conducted a final statistical review of the cleaned dataset.
    * Performed correlation analysis and generated a heatmap to understand feature relationships.
    * Saved the cleaned dataset as an Excel file for future use.

## Key Outcomes and Learnings

* **Data Integrity:**
    * Demonstrated the critical importance of data cleaning in ensuring the reliability of subsequent analyses.
    * Showcased the ability to effectively handle and rectify significant data quality issues.
* **Real Estate Data Insights:**
    * Conducted preliminary statistical analyses (e.g., average price calculations) to illustrate the dataset's potential for real estate-related insights.
    * Highlighted the dataset's utility in understanding market trends and property valuations.
* **Technical Proficiency:**
    * Utilized Python libraries, including Pandas, NumPy, Seaborn, SciPy, and Matplotlib, for data manipulation and visualization.
    * Demonstrated proficiency in data cleaning, outlier detection, and missing value imputation techniques.

## Project Results

* The final cleaned dataset ("df5") represents approximately 12.5% of the original data, reflecting the extent of data redundancy and inconsistencies.
* Preliminary analyses, such as property values by state and sales trend assessments, were conducted, with a primary emphasis on data cleansing.
* For a comprehensive analysis and detailed findings, please refer to the project report.