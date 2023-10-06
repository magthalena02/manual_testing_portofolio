!!!!de inlocuit cu datele proiectului!!!!!
# Final project for ITF Manual Testing Course

The scope of the final project for ITF Manual Testing Course is to use all gained knowledge throught the course and apply them in practice, using a live application. 

Application under test: www.houzz.com

API Documentation: 

**The final project will be split into 2 sections: [Testing section](https://github.com/julai215/itf_final_project_example_and_portofolio/blob/main/Final%20Project/README.md#1-testing-section) and [SQL section](https://github.com/julai215/itf_final_project_example_and_portofolio/blob/main/Final%20Project/README.md#2-sql-section).**

Tools used:

# Functional specifications

- Create account for new user on www.houzz.com
- Search bar implementation for www.houzz.com
- Create an ideabook as a user on www.houzz.com

# 1 Testing section

## 1.1 Test Planning

The Test Plan is designed to describe all details of testing for the X module from the OrangeHRM application. 

The plan identifies the items to be tested, the features to be tested, the types of testing to be performed, the personnel responsible for testing, the resources and schedule required to complete testing, and the risks associated with the plan

#### 1.1.1 Roles assigned to the project and persons allocated

- **Test Lead:** Responsible for overall test planning and execution
- **Test Engineer:** Responsible for developing test cases and scripts, and executing tests
- **Developer:** Responsible for fixing defects and providing support during testing
- **Server administrator:** Responsible for maintaining the test environment

#### 1.1.2 Entry criteria defined

- Ensure that the testing environment of the website is accessible and stable.
- User registration feature is fully developed, accessible and functional, and registration form is accessible.
- Search bar is implemented and visible in the user interface, and data search queries give expected results.
- Ideabook creation feature is fully developed and integrated into website, accessible and functional and users have access to relevant project or design idea data.
  
#### 1.1.3 Exit criteria defined

- Ensure that all the test cases must be executed and passed
- Verify that there are no critical defects (severity level high)
- Confirm that all the test deliverables must be completed and submitted.
- Performance test should pass the threshold limit.
  
#### 1.1.4 Test scope

* __Tests in scope:__
- Ensure that the users can create new account using a valid email address and they choose strong and secure passwords during account creation.
- Users should receive appropiate error message when attempting to create account with invalid email address or incorrect paswword and they can access their profiles with newly created account.
- Confirm that users can enter search queries in the search bar and the results are displayed based on input.
- Using filters by categories or other relevant criteria refine search results and the user receive search suggestions useful as they type in the search bar.
- The registered users can create ideabooks to save and organize design ideas and projects.
- Items added are correctly associated with the users's ideabook and any change made is saved and is reflected in the user account.
  
* __Tests not in scope:__
- Testing of authentication methods such as social media login (Google, Facebook), password recovery or account reset functionality is not in scope for this plan.
- In-depth testing of the search algorithm's accuracy and relevance ranking is not within the scope.
- Performance testing for scenarios involving an exceptionally large number of ideabooks or projects is not covered here.
- Testing of ideabook integration with other functionalities (e.g. purchasing items, sharing ideabooks) is not part of this scope.

#### 1.1.5 Risks detected

* Project risks:
- The testing plan may be affected if there are unresolved technical dependencies with other components or services (e.g., third-party authentication providers) that are necessary for account creation.
- There is a risk of data privacy and security breaches during account creation which could lead to data leaks or unauthorized access.
- As user traffic increases, there may be performance scalability issues with account creation or search functionality, leading to slow response times or system failures.
- Variations in browser behavior and compatibility issues may affect the functionality of account creation, search, or ideabook features.
- Frequent changes or updates to the website's codebase may lead to regression testing challenges, making it difficult to maintain test suites.
  
* Product risks:
- The potential risk of data breaches or unauthorized access to user account information or ideabook data could harm the reputation and trustworthiness of the website.
- Poor usability and a subpar user experience can result in frustrated users who may abandon the website. This risk could impact user retention and engagement.
- Performance issues, such as slow page load times or unresponsive search functionality, can lead to user dissatisfaction and abandonment.
- Incompatibility with different browsers and devices can result in a poor user experience and reduced website accessibility.
- Integration issues with third-party services or external search engines may disrupt the seamless operation of the website's search functionality.
- Weak password management or inadequate security measures may expose user accounts to hacking attempts.
- Data migration from legacy systems to the new website may lead to data loss, inaccuracies, or inconsistencies.

#### 1.1.6 Evaluating entry criteria

The entry criterias defined in the Test Planning phase have been achieved and the test process can continue. 

## 1.2 Test Monitoring and Control

It will be done by generating periodic reports that reflect the current status of the test.

## 1.3 Test Analysis

The testing process will be executed based on the above requirements for the Dependents module. The following test conditions were found:
- The account can be created successfully and the user can log in.
- An error message is displayed if the email address have invalid format or the password does not meet the stregth requirements.
- Relevant search results related to the query are displayed.
- The search results are filtered based on selected criteria.
- Relevant search suggestions are displayed as the user types in the search bar.
- The ideabook is created successfully and is accessible in the user's account.
- The selected projects or ideas are associated with the ideabook and can be viewed within it.

## 1.4 Test Design

Functional test cases were created in Zephyr Squad. Based on the analysis of the specifications, the test design techniques used for generating test cases 
are:

**Test cases:**
-> enter here test cases or at least the titles


The test cases with steps can be viewed here: [test_cases.pdf]()

## 1.5 Test Implementation

The following elements are needed to be ready before the test execution phase begins:

* enter here what needs to be ready for the test execution to begin

## 1.6 Test Execution

* Test cases are executed on the created test Cycle summary: [cycle_summary_execution.pdf]()
* Bugs have been created based on the failed tests. The complete bug reports can be found here: [created_bugs.pdf]()
    *  enter here bug titles


## 1.7 Test Completion

* Exit criteria was evaluated and passed
* The traceability matrix was generated and can be found here: [Traceability_matrix.csv]()
* Test execution chart was generated, the final report shows.... -> describe the final report

-> enter here test execution report/chart

# 2 SQL section
