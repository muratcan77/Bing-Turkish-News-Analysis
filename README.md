![324793617-5ee6d206-1278-42a1-aab8-c291b68e4ef8](https://github.com/user-attachments/assets/4723408c-3195-429f-a64f-d976607a9e48)Bing News Analysis with Microsoft Fabric
This project is a complete end-to-end solution that leverages Microsoft Fabric tools to gather, analyze, and visualize news data from Bing News. The main objectives were to collect the latest news daily, perform sentiment analysis, and display the results using Power BI. Additionally, an alert system was integrated to notify users based on the positivity of the news content.
![324793617-5ee6d206-1278-42a1-aab8-c291b68e4ef8](https://github.com/user-attachments/assets/f6a9643f-f6ea-45a8-a837-f82660387c8e)

Technologies Used
Data Factory: For creating data ingestion and automated data pipelines.
Synapse Data Engineering and Data Science: For transforming data and performing sentiment analysis.
Power BI: To visualize the sentiment analysis results of the news articles.
Data Activator: For setting up notifications based on the analysis results.
Steps in the Project
1. Data Ingestion
Collected news data using Bing News API.
Created a data ingestion pipeline in Azure Data Factory to move data to OneLake in JSON format.
Bing API Documentation
2. Data Transformation
Utilized Synapse Data Engineering to clean and transform JSON data into Delta tables.
Cleaned data by extracting important attributes like headline, category, date, and source.
Transformation Notebook
3. Sentiment Analysis
Used Synapse Data Science for sentiment analysis on news content.
Saved the analyzed data in Delta tables for use in Power BI reports.
Sentiment Analysis Notebook
4. Power BI Reporting
Created reports to visualize news sentiment analysis in Power BI.
Added cards for positive, negative, and neutral sentiment percentages.
![1_ApEie-T2DWiPAJWAUSLfHA](https://github.com/user-attachments/assets/6daafa30-8ada-40d7-b442-f1b6afa01b97)
6. Pipeline Automation
Built a complete Data Factory pipeline to automate data ingestion, transformation, and analysis.
Scheduled the pipeline to run automatically every day at 6:00 AM.
7. Alert System
Set up Data Activator to create alerts in Power BI for specific conditions, such as when the positive sentiment is above a certain threshold.
Configured alerts to be sent mail.
Key Learnings
SCD Type 1 was used to manage data updates effectively without duplication.
Automated pipelines ensure fresh data and insights are available every morning.
Corrected data types for accurate filtering in Power BI.

https://medium.com/p/752be49140d2/edit
