# AWS-Solutions-Architecture - Simple 3 Tier Architecture

A three-tier architecture composed of a frontend (HTML, CSS, JavaScript), backend (Apache Web Server and a Java application), and database (MySQL). The three-tier application hosts a dynamic website that accepts user traffic from the internet.

Users hit Route 53, then to Cloud Front for content delivery to edge location from static content hosted in S3. Dynamic content is served by the Application tier that gets routed through Internet Gatway and Web Tier in Public Subnet.

Both the App Tier and Data Base Tier are in Private subnets so that no direct request can be made by users for better security.

Also considering High Availibility and Resiliency the architecture is span across Availability Zones.

For Database, we have a Standby in case of DB failure and a Ready replica to serve Read Only requests.

![Architecting Solutions on AWS - Capstone Project - 3 Tier Architecture drawio](https://user-images.githubusercontent.com/8630317/206986574-cc889f93-447d-4606-886a-b041b5e63c57.png)
