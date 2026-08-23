# Test Execution Report

## 1. Execution Overview

| Item                  | Details                      |
| --------------------- | ---------------------------- |
| Project               | Swagger Petstore API Testing |
| Execution date        | 23 August 2026               |
| Environment           | Swagger Petstore - Local     |
| Tool                  | Postman Collection Runner    |
| Iterations            | 1                            |
| Duration              | 8.138 s                      |
| Average response time | 158 ms                       |

## 2. Execution Results

| Result              | Count |
| ------------------- | ----: |
| Assertions executed |    36 |
| Passed              |     7 |
| Failed              |    29 |
| Script errors       |     0 |

Evidence: [`initial-collection-run-results.png`](../evidence/initial-collection-run-results.png)

## 3. Result Analysis

The Postman collection and test scripts were executed successfully, with no script errors.

Most failed assertions were caused by the public API returning status `500 Internal Server Error`. The initial failure of resource creation requests also caused dependent workflow requests to fail.

For example, when the Pet creation request returned status 500, later requests could not retrieve or update the expected Pet. As a result, response properties such as `id`, `name`, and `status` were undefined.

The image upload request was tested successfully during manual execution. It failed in Collection Runner because the selected binary file was stored locally and was not available to the Runner.

## 4. Observed Issues

| ID      | Observation                                           | Expected Result                                               | Actual Result                              |
| ------- | ----------------------------------------------------- | ------------------------------------------------------------- | ------------------------------------------ |
| OBS-001 | Upload image response schema mismatch                 | ApiResponse containing `code`, `type`, and `message`          | Full Pet object returned                   |
| OBS-002 | Valid Store requests fail                             | Successful responses according to the documentation           | Store endpoints return status 500          |
| OBS-003 | Multiple valid User requests fail                     | Successful resource creation, retrieval, update, and deletion | User endpoints return status 500           |
| OBS-004 | Login accepts invalid credentials                     | Status 400 for invalid credentials                            | Status 200 and a user session are returned |
| OBS-005 | Missing required Pet fields are not handled correctly | Status 400 or 422                                             | Status 500                                 |

## 5. Excluded or Blocked Requests

The following requests were not executed because their required test resources were not successfully created:

* DELETE Order
* DELETE Pet without Authorization

The image upload request will be excluded from future shared Runner executions because it requires a local binary file. Its result was verified manually.

## 6. Limitations

Swagger Petstore is a public and shared test environment. Its data and availability may be affected by other users or temporary server issues.

Failures caused by unavailable resources or server errors do not indicate JavaScript or Postman script errors.

## 7. Conclusion

The collection successfully demonstrated request configuration, environment and collection variables, dynamic test data, positive and negative API testing, response validation, and end-to-end workflow design.

The execution identified several differences between the OpenAPI documentation and the actual API behavior. A second Collection Runner execution may be performed when the public API is stable.
