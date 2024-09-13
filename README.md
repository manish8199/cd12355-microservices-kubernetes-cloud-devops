Operationalizing a Coworking Space Microservice

Project Overview: Coworking Space Service
The Coworking Space Service is a set of APIs that enables users to request one-time tokens and administrators to authorize access to a coworking space.

This service follows a microservice pattern and the APIs are split into distinct services that can be deployed and managed independently of one another.

Database Setup:
Postgresql DB is used for the project.

Ananlytics application:
Based on Python and build as a docker container image.

Container- AWS- EKS is used

Build Pipeline:
AWS Codebuild is utilized for codebuild process.

Troubleshooting:
AWS Cloudwatch container insights 
