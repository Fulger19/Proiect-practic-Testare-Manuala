# Final project for ITF Manual Testing Course
The scope of the final project for ITF Manual Testing Course is to use all gained knowledge throught the course and apply them in practice, using a live application.

Application under test: https://demo.guru99.com/V4/index.php

API Documentation: https://docs.google.com/document/d/1rPW5DV82VJT6vtA1VDSrfxaCBuAduxW0zb1yfTh_VMk/edit

The final project will be split into 2 sections: **Testing section** and **SQL section**.

Tools used: JIRA, Zephyr Squad, Postman, MySQL Workbench.

# Functional specifications
This project is performed upon the below Story, which was created in JIRA and describes the functional specifications of the **New Customer** module for **Manager role**.

![image](https://github.com/Fulger19/Proiect-practic-Testare-Manuala/assets/135150028/6dc5b021-b7ac-442c-85e3-d53cf4eafdc6)


# 1 Testing section

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

**Tests in scope**: All the feature of **New Customer** module which were defined in software requirement specs need to be tested: functional testing, GUI testing and API testing.

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

The test cases with steps can be viewed here: https://github.com/Fulger19/Proiect-practic-Testare-Manuala/blob/main/ZFJ-issue-export-08-19-2023-242ac113-0001.xlsx

For the API testing, the following checklist was generated: XXXXXXXXXXXXXXXXXX

## 1.5 Test Implementation
The following elements are needed to be ready before the test execution phase begins:

- Testing environment is up and running: https://demo.guru99.com/V4/index.php
- Access to the testing environment is given: Username : mngr505316 | Password : ruvUver
- Cycle summary was created
- Test cases were added to the cycle summary
- Postman collection for the new users API methods was created
- Authorization token was created for accessing the API

## 1.6 Test Execution
- Test cases are executed on the created test Cycle summary: xxxxxx[Dependents_cycle_summary_execution.pdf]xxxxxxxxxxx
- Bugs have been created based on the failed tests. The complete bug reports can be found here: xxxxxxxxDependents_created_bugs.pdfxxxx
    - XXXXXXXXXXXX de adaugat ce bugs am gasit pe modelul de mai jos XXXXXXXXXXXXXX
    - Date format is not dd/mm/yyyy
    - Future "Date of Birth" can be selected from calendar
    - Only 50 characters are allowed for "Please Specify" field
    - Only 50 characters are allowed for "Name" field
    - Relationship "parent" is missing
- API tests are executed based on the checklist. The collection used can be found here: XXXXX JSON file with the collection of requests created for the Dependents API XXXXX
- Full regression testing is needed after the bugs are fixed

## 1.7 Test Completion
- As the Exit criteria were met and satisfied as mentioned in the appropriate section, this feature is suggested to ‘Go Live’ by the Testing team
- The traceability matrix was generated and can be found here: XXXXX Traceability_matrix.csv XXXXX - de actualizat numerele in functie de testele facute de mine !!!!!!!
- Test execution chart was generated, the final report shows that a number 5 tests have failed of a total of 23
- A number of 23 test cases were planned for execution and all of them were executed
- A number of 5 total bugs were found, from which the priority is: 1 is high, 4 are medium and 1 is low

Test execution chart

XXXXXXXXXXXXX

# 2 SQL section

Created a database named 'orangehrm' and a table named 'dependents' with all the columns needed to save data per specifications. Performed different queries inside the sql file: dependents.sql
  
