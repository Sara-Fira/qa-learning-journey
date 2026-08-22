# Test Plan

## 1. Project Objective

The objective of this project is to verify the main functionality of the Swagger Petstore API using Postman.

The project covers all 19 documented API operations for the Pet, Store, and User resources. It includes positive and negative tests, dynamic test data, and end-to-end workflows.

## 2. Test Scope

### In Scope

* Pet, Store, and User API operations
* GET, POST, PUT, and DELETE requests
* Positive and selected negative scenarios
* Status code validation
* Response body and data type validation
* Response header validation
* Response time validation
* Environment and collection variables
* Dynamic test data
* End-to-end workflows
* Collection execution in Postman Collection Runner

### Out of Scope

* Performance and load testing
* Security and penetration testing
* Exhaustive testing of every possible data combination
* Swagger UI interface testing
* Source code testing
* Full OAuth testing

## 3. Test Approach

The tests will be designed based on the Swagger Petstore OpenAPI documentation.

Each API operation will have at least one positive test. Selected operations will also include negative scenarios, such as invalid identifiers, missing data, non-existing resources, or missing authorization.

The project will include the following workflows:

* Pet lifecycle: create, retrieve, update, upload an image, delete, and verify deletion
* Store lifecycle: create, retrieve, delete, and verify deletion of an order
* User lifecycle: create, log in, retrieve, update, log out, and delete a user

## 4. Test Environment

| Item              | Details                               |
| ----------------- | ------------------------------------- |
| API               | Swagger Petstore                      |
| Base URL          | `https://petstore3.swagger.io/api/v3` |
| API documentation | `https://petstore3.swagger.io/`       |
| Testing tool      | Postman                               |
| Execution tool    | Postman Collection Runner             |
| Repository        | GitHub                                |

## 5. Test Data

Dynamic and unique test data will be generated during collection execution.

Collection variables will be used to store values such as:

* Pet ID and pet name
* Order ID
* Username, password, and email address

Sensitive values and active credentials will not be published in the GitHub repository.

## 6. Entry Criteria

Testing can begin when:

* The API documentation is available
* The public API server is accessible
* The Postman collection and environment are configured

## 7. Exit Criteria

Testing will be completed when:

* All planned requests have been executed
* The end-to-end workflows have been completed
* Test results have been reviewed
* Failed tests and API issues have been documented
* The collection has been executed in Collection Runner
* The execution report has been prepared

## 8. Risks and Limitations

Swagger Petstore is a public and shared test environment. Test data may be modified or deleted by other users.

API responses may also differ from the documentation. Any observed differences will be documented in the Test Execution Report.

## 9. Test Deliverables

* Postman collection
* Postman environment without sensitive values
* Test cases
* Collection Runner evidence
* Test Execution Report
* Project README
