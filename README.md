# SQL Recipes for Web Analytics
This repository contains SQL code used in web analytics.

# Data Extract
### Google Analytics Clickstream Data BigQuery Export
This SQL query transforms Google Analytics BigQuery nested data into flat hit level data with a timestamp making data easy to analyze using  tools like Tableau, SAS, R, etc.
#####Instructions:
1. Select either timestamp or UNIX time as you prefer by commenting either line #2 or line #3
2. Select only the appropriate fields. The table may contain more than 200 columns, select only the variables you are capturing/using, namely custom variables, custom dimensions, enhanced ecommerce, etc. Please note this query contains fields that don't exist in older datasets, you will have to adapt accordingly.
3. Output the results to another table and export to Google Storage
4. Download the CSV, done!