# ETL-Data Pipeline-Project
## An automated data pipeline for Covid19 Prediction and Reporting

### Goal of the Project
Building a reliable data pipeline to compile COVID-19 data from several sources, including government health departments, hospitals, and research institutes, would be the project's primary goal. These pipelines can clean, process, and integrate data into a centralized data lake or data warehouse, allowing it to be accessible for additional analysis, using the connections and transformations offered by Azure Data Factory.

### The Datasets' source
In this project, The dataset is ingested to Azure Data Factory from two sources: first dataset is ingested from Azure Blob storage and other dataset is ingested from http i.e website of European Centre for Disease Prevention and Control (ECDC)

### Use Cases
Below are some of the use cases of the data collected:
- The data can be used to identify the impact that affected people by covid-19 virus have on city population, going even further to categorize the impact by gender.
- Medical researchers can use the data to identify what some of the most common reason that the people are getting affected by the virus.
- Doctors can create a good vacccine for the people.

### Database Model
- This project contains various datasets from the ecdc website like cases_deaths, hospital_admissions, testing and country_response and all the datasets are in csv formats.
- The brief description of the datasets are given below.
- 
### Cases Deaths Table

- Columns: country, country_code, continent, population, indicator, daily_count, date, rate_14_day, source.

### Hospital Admissions Table

- Columns: country, indicator, date, year_week, value, source, url.

### Testing Table

- Columns: country, country_code, year_week, new_cases, tests_done, popu
3- For the data storage we use Azure Data Lake Gen 2
