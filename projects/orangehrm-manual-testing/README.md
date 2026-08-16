# OrangeHRM Manual Testing

## Project Status

**Completed – Test planning, test design, functional execution, exploratory testing, defect reporting, and final reporting completed.**

## Project Overview

This is a personal Manual QA portfolio project based on the OrangeHRM Open Source Demo application.

The project demonstrates:

- Manual test planning and test design
- Positive and negative testing
- Functional test execution
- Role-based and end-to-end testing
- Exploratory testing
- Defect reporting in Jira
- TestRail and Jira traceability
- Test evidence collection
- Test summary reporting

The project does not represent commercial work experience.

Five defects were found and registered in Jira.

## Application Under Test

- **Application:** OrangeHRM Open Source Demo
- **Version:** OrangeHRM OS 5.9
- **URL:** [https://opensource-demo.orangehrmlive.com/](https://opensource-demo.orangehrmlive.com/)

## Scope

The project covers selected functionality from:

- Authentication
- PIM – Employee List
- PIM – Add Employee
- PIM – Personal Details
- Admin – User Management
- My Info – Personal Details
- Role-based access control
- Employee and ESS account end-to-end workflows
- Exploratory testing of validation, permissions, data consistency, session behaviour, and usability

## Out of Scope

The following areas were excluded:

- Leave
- Time
- Recruitment
- Performance
- Dashboard
- Directory
- Maintenance
- Claim
- Buzz
- Reports and advanced configuration
- API testing
- Performance testing
- Mobile testing
- Full security testing
- Cross-browser testing
- Automated testing

## Test Approach

The project used requirements-based and exploratory testing.

Since no formal Software Requirements Specification was available, the test cases were based on:

- Observed application behaviour
- Information available in the user interface
- Common expectations for employee-management systems
- Clearly identified testing assumptions

The test design included:

- Positive and negative testing
- Equivalence Partitioning
- Selected boundary and validation checks
- State-transition scenarios
- Role-based testing
- End-to-end workflows
- Error guessing
- Exploratory testing

## Tools

- OrangeHRM Open Source Demo
- TestRail
- Jira Cloud
- Google Chrome
- GitHub

## Test Execution Results

### Functional Test Run

| Metric               | Result |
| -------------------- | -----: |
| Planned              |     40 |
| Executed             |     40 |
| Passed               |     35 |
| Failed               |      5 |
| Blocked              |      0 |
| Untested             |      0 |
| Execution completion |   100% |
| Pass rate            |    88% |

### Exploratory Test Run

| Metric               |     Result |
| -------------------- | ---------: |
| Exploratory sessions |          1 |
| Session timebox      | 45 minutes |
| Mission status       |  Completed |
| Goals covered        |        6/6 |
| TestRail status      |     Passed |
| Linked Jira defects  |          5 |

## Defect Summary

Five defects were documented in Jira and linked to TestRail:

| Jira key | Defect                                                                      | Severity | Priority |
| -------- | --------------------------------------------------------------------------- | -------- | -------- |
| OHRM-1   | No validation message after selecting an unsupported profile picture format | Low      | Medium   |
| OHRM-2   | Invalid Date of Birth can be saved in Personal Details                      | Medium   | High     |
| OHRM-3   | Personal Details updated in My Info are not synchronized with PIM           | High     | High     |
| OHRM-4   | ESS user can access User Management through a direct URL                    | Critical | Highest  |
| OHRM-5   | Disabled ESS account can still be used to log in                            | Critical | Highest  |

## Project Deliverables

### Test Cases

- [Test Case Baseline – PDF](test-cases/orangehrm_test_cases_baseline_v1.0.pdf)
- [Test Case Baseline – CSV](test-cases/orangehrm_test_cases_baseline_v1.0.csv)

### Functional Test Results

- [Functional Test Run – PDF](test-results/orangehrm_functional_test_run_final_20260816.pdf)
- [Functional Test Run – CSV](test-results/orangehrm_functional_test_run_final_20260816.csv)

### Exploratory Testing

- [Exploratory Test Run – PDF](exploratory-testing/orangehrm_exploratory_test_run_final_20260816.pdf)
- [Exploratory Test Run – CSV](exploratory-testing/orangehrm_exploratory_test_run_final_20260816.csv)

### Defect Reports

- [Jira Defect Export – CSV](bug-reports/orangehrm_simulated_defects_20260816.csv)

### Test Summary

- [Test Summary Report – PDF](test-summary/orangehrm_test_summary_report_final_20260816.pdf)

## Selected Test Evidence

### Application Evidence

- Employee and enabled ESS account creation
- Required-field validation
- Password mismatch validation
- Duplicate username validation
- Oversized profile picture validation
- User Management required-field validation

Evidence is available in:

[`screenshots`](screenshots/application)

### TestRail Evidence

Test execution, exploratory testing, and milestone evidence is available in:

[`screenshots`](screenshots/testrail)

### Jira Evidence

Selected Jira defect-management evidence is available in:

[`screenshots`](screenshots/jira)

## Repository Structure

```text
orangehrm-manual-testing/
├── bug-reports/
├── exploratory-testing/
├── screenshots/
├── test-cases/
├── test-plan/
├── test-results/
├── test-summary/
└── README.md
```

## Risks and Limitations

- Testing was performed against a public demo environment that may reset or change test data.
- The project covered selected workflows rather than every OrangeHRM module.
- Cross-browser, mobile, accessibility, performance, API, database, and automated testing were outside the scope.

## Exit Criteria

The project exit criteria were met:

- All 40 planned functional test cases were executed.
- Functional execution reached 100% completion.
- The exploratory mission and all six goals were completed.
- Test evidence and final exports were prepared.
- Jira defects were linked to the exploratory TestRail result.
- The Test Summary Report was completed.
- The TestRail runs and milestone were closed.

## Conclusion

The OrangeHRM Manual Testing Project was completed successfully.

The project demonstrates a complete manual QA workflow, including planning, test design, execution, exploratory testing, defect reporting, evidence collection, TestRail–Jira traceability, and final reporting.
