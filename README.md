# Sales-Credits-and-Debits-Monitoring-System
I participated in a BI training program. During a group project, I had the opportunity to collaborate with a team member who works in a manufacturing organization. He was particularly impressed with my skills in SQL and Power BI. Recognizing the potential benefits for his company, he approached me after the training to see if I'd be interested in helping him to build a POC for a financial reporting system.Using real company data might not be feasible at this stage due to privacy concerns or the need to simplify the process. Since the project is a POC aiming to showcase the system's functionality, I planned to use fake data in order to show how the system can examine sales, credits, and debits for their company.
This project focuses on building a data pipeline to ingest and analyze sales data from distributors and wholesalers. Here's a breakdown of the key points:

Data Sources:
Multiple daily files are received from distributors and wholesalers. These files likely contain information related to:
Sales data (products sold, quantities, prices)
Credit and debit information (transactions involving customer payments)
Inventory data (stock levels, product availability)
Data Ingestion:
A Lambda function is used to process these daily data files.
Lambda functions are serverless compute services that run code in response to events (in this case, new data files arriving).
Data Transformation:
The Lambda function likely performs some business logic to transform the raw data before storing it. This might involve:
Data cleaning (handling missing values, formatting inconsistencies)
Data mapping (matching fields across different files)
Data aggregation (summarizing sales by product, customer, etc.)
Data Storage:
The transformed data is stored in a Redshift database.
Redshift is a cloud-based data warehouse solution optimized for large datasets and complex analytics.

Benefits of this Project:
Centralized Data: This system creates a central repository for sales, credit/debit, and inventory data.
Improved Data Quality: The business logic in the Lambda function ensures consistent and reliable data for analysis.
Efficient Analysis: Storing data in a data warehouse like Redshift enables efficient querying and analysis of sales trends, customer behavior, and inventory management.
Scalability: Redshift and Lambda functions can handle large data volumes and adapt to increasing data needs.
Possible Future Enhancements:
Automation: Schedule the Lambda function to automatically process data files upon arrival.
Data Visualization: Integrate this data pipeline with data visualization tools to create insightful sales reports and dashboards.
Machine Learning: Use the sales data for customer segmentation, churn prediction, or other predictive analytics.

Overall, this project establishes a robust data pipeline for analyzing sales data from distributors and wholesalers. This will provide valuable insights to improve sales strategies, optimize inventory management, and gain a deeper understanding of customer behavior.


