# Redmine Project  


### Revision History

| Date | Description   | Author   | Comments |
| :-----: | :---: | :---: | :---: |
| 05.09.2023 | Test Plan for version 1.0   | Andrada Pricop   | draft test plan |
| 09.21.2023 | v1.1  | Andrada Pricop   | Added more details for Test Process |
| 10.18.2023 | v1.1  | Andrada Pricop   | Added the final version for bugs report |


### Table of Content:

1. Introduction
    
            1.1 Project Objective 
            
            1.2 Functionalities in scope

            1.3 Functionalities and tests out of scope

2. Test process
    
            2.1 Test planning
            
            2.2 Test analysis

            2.3 Test design

            2.4 Test implementation

            2.5 Test execution

            2.6 Test closure

            2.7 Test monitoring and control

3. Test deliverables
    
            3.1 Test plan
            
            3.2 Test conditions

            3.3 Test cases

            3.4 Daily test summary reports

            3.5 Traceability matrix

            3.6 Test case results

            3.7 Bugs report

            3.8 Test completion report


### 1 Introduction
Redmine is a flexible project management web application. Written using the Ruby on Rails framework, it is cross-platform and cross-database.

Redmine is open source and released under the terms of the GNU General Public License v2 (GPL).


### 1.1 Project Objective
We need to raise the trust in the quality of the project as high as possible before releasing it to customers.


Application under test: https://www.redmine.org/ 


Documentation: https://www.redmine.org/guide


### 1.2 Functionalities in scope
  - All the features of My account module which were defined in Redmine business requirements will be tested using the following testing types: functional testing, GUI testing, API testing. 
  - The Redmine Web application will be tested on latest versions of Chrome and IE.


### 1.3 Functionalities and tests out of scope
  - All the features that are not under My account  module 
  - Non-functional testing like stress, performance is beyond scope of this project
  - No QA support for mobile applications developed, only web applications will be tested
  - Automation testing is beyond scope.

 
### 2 Test process
### 2.1 Test Planning

| Roles | Responsabilities | 
| :-----: | :---: |
| Andrada - Tester |  will test: all features from My account module: Information, Email notifications, Email address, Preferences and Password | 


#### Entry criteria:
- roles needed for the project are allocated
- functional specifications are defined
- completion of the software development phase
- availability of the test environment
- availability of test data
- approval of test plans and test cases
- resolution of critical defects
- availability of test resources

#### Exit criteria:
- 100% tests from Functional testing were wxecuted and 58.33% are passed
- 100% tests from GUI testing were executed and 80% are passed
- critical issues that were previously 'in progress' have now been resolved
- update tests are 100% passed 
- exploratory testing was performed on My account module

#### Risks:

##### Product risks
- stress conditions might impact the web application
- new browser might not be supported

##### Project risks
- stability risks (crashes, disconnects, etc)
- IE browser might have performance issues
- the web page pagination could be impacted when opened on mobile devices


### 2.2 Test analysis 
Analyze the business requirements to make sure that we have all the details for creating the test conditions 
Write test conditions (What?)
we plan on running a full regression test on the current version


[Test Conditions](https://github.com/Andrada2192/RedmineProject/blob/main/TestConditions.pdf)


Risk Analysis - covers potential project and product risks that may arise during the testing process of the Redmine web application

| Numele riscului | Risc de proiect   | Risc de produs   | Probabilitate | Impact | Risk level(Probabilitate x impact)​ |
| :-----: | :---: | :---: | :---: | :---: | :---: |
| Incompatibilitatea cu browserele ar putea duce la funcționarea necorespunzătoare a aplicației pe diverse platforme de navigare. |    | x   | 1 | 3 | 3 |
| Posibile probleme de afișare a ecranului "Information" ar putea afecta experiența utilizatorului și ar putea necesita eforturi suplimentare pentru remediere. |   | x   | 3 | 5 | 15 |
| Notificările de email nepotrivite ar putea genera confuzie sau disconfort utilizatorilor.​ |   | x   | 3 | 4 | 12 |
| Preferințele neactualizate ale utilizatorilor ar putea duce la erori sau la funcționarea necorespunzătoare a funcționalităților personalizate.​ |  | x | 2 | 3 | 6 |
| Există riscul unui eșec în actualizarea parolei, care ar putea bloca accesul utilizatorilor la conturile lor.​ |  | x | 3 | 3 | 9 |
| Întârzierea în livrarea screen-urilor din pagina "My Account" ar putea afecta experiența utilizatorului.​ |  | x | 3 | 1 | 3 |
| Un buget insuficient pentru dezvoltarea funcționalității "Preferences" ar putea limita capacitatea de a implementa complet această caracteristică.​ | x |  | 2 | 4 | 8 |
| Resursele umane inadecvate pentru gestionarea notificărilor prin email ar putea duce la întârzieri sau la livrarea unor notificări incoerente.​ | x |  | 2 | 3 | 6 |
| Vulnerabilitățile de securitate în ecranul "Preferences" pot să expună datele sensibile ale utilizatorilor la riscul de acces neautorizat sau de compromitere a securității.​ |  | x | 2 | 3 | 6 |
| Incompatibilitatea cu selecția limbilor din meniul dropdown ar putea limita accesibilitatea aplicației pentru utilizatorii care preferă alte limbi.​ |  | x | 3 | 3 | 9 |
| Posibile probleme de performanță la schimbarea limbii ar putea duce la întârzieri sau la încetiniri ale aplicației, afectând experiența utilizatorului.​ |  | x | 3 | 3 | 9 |







### 2.3 Test design
-all the test cases are written and reviewed 

-all test cases will be created in Jira as test management tool


### 2.4 Test implementation
all the test data is available and reviewed (an account with Admin Role was created)
this test run includes only regression testing in which we will run tests that have the highest priority, this will be main priority
Test suites are created (Cycle Summary was created)


### 2.5 Test execution
-All tests will be executed on the following browsers: Chrome and IE if time will be available we will extend tests on Mozilla and Brave browsers

-Completed GUI and functional testing

-Executed a number of 8 GUI tests, with the majority(7) resulting in a "pass" status, one of them having "fail" status

-Executed a number of 11 functional tests, 6 of them resulting in a "pass" status, 4 of them having "fail" status and one being blocked

-Bugs will be created based on the failed test cases and reported and are currently undergoing remediation. After their resolution, retesting and regression testing will be performed


### 2.6 Test closure
100% tests were executed and 90% of them are passed 
no Critical issues have Open status


### 2.7 Test monitoring and control
Various periodic reports will be generated to reflect the current status of testing process, in case of major problems control measures could be taken. 



### 3 Test deliverables
### 3.1 Test plan


### 3.2 Test conditions 
 - we will use prod environment
 - testing using new accounts or existing account is necessary
   
[Test Conditions](https://github.com/Andrada2192/RedmineProject/blob/main/TestConditions.pdf)



### 3.3 Test cases
[Test Cases](https://github.com/Andrada2192/RedmineProject/blob/main/TestCases.pdf)



### 3.4 Daily test summary report
#### The report generated on 11/07/2023 shows the execution of 10 test cases, out of which 3 failed and 1 was blocked.
![Daily report](https://github.com/Andrada2192/RedmineProject/blob/main/daily%20rep%207noi%20(2).png)  
![Daily report](https://github.com/Andrada2192/RedmineProject/blob/main/daily%20rep%207noi.png)


#### The report generated on 11/09/2023 shows the execution of 12 test cases, out of which 4 failed.
![Daily report](https://github.com/Andrada2192/RedmineProject/blob/main/386886359_638780408179584_6632357104543974468_n.png)
![Daily report](https://github.com/Andrada2192/RedmineProject/blob/main/380826740_876341894084574_3891748152558190536_n.png)



### 3.5 Traceability matrix
![Traceability Matrix](https://github.com/Andrada2192/RedmineProject/blob/main/traceability%20matrix.jfif)
           


### 3.6 Test case results
[Test Case Results](https://github.com/Andrada2192/RedmineProject/blob/main/TestCaseResult.pdf)



### 3.7 Bugs report
[Bugs Report](https://github.com/Andrada2192/RedmineProject/blob/main/BugsReport.pdf)



### 3.8 Test completion report
![Test Completion](https://github.com/Andrada2192/RedmineProject/blob/main/TestExecution.png)

- GUI testing: 7 out of 8 tests passed (87.50%), with one test failing (12.50%).

- Functional testing: 6 out of 11 tests passed (54.55%), 4 tests failed (36.36%), and one test was blocked (9.09%).

In conclusion, GUI testing has a higher pass rate (87.50%) compared to functional testing (54.55% pass rate). Functional testing shows a significant number of failures (36.36%). This suggests a need for further attention to improve functional test effectiveness.


### 3.9 Schedule
 - we have 3 days of testing
 - we have 19 test cases 
 - in order to finish the regression run we would need to run 6/7 tests/day

