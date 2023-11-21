# Final project for ITF Manual Testing Course
The scope of the final project for ITF Manual Testing Course is to use all gained knowledge throught the course and apply them in practice, using a live application.

Application under test: https://demo.guru99.com/V4/index.php

Documentation: https://docs.google.com/document/d/1rPW5DV82VJT6vtA1VDSrfxaCBuAduxW0zb1yfTh_VMk/edit

The final project will be split into 3 sections: **1. Testing section**, **2. API Section** and **3. SQL section**.
- Testing will be done for: https://demo.guru99.com/V4/index.php
- API testing will be done for: https://developer.spotify.com/documentation/web-api
- SQL testing will be done for the students in the 8th grade

Tools used: JIRA, Zephyr Squad, Postman, MySQL Workbench.

# 1. Testing section

# Functional specifications
This project is performed upon the below Story, which was created in JIRA and describes the functional specifications of the **New Customer** module for **Manager role**.

![image](https://github.com/Fulger19/Proiect-practic-Testare-Manuala/assets/135150028/399351a1-9b17-4f7b-881c-bf7fc5a1b48e)


## 1.1 Test Planning
The Test Plan is designed to describe all details of testing for the **New Customer** module for **Manager role** from the Guru99 application.

The plan identifies the items to be tested, the features to be tested, the types of testing to be performed, the personnel responsible for testing, the resources and schedule required to complete testing, and the risks associated with the plan.

### 1.1.1 Roles assigned to the project and persons allocated
- Project manager - Francesco Gabbani
- Product owner - Marco Mengoni
- Software developer - Angelina Mango
- QA Engineer - Irina Fulger

### 1.1.2 Entry criteria defined
- functional specifications are defined
- roles needed for the project are allocated
- initial project risks were detected and mitigated

### 1.1.3 Exit criteria defined
- number of unresolved bugs is insignificant or they have low priority
- all tests have been executed
- all resolved bugs have been re-tested and approved by the QA team
- deadline was reached
- no detected major risk remained un-mitigated
- exploratory regression testing must be performed on the **New Customer** module for **Manager role**
  
### 1.1.4 Test scope

**Tests in scope**: All the features of **New Customer** module which were defined in software requirement specs need to be tested: functional testing, GUI testing and API testing.

**Tests not in scope**: performance testing, integrations of the above modules with other modules, compatibility testing with multiple browsers

### 1.1.5 Risks detected
**Project risks**: lack of experience of the QA team, new team members not well integreted yet, insufficient budget.

**Product risks**: application not working if all database is moved to a new server.

### 1.1.6 Evaluating entry criteria
The entry criterias defined in the Test Planning phase have been achieved and the test process can continue.

## 1.2 Test Monitoring and Control
Various periodic reports were generated to reflect the current status of the testing process, in case of major problems control measures could be taken. The following status report was generated after 40% of the test cases were executed, on July 1st, 2023:

![image](https://github.com/Fulger19/Proiect-practic-Testare-Manuala/assets/135150028/c2988eb8-b38a-4d13-80f1-ece579b9631b)


## 1.3 Test Analysis
The testing process will be executed based on the above requirements for the **New Customer** module for **Manager role**. The following test conditions were found:

- Enter data only for mandatory fields and check that the New Customer is created
- Enter data for all available fields and check that the New Customer is created
- Leave mandatory fields empty and check that the New Customer cannot be created
- Check all validation constraints for the fields

## 1.4 Test Design

Functional test cases were created in Zephyr Squad. Based on the analysis of the specifications, the test design techniques used for generating test cases are boundary value analysis, equivalence partitioning and use case testing.

**Test cases**

![image](https://github.com/Fulger19/Proiect-practic-Testare-Manuala/assets/135150028/2458ad39-98f3-443c-b794-e56e7b3b4d51)

The test cases with steps can be viewed here: https://github.com/Fulger19/Proiect-practic-Testare-Manuala/blob/main/ZFJ-issue-export-08-19-2023-242ac113-0001%20(2).xlsx

## 1.5 Test Implementation
The following elements are needed to be ready before the test execution phase begins:

- Testing environment is up and running: https://demo.guru99.com/V4/index.php
- Access to the testing environment is given with the following email address vahah14739@goflipa.com. This should be used on https://demo.guru99.com/ in order to obtain an username and a password to access the test environment.
- Cycle summary was created
- Test cases were added to the cycle summary
- Postman collection for the new users API methods was created
- Authorization token was created for accessing the API

## 1.6 Test Execution
- Test cases are executed on the created test Cycle summary: 
- 2 bugs have been created based on the failed tests. The complete bug reports can be found here: https://github.com/Fulger19/Proiect-practic-Testare-Manuala/blob/main/bug%20reports.JPG
    - Email - special characters are not allowed
    - Date format is not dd/mm/yyyy
- Full regression testing is needed after the bugs are fixed

## 1.7 Test Completion
- As the Exit criteria were met and satisfied as mentioned in the appropriate section, this feature is suggested to ‘Go Live’ by the Testing team
- The traceability matrix was generated and can be found here: [Traceability_matrix](https://github.com/Fulger19/Proiect-practic-Testare-Manuala/blob/main/Traceability_matrix_Guru99.xlsx)
- Test execution chart was generated, the final report shows that a number 2 tests have failed of a total of 36
- A number of 36 test cases were planned for execution and all of them were executed
- A number of 2 total bugs were found, for which the priority is medium

Test execution chart

![image](https://github.com/Fulger19/Proiect-practic-Testare-Manuala/assets/135150028/87704713-be30-4be2-889c-4f0457f4bd0d)

# 2. API testing

The API documentation can be found here: https://developer.spotify.com/documentation/web-api

Authentification documentation: https://developer.spotify.com/documentation/general/guides/authorization/

For the API testing a checklist with additional information can be found here: https://github.com/Fulger19/Proiect-practic-Testare-Manuala/blob/main/API_test_checklist.xlsx

Some of the API responses can be found here: 
- https://github.com/Fulger19/Proiect-practic-Testare-Manuala/blob/main/response_artist%20albums.json
- https://github.com/Fulger19/Proiect-practic-Testare-Manuala/blob/main/response_catalog%20artist.json
- https://github.com/Fulger19/Proiect-practic-Testare-Manuala/blob/main/GET_403%20error.JPG

# 3. SQL section

The SQL testing was done for the students in an 8th grade.
Created a database named 'scoala89' and two tables named 
- 'copii8C' with columns containing identification information
- 'note8C' with columns containing grades for Mathematics and Romanian
Performed different queries inside the sql file: https://github.com/Fulger19/Proiect-practic-Testare-Manuala/blob/main/SQL_Project_IT_Factory.txt
Some of the queries can be found here:
- all the children from the classroom - https://github.com/Fulger19/Proiect-practic-Testare-Manuala/blob/main/SQL_table%201.JPG,
- all children born in 2008 - https://github.com/Fulger19/Proiect-practic-Testare-Manuala/blob/main/SQL_table%202.JPG,
- all grades for Mathematics and Romanian - https://github.com/Fulger19/Proiect-practic-Testare-Manuala/blob/main/SQL_table%203.JPG,
- all children with at least one grade less then 5 - https://github.com/Fulger19/Proiect-practic-Testare-Manuala/blob/main/SQL_table%204.JPG  
