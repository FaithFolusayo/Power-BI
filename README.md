# Project overview 
This project focuses on supplier quality and performance data from Enterprise Manufacturer limited for the years of 2018-2019. The objective is to analyze and visualize the data to address key business questions about vendor performance, identify trends in defects and downtime and their impact on overall operations, helping the company standardize and improve supplier quality.

# Problem statement
The manufacturer has no control system to monitor and regulate the quality of goods supplied by different vendors across multiple plants. As a result, they are unable to identify which suppliers consistently provide quality goods and which do not. This leads to an increase in defects quantity and downtime, causing significant financial losses.

# Dataset Description
Content: The dataset consists of 9 columns and 5,227 rows

# Tool used: 
Power BI

# Data preprocessing:
1. I imported the dataset into power BI and use power query to transform the dataset
2. Separated the datasets into one (1) fact table and six (6) dimension tables and then remove duplicates from the dimension table.
3. Linked the dimension table to the fact table by adding an index column to the dimension table and then merge the dimension table to the fact table using the index column.
4. Created a calendar table to allow for date-based filtering and analysis.
5. Assumed the cost of downtime to be between $0 and $20 per hour and created a downtime cost parameter for dynamic analysis.
6. Created several new measures (using DAX) and parameters for more detailed insights.
7. Created and Added tooltips to the map chart, displaying each plant location
 
# Exploratory Data analysis
This project analysis is divided into five (5) section:
1. Overview: Provides an overview of defects and downtime trends, vendor and category performance across the organization.
2. Vendor performance: Highlights vendors responsible for the highest quantity of defects and downtime, the impact of defects on downtime and the greatest quantity of the defects and downtime on defect type and vendor.
3. Plant Performance: Analyze defect and downtime data by plant location, identifying top and bottom performers and vendors/material type performance at each plant locations.
4. Material Performance: Reviews the performance of different materials, category and defect by defect quantity and downtime hours. Also includes the monthly trend of defect quantity and downtime hours across each category.
5. Downtime Impact: Focuses on the impact of downtime caused by defective materials, providing insights into areas for improvement.

# Insights
The following insights were drawn from the analysis;
1. What is the total defect quantity and the cumulative downtime hours?
The analysis reveals a total of 2.6 billion defect quantity and 216,000 hours of downtime amounting to an estimated cost of $2.16 million (assuming a rate of  $10 per hour). In 2019, the defect quantity increased by 23.32% compared to the previous year with October recording the highest number of defects.

2. which vendors and plants are causing the greatest defect quantity and downtime?
a) Yombu, Avamm, and Meejo are the top 3 vendors causing the greatest defect quantities, contributing 15.1M, 14.7M, and 14.2M defects, respectively. Despite this, these vendors do not necessarily contribute to the most downtime. For instance, Avamm, although ranking second in defects, ranks first in downtime with 1165 hours alongside Izio (1144), and Meetz (1134) indicating that defect severity might vary significantly across vendors. This also reveal that the vendors with the highest defect quantity don't always contribute the most to downtime, signaling potential differences in defect types or process recovery times.

b) Hingman (100M), Charles City (99M), and Twin Rocks (97M) are the top 3 plants location contributors to defect quantities. However, when looking at downtime, Riverside (8.6k hours), Charles City (8.3k hours), and Twin Rocks (8.0k hours) lead the list, showing that some plant locations are both inefficient in terms of defect management.

3. Which combination of vendor and plant performs poorly?
The combination of Yombu and Prescott performed poorly resulting in the highest defect quantity(3.22M) while the combination of Wikido and Middletown experience the highest downtime (2923 hours). This suggests that certain vendor-plant combinations are more prone to operational inefficiencies and quality issues.

4. Is there a particular combination of vendor and material that perform poorly?
The combination of EdgeBlab and Raw Materials performed poorly resulting in the highest defect quantity (app 6.35M) while the combination of Feedfire and Corrugate had the highest downtime (approximately 568 hours). These material-vendor combinations represent significant problem areas. Across the table, Raw materials and Corrugate material type generated more defect quantity and downtime compare to other material types. Therefore, majority of vendors supplying raw materials and corrugate are causing high defect quantity.

5. Performance comparison of vendor-material combinations across plants location.
The analysis of vendor and material performance across different plants location using a Map chart reveal inconsistencies. The analysis reveals that the combination of vendor-material generating the highest defect quantity varies by plants location. For example, in Hingham, where the overall defect quantity is highest, the combination of FeedFish and Raw materials results to the most defects. Conversely, in Charles City, the combination of Linklinks and Corrugate has the highest defect quantity. These variances may suggest possible differences in plant operations, manufacturing processes, or the level of vendor support by region.

# Recommendation
1.Implement process optimization strategies at plants like Riverside, Charles City, and Twin Rocks to minimize downtime and enhance operational efficiency.
2. Introduce stricter quality checks for material types to minimize defects and downtime.
3. Consider sourcing for alternative vendors for material types such as Corrugate and Raw Materials, which significantly contribute to downtime and defects, to improve overall material quality and reduce operational inefficiencies.
4. Conduct regular vendor audits for vendors with high rates of defects and downtime, focusing on enhancing their performance and ensuring compliance with quality standards.
5. Investigate the factors contributing to poor performance for combination of vendor-material/ vendor-plant and address these issues to prevent recurrence.
 
# Conclusion
This analysis provides a comprehensive overview of supplier performance at Enterprise Ltd., highlighting key insights into the vendors, material types, and plants contributing the most to defects and downtime. The insights from this analysis enables us to monitor the quality of goods thereby reducing downtime by helping us identify the suppliers providing bad quality goods. By addressing these areas, the company can reduce defects, minimize downtime, and improve the overall operation.
 


