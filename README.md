
# Part 1 - [Descryptive Analysis of Rental Standards of Vancouver City](https://elishatioluwaseajayi.github.io/Descriptive-Analysis-of-Rental-Standards/)
* For anyone planning to move to Vancouver or even those living in Vancouver may need to analyse the details of rental and locations with additional information of facilities like hospitals, library, schools and other near it.
* Similarly here I am planning to do descriptive analysis of the details of rentals in each location and also the exploratory analysis of rental units in each of these locations.
* This is mainly to identify which of these areas have high rental units available throughout Vancouver.
* The dataset taken by me is about the  “Rental Stanadards” segment of the “Property” module of the Vancouver city portal.
* In this we have key features like the ‘Business Operators’, ‘Total Units’, ‘Total Outstanding Units’, ‘Street Number’,  ‘Street Name’ and other details.
* The descriptive analysis is on “What is the percentage of number of available Rental  Business Operators in each Geo-areas of Vancouver?”.
#### Dap Design
![image 001](https://github.com/user-attachments/assets/eaf89db3-722c-4b6a-b718-6792029bac32)<br>
The above image displays the DAP design we are implementing for the descyptive analysis.
#### Data Questions (Metric)
Using the above dataset details we will be finding below details as part of our analysis of the descriptive metric:
* Total available operators grouped based on the geo local area.
* The total available operators in Vancouver city altogether.
* Find the information on the percentage split of the operators from each geo local area in detail by dividing the available operators in each geo local are with that of the total available operators in Vancouver.
* Below I mentioned the 4 step process involved in the DAP design related to the descriptive question posted above analysis (highlighted and underlined).
* We are going to use the AWS services like S3, Glue, Glue DataBrew as per our need to store the results and other details of the project.
#### Descriptive  Question for Analysis
* The primary need of this project is to conduct a descriptive and Exploratory Analysis of Vancouver City rental standards based on the datasets taken from City of Vancouver Open Data Portal.
* The hope with this question was to gain insight into how accessible the rental properties are in Vancouver City.
* As informed earlier the dataset select by me is about the “Rental Standards”. Here the descriptive metric Ajayi planned to analyse is about “What is the percentage of number of available Rental Business Operators in each Geo-areas of Vancouver?”
* For this the dataset select is the “Rental Standards” from the City of Vancouver Open Data Portal website.
* This dataset has information of the Business operator, their url, the business address details(like Business Operators, Details url, street name and others), the outstanding units and total units. I selected the dataset related to rentals in Vancouver.
* I selected to work on the rental agencies in different areas of Vancouver.
* This second part of the DAP design includes the next process of DAP that is once the needed analysis data is available after Glue pipeline design.
* This included multiple details and segments discussed below.
![image 000](https://github.com/user-attachments/assets/a70419bf-6d2f-44d0-a09d-436113eee21f)<br>
The above images displays the descryptive analysis of our DAP model. 
#### Step 1: Data Ingestion
* This step explains about the Data ingestion into AWS Environment.
* Previously we decided that the descriptive metric is “What is the percentage of number of available Rental  Business Operators in each Geo-areas of Vancouver?”.
* We also took the details of dataset from the ‘Vancouver.ca’ website. Now we decide how we are going to make them available for in the AWS portal for usage and also for analysis purpose.
* To do this the solution we have is ‘S3’ buckets. We are going to create 2 buckets namely “vrs-raw-ajayi” and “vrs-transformed-ajayi”.
* The bucket “vrs-raw-ajayi” stores the raw data taken from the ‘Vancouver.ca’ website and “vrs-transformed-ajayi” stores the cleaned and transformed datasets.
* Inside the “vrs-raw-ajayi” bucket we will be creating a ‘Ingestion-year-2024’ folder to store the details of the ‘Rental Stnadards’.
* We will also create 3 folders inside “vrs-transformed-ajayi” bucket called ‘Data-cleaning’, ‘Data-profiling’ and ‘Rental-Operators’.
* This is to store the details respectively for these stages. Below are the images showing these storage details.
![image 001](https://github.com/user-attachments/assets/eaf89db3-722c-4b6a-b718-6792029bac32)<br>
The above image displays the DAP design we are implementing for the descyptive analysis.
![image 002](https://github.com/user-attachments/assets/efd81569-7dae-42e5-a2fe-1d10330018fb)<br>
* The above image shows the buckets created
![image 003](https://github.com/user-attachments/assets/80b487a5-5218-4d5b-b3be-a9fd54193bc5)<br>
* The above image shows the excel file uploaded in the folder inside raw bucket.
#### Step 2: Data Profiling
* This step explain the data profiling in the AWS environment.
* During Profiling we will be do a detailed understanding on the dataset we selected.
* Like we will be checking on the data, its quality, validity, and other details.
* We will mainly even be checking if these data values are valid, there are any missing value or other issues with the data and its structure.
![image 003-2](https://github.com/user-attachments/assets/7307db4b-4734-4b66-92bb-5f6d9c82a8ff)<br>
* The above image shows an important step of profiling in DAP design.
![image 003-1](https://github.com/user-attachments/assets/787a7dda-2bf8-4316-bec8-ec1a2cbbd102)<br>
* The above image shows the dataset profiling job created.
![image 004](https://github.com/user-attachments/assets/304e6d70-5cb6-4cf6-bd10-736613a52989)<br>
* The above image shows the result of the data profiling job created.
![image 004-2](https://github.com/user-attachments/assets/6861fe13-4f7e-439a-bdb9-6aae1d06e3dc)<br>
* The above image shows the result of the dataset profiling job created.
![image 005](https://github.com/user-attachments/assets/56650528-4193-4e72-b669-4c89f8f8fd19)<br>
* The above image shows the column statistics results of the dataset profiling job created.
![image 006](https://github.com/user-attachments/assets/c49fb566-f80d-4969-818e-5d6d2444dbbe)<br>
* The above image shows the dataset lineage result of the dataset profiling job created.
#### Step 3: Data Cleaning 
* This step explaing the Data cleaning done using the AWS DataBrew service.
* 
#### Step 4: Data Pipeline Design 
This step explain the process of designing a ETL pipeline to transform raw data into structured data.
