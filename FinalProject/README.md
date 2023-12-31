# Final project for ITF Manual Testing Course

The scope of the final project for ITF Manual Testing Course is to use all gained knowledge throught the course and apply them in practice, using a live application. 

Application under test: www.houzz.com

**The final project will be split into 2 sections: [Testing section](https://github.com/magthalena02/manual_testing_portofolio/edit/main/FinalProject/README.md) and [SQL section](https://github.com/julai215/itf_final_project_example_and_portofolio/blob/main/Final%20Project/README.md#2-sql-section).**

Tools used: Jira Software, Zephyr Squad.

# Functional specifications

- Story GM-1: Create account for new user on www.houzz.com ![Story GM-1](https://github.com/magthalena02/manual_testing_portofolio/assets/130222530/5c3836e6-f709-4aa3-be21-c426f5512bf2)

- Story GM-5: Search bar implementation for www.houzz.com ![Story GM-5](https://github.com/magthalena02/manual_testing_portofolio/assets/130222530/d26286ae-d764-474e-b7d1-0ac80fd0f304)

- Story GM-9: Create an ideabook as a user on www.houzz.com ![Story GM-9](https://github.com/magthalena02/manual_testing_portofolio/assets/130222530/5a102553-e7f4-41ef-9150-4d1168dee2f9)


# 1 Testing section

## 1.1 Test Planning

The Test Plan is designed to describe details of testing for the User Account module from the www.houzz.com application. 

The plan identifies the items to be tested, the features to be tested, the types of testing to be performed, the personnel responsible for testing, the resources and schedule required to complete testing, and the risks associated with the plan

#### 1.1.1 Roles assigned to the project and persons allocated

- **Test Lead John Smith:** Responsible for overall test planning and execution
- **Test Engineer Michael Jones:** Responsible for developing test cases and scripts, and executing tests
- **Developer Dave Hatt:** Responsible for fixing defects and providing support during testing
- **Server administrator Kevin Brown:** Responsible for maintaining the test environment

#### 1.1.2 Entry criteria defined

- The test environment, including staging servers or environments that closely mimic production, must be set up and configured to reflect the production environment accurately.
- Test data, including realistic user profiles, sample content, and any required databases, should be available and populated in the test environment.
- Test cases, test plans, and any other testing documentation must be created, reviewed, and approved.
- All necessary testing tools and infrastructure, such as test management tools, automation frameworks, and devices for compatibility testing, must be in place and ready for use.
- Ensure that test data handling complies with data privacy regulations, and sensitive or personal information is anonymized or masked as necessary.
- Review and confirm that the documented requirements, user stories, and acceptance criteria are clear, complete, and agreed upon by stakeholders.
  
#### 1.1.3 Exit criteria defined

- Ensure that all the test cases must be executed and passed
- Verify that there are no critical defects (severity level high)
- Confirm that all the test deliverables must be completed and submitted.
- Performance test should pass the threshold limit.
  
#### 1.1.4 Test scope

##### Tests in scope:
- Ensure that the users can create new account using a valid email address and they choose strong and secure passwords during account creation.
- Users should receive appropiate error message when attempting to create account with invalid email address or incorrect paswword and they can access their profiles with newly created account.
- Confirm that users can enter search queries in the search bar and the results are displayed based on input.
- Using filters by categories or other relevant criteria refine search results and the user receive search suggestions useful as they type in the search bar.
- The registered users can create ideabooks to save and organize design ideas and projects.
- Items added are correctly associated with the users's ideabook and any change made is saved and is reflected in the user account.
  
##### Tests not in scope:
- Testing of authentication methods such as social media login (Google, Facebook), password recovery or account reset functionality is not in scope for this plan.
- In-depth testing of the search algorithm's accuracy and relevance ranking is not within the scope.
- Performance testing for scenarios involving an exceptionally large number of ideabooks or projects is not covered here.
- Testing of ideabook integration with other functionalities (e.g. purchasing items, sharing ideabooks) is not part of this scope.

#### 1.1.5 Risks detected

##### Project risks:
- The testing plan may be affected if there are unresolved technical dependencies with other components or services (e.g., third-party authentication providers) that are necessary for account creation.
- Delays in delivery and task completion for new implementations by testing team. 
- Cost-cutting across organization, which could lead to reduced funds and resources needed to improve the project.
- Poor definition of the business requirements can lead to misinterpretations.
- Frequent changes or updates to the website's codebase may lead to regression testing challenges, making it difficult to maintain test suites.

##### Product risks:
- The potential risk of data breaches or unauthorized access to user account information or ideabook data could harm the reputation and trustworthiness of the website.
- Poor usability and a subpar user experience can result in frustrated users who may abandon the website. This risk could impact user retention and engagement.
- Performance issues, such as slow page load times or unresponsive search functionality, can lead to user dissatisfaction and abandonment.
- Incompatibility with different browsers and devices can result in a poor user experience and reduced website accessibility.
- Integration issues with third-party services or external search engines may disrupt the seamless operation of the website's search functionality.
- Weak password management or inadequate security measures may expose user accounts to hacking attempts.
- Data migration from legacy systems to the new website may lead to data loss, inaccuracies, or inconsistencies.
- As user traffic increases, there may be performance scalability issues with account creation or search functionality, leading to slow response times or system failures.

#### 1.1.6 Evaluating entry criteria

The entry criteria defined in the Test Planning phase have been achieved and the test process can continue. 

## 1.2 Test Monitoring and Control

It will be done by generating periodic reports that reflect the current status of the test.
![Test metrics_daily test_project](https://github.com/magthalena02/manual_testing_portofolio/assets/130222530/5dd7c344-c3fb-4959-9b91-324e758cbb36)

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
- GM-2 Successfully create account with valid data on www.houzz.com
- GM-4 Create account with invalid data on www.houzz.com
- GM-6 Create ideabook with success on www.houzz.com
- GM-8 Successfull login with created account on www.houzz.com
- GM-10 Failed login with created account on www.houzz.com
- GM-12 Unsuccessfully create account with invalid password on www.houzz.com
- GM-13 Unsuccessfully create account with invalid email on www.houzz.com
- GM-14 Search "Dining Table" product in search bar of www.houzz.com
- GM-15 Check status of "Create" button for creating new ideabook on www.houzz.com
- GM-16 Clear history for search bar on www.houzz.com

The test cases with steps can be viewed here: [Test cases with steps_ZFJ-issue-export.xlsx](https://github.com/magthalena02/manual_testing_portofolio/files/12872272/Test.cases.with.steps_ZFJ-issue-export.xlsx)

## 1.5 Test Implementation

The following elements are needed to be ready before the test execution phase begins:

- Test Manager ensure delivery of test environment and test data at this stage
- Constrains, risks and priorities of the project are prepared.
- Test team is complete and is ready for execution.
- Entry criteria is ready.

## 1.6 Test Execution

* Test cases are executed on the created test Cycle summary: ![Cycle Summary of the project](https://github.com/magthalena02/manual_testing_portofolio/assets/130222530/87742cc5-6522-4953-846b-529f9e0c44df)

* Bugs have been created based on the failed tests. The complete bug reports can be found here [BUG ticket Report.pdf](https://github.com/magthalena02/manual_testing_portofolio/files/12872368/BUG.ticket.Report.pdf):

    *  GM-3 Error message still displayed after deleting invalid email address and wrong password when signing up on www.houzz.com 
    *  GM-11 Error message still displayed after deleting invalid email address when signing up on www.houzz.com

## 1.7 Test Completion

* Exit criteria was evaluated and passed.
* The traceability matrix was generated and can be found here [Forward Traceability.xlsx](https://github.com/magthalena02/manual_testing_portofolio/files/12872421/Forward.Traceability.xlsx):
  ![Forward Traceability](https://github.com/magthalena02/manual_testing_portofolio/assets/130222530/d4ef5504-08dd-46fe-85a8-bd9c30da34b0)

* Test execution chart was generated, the final report shows that the homepage loaded successfully and all elements were functional, meeting the requirements. New account was created using an valid email address and an invalid one for negative testing confirming that the account creation process functioned as expected. Error messages persisted after deleting invalid email address or password during sing-up and login, which was not in line with the expected behavior. The search bar provided accurate search results and suggestions meeting the acceptance criteria. The process of creating an ideabook worked as intended and it was saved without issues.<p>
  <p>Regarding this conclusions, we recommend to investigate and resolve the persistence of error messages during the sign-up and login processes to improve user satisfaction. Defects discovered during testing have been logged into the defect tracking system for further investigation and resolution.
  <p>This test completion report provides an overview of the quality of www.houzz.com based on the testing of 10 critical test cases. The identified issues need to be addressed to enhance the overall user experience and website functionality.<p>

    Project Report can be find here: [Zephyr Test Steps + Executions + Results (Jira) .pdf](https://github.com/magthalena02/manual_testing_portofolio/files/12873917/Zephyr.Test.Steps.%2B.Executions.%2B.Results.Jira.pdf)<br>
    Test execution chart: ![Test execution chart](https://github.com/magthalena02/manual_testing_portofolio/assets/130222530/a2222bb5-c05e-4c2f-a118-9c98354d396a)




