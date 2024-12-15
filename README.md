
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
![image 000](https://github.com/user-attachments/assets/a70419bf-6d2f-44d0-a09d-436113eee21f)<br>
The above images displays the descryptive analysis of our DAP model.
#### Step 1: Data Ingestion
This step explains about the Data ingestion into AWS Environment
#### Step 2: Data Profiling
This step explain the data profiling in the AWS environment.
#### Step 3: Data Cleaning 
This step explaing the Data cleaning done using the AWS DataBrew service.
#### Step 4: Data Pipeline Design 
This step explain the process of designing a ETL pipeline to transform raw data into structured data.
