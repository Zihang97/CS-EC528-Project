# CS/EC528-Project

## 1. Vision and Goals Of The Project:

Self Service Cloud-Native Data Analysis Platform is a platform for data scientists to ingest and analyze data on the cloud using varying levels of managed services based on user requirements.

Goals:
- Select tools and services for each component (Compute, Storage, Data Analysis, Security, and UI) based on tradeoffs of using managed services versus custom solutions
- Develop data science infrastructure within the cloud that can:
  - Pull and store data in cloud storage solution
  - Perform transform operations on data
  - Leverage standardized data science softare (Tensorflow, BigQuery, etc.)

** **

## 2. Users/Personas Of The Project:
The platform will be used by data scientists from companies and government institutions.
- A user who wants to extract data from a remote S3 bucket
- A user who needs to query and search a specific item in the data
- A user who wants to compute the average of multiple data
- A user who wants to use linear regression to find relationship between two factors of the data
- A user who needs to use machine learning models to draw inferences about the data
 


It doesn’t target:
- End-users who need to deal with extremely large datasets
- End-users who follow standard pipeline and don’t need customized solution
- Institutions with unique use cases considering the development of their own service

** **

## 3.   Scope and Features Of The Project:

- Self-service allocation based on the description of the detailed pipeline component needs.
- Leverages standardized software to analyse data.
- Provides storage for user data which is able to pull data from one or multiple source
- Provides ability to run python codes to transform and analyze data
- Provides support for sql commands to query the database
- Security: only select users are able to access and modify the data.
- Ability for multiple users to use simultaneously and independently

** **

## 4. Solution Concept
High-level outline of the solution:
- Storage for Data: cloud-native technologies like AWS S3/GCP GCS/ DynamoDB/Spanner
- Computing Engine: use existing IaaS solutions like AWS EC2 or GCP (can also use Container solution) 
- Data Analysis: use data analysis platforms like Jupyter and Pandas to support machine learning codes of Tensorflow/Pytorch. (We could start simple with sklearn just to test our pipeline)
- Permission and Access Control: Provide security solutions between services and external access (Cloud IAM).  
Strech Goals:
- Front-end UI: HTML/CSS/JS for webpage and  Python Flask for web application

** **

## 5. Acceptance criteria
Minimum acceptance criteria is a self service platform that can:  
- Extract data from a cloud storage service and return it.
- Support standardised data science software (tensorflow, BigQuery etc).
- Allocate storage and computation resources to ETL pipelnes based on user requirement.


Stretch goals include:
- Use this project to analyze Boston Open Data
- Provide several compute and size options
- Build a user friendly UI to interact with the platform

** **

## 6.  Release Planning:
Release #1 (due by Week 5) - [Demo #1](https://drive.google.com/file/d/1oXEU7WKBcbGg8-MOb6BIO_EFvi4C5_9g/view?usp=sharing):
- Data extraction and storage  
- When end-users decide to upload the data, we can extract the data from their buckets and store them in our built databases.

Release #2 (due by Week 9) - [Demo #2](https://drive.google.com/file/d/1xs2OyQpqQeajm7Ldirc7uzXbDh8Poh07/view?usp=sharing):
- Data transformation

Release #3 (due by Week 11):
- Incorporation of standardized data science software.

Release #4 (due by Week 13):
- Security and access

Release #5 (due by Week 15):
- Final Product and report

** **

## Mentors
- Dan Hyland: dan.hyland@twosigma.com
- Edward Yang: edward.yang@twosigma.com

## Team
- Ibrahim Chand: ichand@bu.edu
- Zihang Jiang: jzh15@bu.edu
- Anish Yennapusa: anishry@bu.edu
- Ze Yu: zey@bu.edu
