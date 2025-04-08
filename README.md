## Blinkit Sales Performance Analysis - Power BI Dashboard

**Project Objective:**

This project analyzes Blinkit's sales data to gain actionable insights that will optimize performance, inventory distribution, and customer satisfaction.

[Blinkit Sales Dashboard](https://github.com/user-attachments/assets/489e2428-2748-49d5-ad51-cedbde366200)

**Dataset Used:** <a href="https://docs.google.com/spreadsheets/d/1iiqAJSjHRJx5bYcvb3aTjkXzyRxI3r_E/edit?usp=drive_link&ouid=117599201032091952181&rtpof=true&sd=true"> Download Dataset<a/>

The dataset includes information on 8,253 sales transactions, including item details (fat content, type), outlet information (location, size, type), sales figures, and customer ratings.

**Dashboard:** <a href="https://drive.google.com/file/d/1RJYemlbTFwRFvVVwnhXSp7xnLgtpQgE4/view?usp=sharing">View Dashboard<a/>

**Questions (KPIs):**

*   **How do sales vary by item fat content?**
    *   Low Fat items account for $425.36K in sales
    *   Regular items account for $5776.32K in sales

*   **Which outlet types perform best?**
    *   Supermarket Type1 leads with $787.55K in sales
    *   Grocery Stores follow with $151.94K in sales

*   **What is the total sales revenue?**
    *   $1.20M across all outlets

*   **How does outlet size affect sales?**
    *   Tier 3 outlets dominate with $50.17M in sales
    *   Tier 1 outlets show $50.12M in sales

*   **What is the average rating across outlets?**
    *   Consistent 3.9 average rating across outlet types

**KPIs:**

*   **Total Sales:** $1.20M
*   **Number of Items:** 8,523
*   **Average Sales:** $140-$142 (varies by outlet type)
*   **Average Rating:** 3.9

**Process:**

1.  **Data Cleaning:**
    *   Used Power Query to clean and transform data:
        *   Standardized "Item Fat Content" values (LF → Low Fat, Reg → Regular)
        *   Verified 100% data quality after cleaning
    *   Created custom canvas (800 × 1400 px, 40% transparency)

2.  **Data Analysis:**
    *   Created DAX measures:
        ```dax
        Total Sales = SUM(Sales[Amount])
        Average Sales = AVERAGE(Sales[Amount])
        No. of Items = DISTINCTCOUNT(Items[ID])
        Average Rating = AVERAGE(Ratings[Score])
        ```
    *   Developed visualizations:
        *   Donut charts for fat content distribution
        *   Bar charts for item type performance
        *   Stacked columns for outlet comparisons
        *   Line charts for outlet establishment trends

3.  **Dashboard Development:**
    *   Implemented interactive filters (location, size, type)
    *   Added reset button for slicers
    *   Designed intuitive layout with KPI cards

**Insights:**

*   **Top-Selling Items:** Regular fat content items dominate sales
*   **Best-Performing Outlets:** Tier 3 outlets show highest sales
*   **Rating Consistency:** All outlet types maintain 3.9 average rating
*   **Geographic Trends:** Urban locations show stronger performance
*   **Outlet Age Impact:** Newer outlets demonstrate consistent sales

**Recommendations:**

*   **Inventory Optimization:** Increase stock of Regular fat content items
*   **Outlet Expansion:** Focus on Tier 3 outlet models for new locations
*   **Promotional Strategies:** Highlight high-rated items to boost sales
*   **Data Collection:** Enhance customer feedback mechanisms
*   **Regional Focus:** Allocate more resources to high-performing locations

**Dashboard Features:**

*   **Interactive Filters:** Segment by outlet location, size, and type
*   **Dynamic Visuals:** Hover tooltips and drill-down capabilities
*   **Comprehensive View:** All key metrics on single dashboard
*   **Mobile-Responsive:** Adapts to different screen sizes

This analysis provides valuable insights into Blinkit's sales performance and can inform strategic decisions regarding inventory management, outlet expansion, and customer engagement strategies.
