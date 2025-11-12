# ETLProjectWork
Keep record of projects which I have worked on recently as of 2023 to Present.

Project 1:
Correspondence Letters
Description:
Worked on ETL Development Project involving creation of XML file using columns from flat files which are fixed-width in length.
Skills:
PySpark, AWS Services like S3, Glue ETL, AWS Lambda, EventBridge, SQS, DynamoDB Tables
Source File:
.txt with fixed-width containing roughly around 500 columns
lookup reference tables which are .csv are ingested into staging layer in AWS Datalake.
Target File:
.xml file containing consolidated XMLs inside along with their respective categories with total XML counts.

Project 2:
MDM and Delta and Monthly File Creation
Description:
Worked on Delta logic to fetch columns like Policy, Effective Date, Policy Type which will be used to extract, transform and load staging datalake into AWS Athena.
Once the unique policies are identified, the contents are sent to MDM which will further be used to create ECN numbers for every policy-customer to uniquely identify their Master record called MDM data and metadata.
Skills: 
SparkSQL query transformation, AWS Services like S3, Athena, Glue ETL, AWS Lambda, EventBridge, SQS, DynamoDB Tables
Source File:
Staging datalake Athena tables.
Target File:
4 Files containing information such as Policy, Customer, Address which are .txt files with data outputs separated using pipe-delimited rows. A trigger .txt file having total counts is sent to downstream after the 3 file generation to kick-start further processes in other admin systems. 
