# ETL-Data Pipeline-Project
## An automated data pipeline for Covid19 Prediction and Reporting

### Goal of the Project
Building a reliable data pipeline to compile COVID-19 data from several sources, including government health departments, hospitals, and research institutes, would be the project's primary goal. These pipelines can clean, process, and integrate data into a centralized data lake or data warehouse, allowing it to be accessible for additional analysis, using the connections and transformations offered by Azure Data Factory. The overall task which needs to performed are as shown:

![Image_1_Project_overflow](https://github.com/rahulingle92/COVID-19-ETL_data_pipeline/assets/44425377/94e0e6b9-118f-4299-841e-654a5f31ceb5)



### The Datasets' source
In this project, The dataset is ingested to Azure Data Factory from two sources: first dataset is ingested from Azure Blob storage where dataset is stored from Eurostat website and other dataset is ingested directly from http i.e website of European Centre for Disease Prevention and Control (ECDC). 

![Image_2_Data_Ingestion](https://github.com/rahulingle92/COVID-19-ETL_data_pipeline/assets/44425377/d9adad45-d4c2-410e-b6bc-869570f564f0)

#### We received following details  from the ECDC  website:
 * Confirmed Cases on daily basis
 * Mortality due to COVID 19 on daily basis
 * Hospitalization / ICU cases
 * Testing Numbers
   
#### We received  following details from Eurostat website which is stored in Azure Blob Storage :
 * Country's Population by Age Group

### Solution Architecture 

![Image_3](https://github.com/rahulingle92/COVID-19-ETL_data_pipeline/assets/44425377/3da3bd9f-6af5-44a4-8483-2739296fa938)

### Storage Solutions used in this project

![Image_4_Storage_solution](https://github.com/rahulingle92/COVID-19-ETL_data_pipeline/assets/44425377/8b70aa2a-352f-4c28-8dac-a73a13c5fae6)



### The Datalake that we built with following data to help the data Scientist to predict the spread of the virus/ Mortality:
 * Confirmed Cases on daily basis
 * Mortality due to COVID 19 on daily basis
 * Hospitalization / ICU cases
 * Testing Numbers
 * Country's Population by Age Group
### The Data Warehouse that we built with the following data to aid reporting on Trends
 * Confirmed Cases on daily basis
 * Mortality due to COVID 19 on daily basis
 * Hospitalization / ICU cases
 * Testing Numbers
 * Country's Population by Age Group

### Environment setup
 * As the first step in Project implementation, we have set up Environment for the Project Deployment.
 * Initially we have deployed the Azure Data Factory for "Covid reporting project" Dashboard as below:

   ![image](https://github.com/rahulingle92/COVID-19-ETL_data_pipeline/assets/44425377/cd4925b1-de05-45d3-a95b-a154f586f02b)

* Then we have set up Azure storage account ( Named as "covidreportingsa0806" ) and it is deployed on "Covid reporting project" Dashboard as below:

  ![Image_6_Storage_Account_deployment](https://github.com/rahulingle92/COVID-19-ETL_data_pipeline/assets/44425377/429fabf7-1593-4d7b-bb54-dbdf12730f0b)

* Then we have created Azure Data Lake Gen2 account ( Named as "covidreportingdl0806") and it is deployed on "Covind reporting project" Dashboard as below:

  ![Image_7_Datalake_Storage_Account_Deployment](https://github.com/rahulingle92/COVID-19-ETL_data_pipeline/assets/44425377/2e617d91-eb82-4898-83e3-eda1ebb3e365)


 
   
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
