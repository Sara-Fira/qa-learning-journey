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
