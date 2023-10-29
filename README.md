# ETL-Data Pipeline-Project
## An automated data pipeline for Covid19 Prediction and Reporting

### Goal of the Project
Building a reliable data pipeline to compile COVID-19 data from several sources, including government health departments, hospitals, and research institutes, would be the project's primary goal. These pipelines can clean, process, and integrate data into a centralized data lake or data warehouse, allowing it to be accessible for additional analysis, using the connections and transformations offered by Azure Data Factory. The overall task which needs to performed are as shown:
![Image_1](https://github.com/rahulingle92/COVID-19-ETL_data_pipeline/assets/44425377/df821e06-7b7b-4f3f-a195-bd597c7ed8e2)


![Goal of the project](https://github.com/rahulingle92/COVID-19-ETL_data_pipeline/assets/44425377/1a66c120-7146-4a87-8f30-3a2aa551dc27)


### The Datasets' source
In this project, The dataset is ingested to Azure Data Factory from two sources: first dataset is ingested from Azure Blob storage and other dataset is ingested from http i.e website of European Centre for Disease Prevention and Control (ECDC). We received following details  from the ECDC  website:
 * Confirmed Cases on daily basis
 * Mortality due to COVID 19 on daily basis
 * Hospitalization / ICU cases
 * Testing Numbers
#### We received  following details from Eurostat website :
 * Country's Population by Age Group

### The Datalake that we built with following data to help the data Scientist to predict the spread of the virus/ Mortality:
 * Confirmed Cases on daily basis
 * Mortality due to COVID 19 on daily basis
 * Hospitalization / ICU cases
 * Testing Numbers
 * Country's Population by Age Group
The Data Warehouse that we built with the following data to aid reporting on Trends
 * Confirmed Cases on daily basis
 * Mortality due to COVID 19 on daily basis
 * Hospitalization / ICU cases
 * Testing Numbers
 * Country's Population by Age Group

![Tools Used](https://github.com/rahulingle92/COVID-19-ETL_data_pipeline/assets/44425377/eb9c40aa-5617-41c9-987e-b3ff71d239ed)

![Solution Architecture](https://github.com/rahulingle92/COVID-19-ETL_data_pipeline/assets/44425377/088e9576-68a7-49a3-9972-09332e99ce76)

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
