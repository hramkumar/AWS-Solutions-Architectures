# AWS-Solutions-Architecture - Data Analytics Architecture

A Data Analytics Architecture to migrate nearly any amount of data from an on-premises Apache Hadoop environment to AWS and store it in S3.

Currently the data is stored in On Premise Data center and if a power outage occurred in the data center, all systems would be brought offline.

Until data is migrated to AWS, Direct Connect is added to the architecture. Once it is all migrated to S3, we can use Athena to query the details using SQL and Quicksight visualization to derive insights.

**For migration we are using Anazon DataSync to migrate from on premise to S3. **


![Architecting Solutions on AWS - Capstone Project - Data Analytics drawio](https://user-images.githubusercontent.com/8630317/207009408-3c684772-7b67-4bf1-8d44-a3dbcad4fdcc.png)
