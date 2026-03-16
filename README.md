# Coffee Operations Analysis Report (Maven Coffee Challenge)

### **Project Description**
This project is an in-depth operational analysis of a coffee shop chain, designed to bridge the gap between raw transactional data and strategic business decisions. In a competitive retail environment, understanding the "rhythm" of sales is crucial. 

I transformed a complex dataset of coffee transactions into a high-performance **Executive Dashboard** that tracks not just revenue, but the pulse of daily operations. By leveraging advanced Data Modeling and DAX, this report provides a granular view of customer behavior, product lifecycle, and store-level efficiency—empowering stakeholders to optimize staffing, inventory, and marketing efforts based on real-time trends.

**Data Source Information**
* **Dataset:** Maven Coffee Challenge (Transactional Records).
* **Volume:** Comprehensive records of daily coffee shop transactions.
* **Scope:** Includes Transaction Date/Time, Store Location, Product Category, Quantity, and Unit Price.

**Project Overview & Key Business Insights**
* **Peak Periods:** Identified specific hours with the highest transaction volume using a **Time-Series Heatmap**, allowing for optimized staff scheduling.
* **Revenue Drivers:** Determined which product categories (e.g., Coffee vs. Bakery) contribute most to the bottom line versus those that drive volume.
* **Operational Efficiency:** Tracked the **Average Order Value (AOV)** and **Average Coffee per Day** to benchmark store performance across different locations.

**Recommended Analysis (Answering Key Business Questions):**

1. **How have Maven Roasters sales trended over time?** Analyzed monthly and daily revenue streams to identify growth patterns. Used **Time Intelligence DAX** to compare performance across different months and identify seasonal surges.

2. **Which days of the week tend to be busiest, and why?** Identified peak transaction days using `DayName` distributions. Observations suggest specific weekdays/weekends show higher footfall, likely due to morning commute patterns or local store vicinity activities.

3. **What times of day tend to be most popular? Does the trend hold across all locations?** Pinpointed the most popular hours via **Hourly Transaction Trends**. Comparison across locations shows whether the "Morning Rush" is universal or if some branches thrive as "Afternoon Chill" spots.

4. **Which products are sold most and least often? Which drive the most revenue?** **Volume vs. Value Analysis:** Visualized products that have high transaction frequency (sold most often) versus "Premium" items that drive the highest total revenue for the business.

**Technical Process (The Workflow)**

**Data Preparation & ETL:**
* **Power Query Transformation:** Performed heavy data cleaning, including changing column names to proper names for a professional look.
* **Data Integrity:** Handled messy `Time Stamp` formats and standardized product categories.
* **Custom Date Table:** Built a robust **Calendar Table** with `MonthSort`, `DayNo`, `Quarter`, and `DayName` to ensure chronological sorting (Jan-Dec) instead of alphabetical.

**Data Analysis Expressions (DAX):**
* **Time Intelligence:** Developed measures for **MoM Revenue Growth** using `CALCULATE` and `DATEADD`.
  * Formula: $$MoM \% = \frac{\text{Total Revenue} - \text{Last Month Revenue}}{\text{Last Month Revenue}}$$
* **Complex Aggregations:** Created the **Average Coffee per Day** measure using `DISTINCTCOUNT` of `TransactionDate`.
* **Measures Management:** Organized all formulas into a dedicated **"Key Measures"** table for better model scalability.

**Effective Visualization & UI/UX:**
* **Dynamic Formatting:** Implemented a **SWITCH** statement for conditional color coding (Red/Green) to provide instant performance cues.
* **Data Modeling:** Established a **Star Schema** with **One-to-Many (1:*)** relationships between the Date Table and Transactions to ensure filter accuracy.

---

### **🌱 Personal Growth & Milestone**
**This project marks a significant milestone in my data journey. Beyond the technicalities of Power BI, **this is where I mastered the end-to-end process of publishing a project.** I learned how to structure a professional repository, document technical workflows, and present data insights in a way that is accessible to both technical and non-technical stakeholders. It represents my commitment to continuous learning and professional transparency.
**
---


<img width="960" height="424" alt="Coffee_Operations_Analysis_Report" src="https://github.com/user-attachments/assets/41355cae-6257-40a1-ab05-9ffc7a4a6643" />



---

### 📬 Contact Me
* **Email:** jemico.dalangin@gmail.com
* **GitHub Portfolio:** [JCoquillaD](https://github.com/JCoquillaD)
