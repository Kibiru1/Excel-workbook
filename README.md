# Excel-workbook
An interactive Excel dashboard analyzing Jumia e-commerce product performance, pricing strategies, and customer engagement metrics.

# Jumia Product Performance Dashboard

**Author:** Simon Kibiru

## 📌 Project Overview
This project involves the data cleaning, analysis, and visualization of a Jumia e-commerce product dataset. The primary objective is to transform raw, unstructured product data into an interactive Excel dashboard that provides stakeholders with actionable business insights regarding pricing strategies, customer engagement, and product quality.

## 🛠️ Tools & Techniques Used
* **Microsoft Excel:** Advanced Data Analytics & Visualization
* **Data Cleaning:** Imputation, string extraction (`LEFT`, `FIND`), absolute value conversions, and standardized logical fallback values.
* **Backend Logic:** Pivot Tables, `INDEX`/`MATCH` arrays, and nested `IF` statements.
* **Frontend UI:** Interactive Dashboard, Dynamic PivotCharts, and connected Slicers.

## 🧹 Data Cleaning Methodology
To ensure mathematical accuracy for downstream Pivot Tables, several data standardization steps were executed:
* **Missing Value Imputation:** Blank entries in the "Old Price" column were dynamically replaced with the "Current Price" to accurately reflect a $0 discount rather than a negative mathematical error.
* **String Dissection:** Text-based ratings (e.g., "4.3 out of 5") were stripped using search functions to extract pure decimal values.
* **Variable Price Standardization:** Products displaying a variable price range (e.g., KSh 1,620 - KSh 1,980) were manually standardized to their base (minimum) price to allow for accurate macro-level average calculations.
* **Absolute Values:** Negative review counts were converted to standard positive integers to correct sorting behaviors.

## 📊 Key Business Insights

**1. The Impact of Discounts on Customer Engagement** There is a clear positive correlation between the discount percentage and customer interaction. Products categorized under "High Discount" (above 40%) consistently generate a higher volume of user reviews compared to "Low Discount" items, indicating that aggressive pricing strategies effectively drive product visibility and customer engagement on the platform.

**2. The "Perfect Score" Illusion** A perfect 5.0 rating is often an artifact of exceptionally low sample sizes rather than universally superior product quality. The analysis reveals that items with the absolute highest ratings typically possess fewer than 5 reviews. Conversely, the most frequently purchased and heavily reviewed products stabilize at a more realistic "Average" to "Excellent" threshold (e.g., 4.1 to 4.6), providing a more reliable indicator of consistent market performance.

**3. Price Reductions vs. Perceived Quality** Heavy discounting does not inherently damage the perceived quality of a product. The data indicates that products in the "High Discount" category maintain average ratings that are competitive with items rarely on sale. This suggests that while sales drive transaction volume, Jumia customers still rate items strictly based on the intrinsic utility and functionality of the product rather than its discounted status.

## 📂 Repository Contents:

* 📂 assets/: `Dashboard_Preview.png`: A high-resolution screenshot of the final dashboard UI.
* 📂 data/: `Raw_Data.csv`: The original, unmodified dataset provided for the assessment.
* `Excel_jumia_data set assessment.xlsx`: The final workbook; containing the cleaned database, backend Pivot Tables, and the interactive frontend dashboard.
* 📄 README.md
