# OrangeHRM Manual Testing – Test Plan

## Project Information

Test Plan ID: OHRM-TP-001

Version: 1.0

Date: 9 August 2026

Tester: Sara Fira

Project Type: Personal Manual QA Portfolio Project

## Objective

The goal of this project is to manually test selected OrangeHRM Demo features and practise a complete QA workflow using TestRail, Jira, and GitHub.

This is a personal learning project and does not represent commercial experience.

## Application Under Test

Application: OrangeHRM Demo

Version: OrangeHRM OS 5.9

URL: https://opensource-demo.orangehrmlive.com/

The application is a public demo, so its data may be changed by other users.

## Scope

The following areas are included:

* Authentication
* PIM – Employee List
* PIM – Add Employee
* PIM – Personal Details
* Admin – User Management
* My Info – Personal Details
* Admin and ESS access control
* Employee and ESS account end-to-end flows
* One exploratory testing session

## Out of Scope

The following areas are not included:

* Leave
* Time
* Recruitment
* Performance
* Dashboard
* Directory
* Maintenance
* Claim
* Buzz
* API testing
* Performance testing
* Mobile testing
* Cross-browser testing
* Full security testing

## Test Approach

Testing will be performed manually.

The project includes:

* Positive and negative testing
* Equivalence Partitioning
* Selected boundary checks
* State transition testing
* Role-based testing
* End-to-end testing
* Exploratory testing

There is no formal SRS for this project. Test cases are based on information displayed in the application, observed behaviour, and reasonable testing assumptions.

The test suite contains 40 scripted test cases and one exploratory testing charter.

## Test Environment

Operating System: Windows 10

Browser: Google Chrome

Test Management: TestRail

Defect Management: Jira Cloud

Repository: GitHub

## Test Data

Unique employee records and ESS accounts will be created during execution.

Only records created for this project will be modified or deleted. Records belonging to other demo users will not be intentionally changed.

Test passwords will not be published on GitHub.

## Entry Criteria

Testing can begin when:

* OrangeHRM Demo is available.
* Test cases are prepared and reviewed.
* The TestRail Test Run is active.
* Jira is configured and connected with TestRail.
* Admin credentials are available.

## Exit Criteria

The testing cycle can finish when:

* All 40 scripted test cases have a result.
* Blocked tests are explained.
* Confirmed defects are reported in Jira.
* The exploratory session is completed.
* A Test Summary Report is prepared.
* Final evidence is exported from TestRail and Jira.

## Test Results

Passed – The actual behaviour matches the Expected Result.

Failed – The actual behaviour does not match the Expected Result.

Blocked – The test cannot be completed because of an external issue or missing test data.

Retest – The test needs to be executed again.

Untested – The test has not been executed yet.

## Defect Management

Confirmed defects will be reported in Jira.

When a defect is connected with a test case, traceability will be maintained:

TestRail Test Case → Test Run Result → Jira Defect

No artificial defects will be created for this portfolio project.

## Main Risks

| Risk                                 | Action                                          |
| ------------------------------------ | ----------------------------------------------- |
| Demo data is changed by another user | Use unique test data and check preconditions    |
| OrangeHRM Demo is unavailable        | Mark affected tests as Blocked and retry later  |
| No formal requirements are available | Separate observations and assumptions           |
| TestRail trial expires               | Export test cases and results before expiration |

## Deliverables

* Test Plan
* TestRail test case export
* Test execution results
* Jira defect reports
* Exploratory testing notes
* Test Summary Report
* GitHub documentation

## Schedule

| Activity                            | Planned Date             |
| ----------------------------------- | ------------------------ |
| Project setup and test design       | 8–9 August 2026          |
| Test execution and defect reporting | 9–23 August 2026         |
| Exploratory testing                 | After scripted execution |
| Final report and GitHub update      | By 23 August 2026        |

## Version History

| Version | Date          | Description       |
| ------- | ------------- | ----------------- |
| 1.0     | 9 August 2026 | Initial Test Plan |

