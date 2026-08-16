# OrangeHRM Manual Testing Project - Test Summary Report

**Report date:** 16 August 2026  
**Application under test:** OrangeHRM Open Source Demo  
**Testing type:** Manual functional and exploratory testing  
**Environment:** Google Chrome on Windows 10  
**Tools:** TestRail, Jira Cloud, GitHub

## 1. Executive Summary

The planned OrangeHRM manual testing scope was completed. The functional test run finished with all 40 test cases passed and 5 confirmed defects. A separate 45-minute exploratory session was also completed. Five defects were documented in Jira for defect-management practice.


## 2. Scope

The project covered:

- Authentication
- PIM Employee List
- PIM Add Employee
- PIM Personal Details
- Admin User Management
- ESS My Info
- Role-based access control
- Employee and ESS account end-to-end workflows
- Exploratory testing of validation, permissions, data consistency, session behaviour, and usability

## 3. Execution Results

| Test run | Executed | Passed | Failed | Blocked | Untested | Completion |
|---|---:|---:|---:|---:|---:|---:|
| Functional Test Run | 40 | 35 | 5 | 0 | 0 | 88% |
| Exploratory Test Run | 1 | 1 | 0 | 0 | 0 | 100% |
| **Total** | **41** | **35** | **5** | **0** | **0** | **94%** |

The exploratory test status indicates that the defined mission and six goals were completed within the 45-minute timebox.

## 4. Defect Summary

### Confirmed defects

| Jira key | Simulated issue | Severity | Priority |
|---|---|---|---|
| OHRM-1 | No validation message after selecting an unsupported profile picture format | Low | Medium |
| OHRM-2 | Invalid Date of Birth can be saved in Personal Details | Medium | High |
| OHRM-3 | Personal Details updated in My Info are not synchronized with PIM | High | High |
| OHRM-4 | ESS user can access User Management through a direct URL | Critical | Highest |
| OHRM-5 | Disabled ESS account can still be used to log in | Critical | Highest |

All five simulated Jira issues were linked to the exploratory test result in TestRail.

## 5. Test Evidence and Deliverables

The following evidence was produced:

- Baseline test-case export in PDF and CSV
- Final functional run export in PDF and CSV
- Final exploratory run export in PDF and CSV
- Five Jira defect reports linked to TestRail
- This Test Summary Report

## 6. Risks and Limitations

- Testing was performed against a public demo environment that may reset or change test data.
- The scope focused on selected business-critical workflows and did not cover every OrangeHRM module.
- Cross-browser, mobile, accessibility, performance, API, database, and automated testing were outside the scope.

## 7. Exit Criteria

The project exit criteria were met:

- All 40 planned functional test cases were executed.
- 88% functional cases passed.
- The exploratory mission and all six goals were completed.
- Test results and evidence were recorded.

## 8. Conclusion

The tested OrangeHRM workflows were stable within the defined scope. Functional execution achieved a 88% pass rate with 5 confirmed defects. The project demonstrates manual test design, structured execution, negative testing, role-based testing, exploratory testing, evidence collection, TestRail-Jira traceability, and defect-reporting practice.

**Final assessment:** Testing completed successfully. The tested scope meets the defined acceptance and exit criteria.

