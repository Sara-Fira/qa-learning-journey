# API Test Cases

## 1. Pet

| ID      | Test Scenario                          | Method | Endpoint                   | Expected Result                                                                 |
| ------- | -------------------------------------- | ------ | -------------------------- | ------------------------------------------------------------------------------- |
| PET-001 | Create a pet with valid data           | POST   | `/pet`                     | Status 200; the pet is created with the submitted data                          |
| PET-002 | Retrieve an existing pet by ID         | GET    | `/pet/{petId}`             | Status 200; the response contains the correct pet                               |
| PET-003 | Update an existing pet with valid data | PUT    | `/pet`                     | Status 200; the complete pet record is updated                                  |
| PET-004 | Update a pet using form data           | POST   | `/pet/{petId}`             | Status 200; the pet name and status are updated                                 |
| PET-005 | Retrieve pets by status                | GET    | `/pet/findByStatus`        | Status 200; the response contains an array of pets matching the selected status |
| PET-006 | Retrieve pets by tag                   | GET    | `/pet/findByTags`          | Status 200; the response contains an array of pets matching the selected tag    |
| PET-007 | Upload an image for an existing pet    | POST   | `/pet/{petId}/uploadImage` | Status 200; the image upload is accepted and upload information is returned     |
| PET-008 | Delete an existing pet                 | DELETE | `/pet/{petId}`             | Status 200; the pet is deleted successfully                                     |


## 2. Store

| ID | Test Scenario | Method | Endpoint | Expected Result |
|---|---|---|---|---|
| STORE-001 | Retrieve pet inventory | GET | `/store/inventory` | Status 200; the response contains pet status names and quantities |
| STORE-002 | Create an order with valid data | POST | `/store/order` | Status 200; the order is created with the submitted data |
| STORE-003 | Retrieve an existing order by ID | GET | `/store/order/{orderId}` | Status 200; the response contains the correct order |
| STORE-004 | Delete an existing order | DELETE | `/store/order/{orderId}` | Status 200; the order is deleted successfully |



## 3. User

| ID | Test Scenario | Method | Endpoint | Expected Result |
|---|---|---|---|---|
| USER-001 | Create a user with valid data | POST | `/user` | Status 200; the user is created successfully |
| USER-002 | Retrieve an existing user by username | GET | `/user/{username}` | Status 200; the response contains the correct user data |
| USER-003 | Update an existing user | PUT | `/user/{username}` | Status 200; the user data is updated successfully |
| USER-004 | Log in with valid credentials | GET | `/user/login` | Status 200; the login is successful and a session message is returned |
| USER-005 | Log out the current user | GET | `/user/logout` | Status 200; the user is logged out successfully |
| USER-006 | Create multiple users from a list | POST | `/user/createWithList` | Status 200; the user list is processed successfully |
| USER-007 | Delete an existing user | DELETE | `/user/{username}` | Status 200; the user is deleted successfully |
