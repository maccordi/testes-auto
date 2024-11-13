# MES Automation

This project began as a simple site-scraping tool for the MES system—an extension of the industry ERP that captures machine and production data. It has since evolved into a fully automated data collection system, designed to compare various data frames and update them for better data utility and decision-making.

# Development:


Previously, data from the MES system was manually retrieved and downloaded as an unstructured spreadsheet. This task was both time-consuming and redundant, adding strain to the already fast-paced environment typical of the metallurgical industry.

The key metric analyzed is a KPI called Active Pending Items (**API**). Monitoring these APIs is critical, as they represent bottlenecks for materials awaiting release to the customer. Any pending item over two days would be flagged in board meetings, often leading to delays in warehouse operations.

One significant limitation of the MES system is its lack of historical data storage for APIs. Completed items were deleted, making it difficult to analyze past performance for continuous improvement. The main goal of this project was to establish a historical record of APIs to study the root causes of recurring issues.

# Having data history

This project aimed to create a data history for one of the most significant bottlenecks in this industry. API causes and impacts on the warehouse vary widely, necessitating a standardized approach to analyzing and addressing each type of issue. The data collected is visualized in a Power BI dashboard, serving as a reference for senior management on the primary drivers of API impacts and streamlining the previously tedious daily process of filtering data from the MES system.

# Lessons Learned:

This was my first solo data science project and a challenging learning experience. I gained insights into the _data scientist’s mindset_—learning how to frame meaningful questions and identify the most relevant answers. Starting this project was a personal initiative, motivated by my desire to apply newly acquired programming skills, and it ultimately evolved into a comprehensive data science project.

# MES is a Mess!

One of the biggest challenges was automating the MES system. It’s a slow, outdated system that only operates on Internet Explorer! Performance varied greatly during testing, and the system frequently went offline due to the heavy flow of data input. This project’s success was especially rewarding because it removed one of the biggest inconveniences from my daily routine.

