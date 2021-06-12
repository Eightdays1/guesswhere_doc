# Test plan

## 1.	Introduction
### 1.1	Purpose
The purpose of the Iteration Test Plan is to gather all of the information necessary to plan and control the test effort for a given iteration. 
It describes the approach to testing the software.
This Test Plan for vnv supports the following objectives:
-	Identifies the items that should be targeted by the tests.
-	Identifies the motivation for and ideas behind the test areas to be covered.
-	Outlines the testing approach that will be used.
-	Identifies the required resources and provides an estimate of the test efforts.

### 1.2	Scope
This document describes the used tests.

### 1.3	Intended Audience
This document is meant for internal use primarily.

### 1.4	Document Terminology and Acronyms
- **SRS**	Software Requirements Specification
- **n/a**	not applicable
- **tbd**	to be determined

### 1.5	 References
| Reference        | 
| ------------- |
| [Blog](https://guesswheregame.wordpress.com/) | 
| [SRS](https://github.com/Eightdays1/guesswhere_doc/blob/master/SRS.md) |
| [SAD](https://github.com/Eightdays1/guesswhere_doc/blob/master/SAD.md) |
| [UC1 Game](https://github.com/Eightdays1/guesswhere_doc/blob/master/UseCases/Use-Case_Game.md) |
| [UC2 Start Game](https://github.com/Eightdays1/guesswhere_doc/blob/master/UseCases/Use-Case_StartGame.md) |
| [UC3 Challenge User](https://github.com/Eightdays1/guesswhere_doc/blob/master/UseCases/Use-Case_Challenge_User.md) |
| [UC4 Options](https://github.com/Eightdays1/guesswhere_doc/blob/master/UseCases/Use-Case_Options.md) |
| [UC5 Statistics](https://github.com/Eightdays1/guesswhere_doc/blob/master/UseCases/Use-Case_Statistics.md) |

## 2.	Evaluation Mission and Test Motivation
### 2.1	Background
By testing our project, we make sure that all changes to the sourcecode do not break the functionality. Also by integrating the test process in our deployment process, we make sure that only working versions of our project getting deployed.
### 2.2	Evaluation Mission
n/a
### 2.3	Test Motivators
Our testing is motivated by 
- quality risks 
- technical risks 
- use cases 
- functional requirements

## 3.	Test Approach
### 3.1	Testing Techniques and Types
We used Unit-tests to test the Applications components and API-Test using Postman to test the APIs Responses.

#### 3.1.1	Unit Testing
|||
|---|---|
|Technique Objective|All Unit-Tests run without producing an error|
|Technique|Unit testing|
|Oracles|Valid data is provided, for example a valid username and a valid password|
|Required Tools|Android Studio and JUnit|
|Success Criteria|All tests pass without an error|
|Special Consideration|-|
#### 3.1.2	Business Cycle Testing
n/a

#### 3.1.3	API Testing
|||
|---|---|
|Technique Objective|The API responses correctly to requests|
|Technique|API testing|
|Oracles|Valid data is provided, for example a valid username and a valid password|
|Required Tools|Postman|
|Success Criteria|All tests pass without an error|
|Special Consideration|-|

#### 3.1.4	Performance Profiling 
n/a

#### 3.1.5	Load Testing
n/a

#### 3.1.6	Stress Testing
n/a
 
#### 3.1.7	Volume Testing
n/a

#### 3.1.8	Security and Access Control Testing
n/a

#### 3.1.9	Failover and Recovery Testing
n/a

#### 3.1.10	Configuration Testing
n/a

#### 3.1.11	Installation Testing

|||
|---|---|
|Technique Objective|The App is installed on the device|
|Technique|Installation testing|
|Oracles|-|
|Required Tools|-|
|Success Criteria|The installation is successful|
|Special Consideration|-|

## 4.	Entry and Exit Criteria
### 4.1	Test Plan
**n/a**
#### 4.1.1	Test Plan Entry Criteria
**n/a**
#### 4.1.2	Test Plan Exit Criteria
When all tests pass without throwing an exception.
#### 4.1.3 Suspension and Resumption Criteria
n/a

## 5.	Environmental Needs
### 5.1	Base System Hardware
n/a

### 5.2	Base Software Elements in the Test Environment
Android Studio
JUnit
Andoid VM or Andoid Smartphone
Postman

### 5.3	Productivity and Support Tools
n/a

### 5.4	Test Environment Configurations
### 5.4.1 Android Studio Configuration
1. Run-Configuration "Android JUnit"
2. Testclass: com.example.guesswhereapp.UnitTest

### 5.4.2 Postman Configuration
1. Environment to hold Environment-Variables
2. Environment-Variables for the Access-Token and the Game-Id
3. [Collection](https://github.com/Eightdays1/guesswhere_doc/blob/master/documentation/Tests/API-Tests/API-Test_postmanCollection) to run the tests
4. HTML-Requests and their test-parameters

## 6.	Responsibilities, Staffing, and Training Needs
### 6.1	People and Roles
This table shows the staffing assumptions for the test effort.
|Role|Minimum Resources Recommended(number of full-time roles allocated)|Specific Responsibilities or Comments|
|---|---|---|
|Test Manager|1|Provides management oversight.  Responsibilities include:  planning and logistics  agree mission  identify motivators acquire appropriate resources present management reporting advocate the interests of testevaluate effectiveness of test effort|
|Test Designer|1|Defines the technical approach to the implementation of the test effort.  Responsibilities include: define test approach define test automation architecture verify test techniques define testability elements structure test implementation|
|Tester|1|Implements and executes the tests. Responsibilities include: implement tests and test suites execute test suites log results analyze and recover from test failures document incidents|
|Test System Administrator|1|Ensures test environment and assets are managed and maintained. Responsibilities include: 	administer test management system install and support access to, and recovery of, test environment configurations and test labs|
|Database Administrator|1|Ensures test data (database) environment and assets are managed and maintained. Responsibilities include: support the administration of test data and test beds (database)|
|Implementer|1|Implements and unit tests the test classes and test packages. Responsibilities include: creates the test components required to support testability requirements as defined by the designer|

### 6.2	Staffing and Training Needs
n/a

## 7.	Risks, Dependencies, Assumptions, and Constraints
| Risk | Mitigation Strategy	| Contingency (Risk is realized) |
|---|---|---|
| Untestable features in <br/>the framework | Cannot be avoided | Try to test it with integration tests |
| Testing scenario is not <br/>covered | Carefully design tests | Add scenario | 
| Technical Difficulties for Testers | Try to help remote | Try it out on different browsers before and check the availability on multiple systems | 
## 8. Management Process and Procedures
n/a
