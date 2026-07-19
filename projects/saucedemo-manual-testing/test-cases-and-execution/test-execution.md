# Test Execution – SauceDemo

**Project:** SauceDemo
**Tester:** Sara Fira
**Execution type:** Manual testing

## Execution Summary

| Metric               | Result |
| -------------------- | -----: |
| Total test scenarios |     30 |
| Total test cases     |     56 |
| Executed test cases  |     56 |
| Passed               |     56 |
| Failed               |      0 |
| Blocked              |      0 |
| Not tested           |      0 |

---

## 1. Login Execution

| Scenario ID | Test Case ID | Test Case                               | Status | Actual Result                                                              |
| ----------- | ------------ | --------------------------------------- | ------ | -------------------------------------------------------------------------- |
| SC-LOG-001  | TC-LOG-001   | Verify login with valid credentials     | Passed | User logged in successfully and was redirected to the Products page.       |
| SC-LOG-002  | TC-LOG-002   | Verify login with invalid username      | Passed | Error message was displayed and user was not logged in.                    |
| SC-LOG-002  | TC-LOG-003   | Verify login with invalid password      | Passed | Error message was displayed and user was not logged in.                    |
| SC-LOG-003  | TC-LOG-004   | Verify login with empty username field  | Passed | Error message was displayed for missing username.                          |
| SC-LOG-003  | TC-LOG-005   | Verify login with empty password field  | Passed | Error message was displayed for missing password.                          |
| SC-LOG-003  | TC-LOG-006   | Verify login with both fields empty     | Passed | Error message was displayed and user was not logged in.                    |
| SC-LOG-004  | TC-LOG-007   | Verify login with locked out user       | Passed | Locked out user could not log in and relevant error message was displayed. |
| SC-LOG-002  | TC-LOG-008   | Verify error message after failed login | Passed | Error message was displayed correctly after failed login attempt.          |
| SC-LOG-002  | TC-LOG-009   | Verify error message can be closed      | Passed | Error message was closed after clicking the close icon.                    |
| SC-LOG-005  | TC-LOG-010   | Verify logout functionality             | Passed | User logged out successfully and was redirected to the login page.         |

---

## 2. Products Page Execution

| Scenario ID | Test Case ID | Test Case                                                    | Status | Actual Result                                                              |
| ----------- | ------------ | ------------------------------------------------------------ | ------ | -------------------------------------------------------------------------- |
| SC-PRD-001  | TC-PRD-001   | Verify products page loads after successful login            | Passed | Products page loaded successfully after login.                             |
| SC-PRD-002  | TC-PRD-002   | Verify product names are displayed correctly                 | Passed | Product names were visible and displayed correctly.                        |
| SC-PRD-002  | TC-PRD-003   | Verify product prices are displayed correctly                | Passed | Product prices were visible and displayed in the correct format.           |
| SC-PRD-002  | TC-PRD-004   | Verify product images are displayed correctly                | Passed | Product images were visible on the Products page.                          |
| SC-PRD-003  | TC-PRD-005   | Verify product details page opens correctly                  | Passed | Product details page opened after selecting a product.                     |
| SC-PRD-004  | TC-PRD-006   | Verify user can return from product details to products list | Passed | User returned successfully from product details page to the Products list. |
| SC-PRD-005  | TC-PRD-007   | Verify sorting by name A to Z                                | Passed | Products were sorted correctly by name from A to Z.                        |
| SC-PRD-005  | TC-PRD-008   | Verify sorting by name Z to A                                | Passed | Products were sorted correctly by name from Z to A.                        |
| SC-PRD-005  | TC-PRD-009   | Verify sorting by price low to high                          | Passed | Products were sorted correctly by price from low to high.                  |
| SC-PRD-005  | TC-PRD-010   | Verify sorting by price high to low                          | Passed | Products were sorted correctly by price from high to low.                  |

---

## 3. Cart Execution

| Scenario ID | Test Case ID | Test Case                                                 | Status | Actual Result                                                                  |
| ----------- | ------------ | --------------------------------------------------------- | ------ | ------------------------------------------------------------------------------ |
| SC-CART-001 | TC-CART-001  | Verify user can add one product to cart                   | Passed | One product was added to the cart successfully.                                |
| SC-CART-003 | TC-CART-002  | Verify cart badge updates after adding product            | Passed | Cart badge updated correctly after adding a product.                           |
| SC-CART-002 | TC-CART-003  | Verify user can add multiple products to cart             | Passed | Multiple products were added to the cart successfully.                         |
| SC-CART-004 | TC-CART-004  | Verify user can remove product from products page         | Passed | Product was removed from the Products page and cart badge updated correctly.   |
| SC-CART-004 | TC-CART-005  | Verify user can remove product from cart page             | Passed | Product was removed successfully from the cart page.                           |
| SC-CART-005 | TC-CART-006  | Verify cart page displays selected products correctly     | Passed | Cart page displayed selected products correctly.                               |
| SC-CART-005 | TC-CART-007  | Verify product name and price in cart match products page | Passed | Product name and price in the cart matched the Products page.                  |
| SC-CART-005 | TC-CART-008  | Verify user can continue shopping from cart               | Passed | User returned from cart to the Products page after clicking Continue Shopping. |
| SC-CART-005 | TC-CART-009  | Verify empty cart behavior                                | Passed | Empty cart was displayed correctly when no products were added.                |
| SC-CART-006 | TC-CART-010  | Verify cart content remains after page refresh            | Passed | Cart content remained visible after refreshing the page.                       |

---

## 4. Checkout Execution

| Scenario ID | Test Case ID | Test Case                                                        | Status | Actual Result                                                     |
| ----------- | ------------ | ---------------------------------------------------------------- | ------ | ----------------------------------------------------------------- |
| SC-CHK-001  | TC-CHK-001   | Verify checkout can be started from cart                         | Passed | Checkout can be started from cart.                                |
| SC-CHK-002  | TC-CHK-002   | Verify checkout form is displayed correctly                      | Passed | Checkout form is displayed correctly.                             |
| SC-CHK-002  | TC-CHK-003   | Verify checkout with valid first name, last name and postal code | Passed | Checkout is complete with valid credentials.                      |
| SC-CHK-002  | TC-CHK-004   | Verify checkout with empty first name                            | Passed | Error message was displayed correctly.                            |
| SC-CHK-002  | TC-CHK-005   | Verify checkout with empty last name                             | Passed | Error message was displayed correctly.                            |
| SC-CHK-002  | TC-CHK-006   | Verify checkout with empty postal code                           | Passed | Error message was displayed correctly.                            |
| SC-CHK-002  | TC-CHK-007   | Verify checkout error messages are displayed correctly           | Passed | Error messages are displayed correctly.                           |
| SC-CHK-002  | TC-CHK-008   | Verify checkout can be cancelled                                 | Passed | Checkout can be cancelled.                                        |
| SC-CHK-003  | TC-CHK-009   | Verify checkout overview displays correct products               | Passed | Checkout overview displays correct products.                      |
| SC-CHK-003  | TC-CHK-010   | Verify item total is calculated correctly                        | Passed | Item total is calculated correctly.                               |
| SC-CHK-003  | TC-CHK-011   | Verify tax is displayed                                          | Passed | Tax is displayed.                                                 |
| SC-CHK-003  | TC-CHK-012   | Verify final total is calculated correctly                       | Passed | Final total is calculated correctly.                              |
| SC-CHK-004  | TC-CHK-013   | Verify order can be completed successfully                       | Passed | Order completed successfully.                                     |
| SC-CHK-005  | TC-CHK-014   | Verify confirmation message after successful order               | Passed | Correct confirmation message is displayed after successful order. |

---

## 5. Navigation & Session Execution

| Scenario ID | Test Case ID | Test Case                                                                      | Status | Actual Result                                                                       |
| ----------- | ------------ | ------------------------------------------------------------------------------ | ------ | ----------------------------------------------------------------------------------- |
| SC-NAV-001  | TC-NAV-001   | Verify side menu opens correctly                                               | Passed | Side menu opens correctly.                                                          |
| SC-NAV-001  | TC-NAV-002   | Verify side menu closes correctly                                              | Passed | Side menu closes correctly.                                                         |
| SC-NAV-002  | TC-NAV-003   | Verify “All Items” link redirects to products page                             | Passed | “All Items” link redirects to products page.                                        |
| SC-NAV-002  | TC-NAV-004   | Verify “About” link redirects correctly                                        | Passed | “About” link redirects correctly.                                                   |
| SC-NAV-003  | TC-NAV-005   | Verify logout redirects user to login page                                     | Passed | Logout redirects user to login page.                                                |
| SC-NAV-004  | TC-NAV-006   | Verify user cannot access products page after logout using browser back button | Passed | User could not access the Products page after logout using the browser back button. |

---

## 6. Usability Execution

| Scenario ID | Test Case ID | Test Case                                             | Status | Actual Result                                   |
| ----------- | ------------ | ----------------------------------------------------- | ------ | ----------------------------------------------- |
| SC-USB-001  | TC-USB-001   | Verify main elements are aligned correctly on desktop | Passed | Main elements are aligned correctly on desktop. |
| SC-USB-002  | TC-USB-002   | Verify buttons are visible and readable               | Passed | Buttons are visible and readable.               |
| SC-USB-003  | TC-USB-003   | Verify error messages are clear and understandable    | Passed | Error messages are clear and understandable.    |
| SC-USB-004  | TC-USB-004   | Verify form fields are labeled correctly              | Passed | Form fields are labeled correctly.              |
| SC-USB-005  | TC-USB-005   | Verify layout remains usable on smaller browser width | Passed | Layout remains usable on smaller browser width. |
| SC-USB-005  | TC-USB-006   | Verify important actions are easy to identify         | Passed | Important actions are easy to identify.         |
