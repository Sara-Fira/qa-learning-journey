# Test Execution – SauceDemo

**Project:** SauceDemo
**Tester:** Sara Fira
**Execution type:** Manual testing

## Execution Summary

| Metric               | Result |
| -------------------- | -----: |
| Total test scenarios |     30 |
| Total test cases     |     56 |
| Executed test cases  |        |
| Passed               |        |
| Failed               |        |
| Blocked              |        |
| Not tested           |        |

---

## 1. Login Execution

| Scenario ID | Test Case ID | Test Case                               | Status | Notes |
| ----------- | ------------ | --------------------------------------- | ------ | ----- |
| SC-LOG-001  | TC-LOG-001   | Verify login with valid credentials     |        |       |
| SC-LOG-002  | TC-LOG-002   | Verify login with invalid username      |        |       |
| SC-LOG-002  | TC-LOG-003   | Verify login with invalid password      |        |       |
| SC-LOG-003  | TC-LOG-004   | Verify login with empty username field  |        |       |
| SC-LOG-003  | TC-LOG-005   | Verify login with empty password field  |        |       |
| SC-LOG-003  | TC-LOG-006   | Verify login with both fields empty     |        |       |
| SC-LOG-004  | TC-LOG-007   | Verify login with locked out user       |        |       |
| SC-LOG-002  | TC-LOG-008   | Verify error message after failed login |        |       |
| SC-LOG-002  | TC-LOG-009   | Verify error message can be closed      |        |       |
| SC-LOG-005  | TC-LOG-010   | Verify logout functionality             |        |       |

---

## 2. Products Page Execution

| Scenario ID | Test Case ID | Test Case                                                    | Status | Notes |
| ----------- | ------------ | ------------------------------------------------------------ | ------ | ----- |
| SC-PRD-001  | TC-PRD-001   | Verify products page loads after successful login            |        |       |
| SC-PRD-002  | TC-PRD-002   | Verify product names are displayed correctly                 |        |       |
| SC-PRD-002  | TC-PRD-003   | Verify product prices are displayed correctly                |        |       |
| SC-PRD-002  | TC-PRD-004   | Verify product images are displayed correctly                |        |       |
| SC-PRD-003  | TC-PRD-005   | Verify product details page opens correctly                  |        |       |
| SC-PRD-004  | TC-PRD-006   | Verify user can return from product details to products list |        |       |
| SC-PRD-005  | TC-PRD-007   | Verify sorting by name A to Z                                |        |       |
| SC-PRD-005  | TC-PRD-008   | Verify sorting by name Z to A                                |        |       |
| SC-PRD-005  | TC-PRD-009   | Verify sorting by price low to high                          |        |       |
| SC-PRD-005  | TC-PRD-010   | Verify sorting by price high to low                          |        |       |

---

## 3. Cart Execution

| Scenario ID | Test Case ID | Test Case                                                 | Status | Notes |
| ----------- | ------------ | --------------------------------------------------------- | ------ | ----- |
| SC-CART-001 | TC-CART-001  | Verify user can add one product to cart                   |        |       |
| SC-CART-003 | TC-CART-002  | Verify cart badge updates after adding product            |        |       |
| SC-CART-002 | TC-CART-003  | Verify user can add multiple products to cart             |        |       |
| SC-CART-004 | TC-CART-004  | Verify user can remove product from products page         |        |       |
| SC-CART-004 | TC-CART-005  | Verify user can remove product from cart page             |        |       |
| SC-CART-005 | TC-CART-006  | Verify cart page displays selected products correctly     |        |       |
| SC-CART-005 | TC-CART-007  | Verify product name and price in cart match products page |        |       |
| SC-CART-005 | TC-CART-008  | Verify user can continue shopping from cart               |        |       |
| SC-CART-005 | TC-CART-009  | Verify empty cart behavior                                |        |       |
| SC-CART-006 | TC-CART-010  | Verify cart content remains after page refresh            |        |       |

---

## 4. Checkout Execution

| Scenario ID | Test Case ID | Test Case                                                        | Status | Notes |
| ----------- | ------------ | ---------------------------------------------------------------- | ------ | ----- |
| SC-CHK-001  | TC-CHK-001   | Verify checkout can be started from cart                         |        |       |
| SC-CHK-002  | TC-CHK-002   | Verify checkout form is displayed correctly                      |        |       |
| SC-CHK-002  | TC-CHK-003   | Verify checkout with valid first name, last name and postal code |        |       |
| SC-CHK-002  | TC-CHK-004   | Verify checkout with empty first name                            |        |       |
| SC-CHK-002  | TC-CHK-005   | Verify checkout with empty last name                             |        |       |
| SC-CHK-002  | TC-CHK-006   | Verify checkout with empty postal code                           |        |       |
| SC-CHK-002  | TC-CHK-007   | Verify checkout error messages are displayed correctly           |        |       |
| SC-CHK-002  | TC-CHK-008   | Verify checkout can be cancelled                                 |        |       |
| SC-CHK-003  | TC-CHK-009   | Verify checkout overview displays correct products               |        |       |
| SC-CHK-003  | TC-CHK-010   | Verify item total is calculated correctly                        |        |       |
| SC-CHK-003  | TC-CHK-011   | Verify tax is displayed                                          |        |       |
| SC-CHK-003  | TC-CHK-012   | Verify final total is calculated correctly                       |        |       |
| SC-CHK-004  | TC-CHK-013   | Verify order can be completed successfully                       |        |       |
| SC-CHK-005  | TC-CHK-014   | Verify confirmation message after successful order               |        |       |

---

## 5. Navigation & Session Execution

| Scenario ID | Test Case ID | Test Case                                                                      | Status | Notes |
| ----------- | ------------ | ------------------------------------------------------------------------------ | ------ | ----- |
| SC-NAV-001  | TC-NAV-001   | Verify side menu opens correctly                                               |        |       |
| SC-NAV-001  | TC-NAV-002   | Verify side menu closes correctly                                              |        |       |
| SC-NAV-002  | TC-NAV-003   | Verify “All Items” link redirects to products page                             |        |       |
| SC-NAV-002  | TC-NAV-004   | Verify “About” link redirects correctly                                        |        |       |
| SC-NAV-003  | TC-NAV-005   | Verify logout redirects user to login page                                     |        |       |
| SC-NAV-004  | TC-NAV-006   | Verify user cannot access products page after logout using browser back button |        |       |

---

## 6. Usability Execution

| Scenario ID | Test Case ID | Test Case                                             | Status | Notes |
| ----------- | ------------ | ----------------------------------------------------- | ------ | ----- |
| SC-USB-001  | TC-USB-001   | Verify main elements are aligned correctly on desktop |        |       |
| SC-USB-002  | TC-USB-002   | Verify buttons are visible and readable               |        |       |
| SC-USB-003  | TC-USB-003   | Verify error messages are clear and understandable    |        |       |
| SC-USB-004  | TC-USB-004   | Verify form fields are labeled correctly              |        |       |
| SC-USB-005  | TC-USB-005   | Verify layout remains usable on smaller browser width |        |       |
| SC-USB-005  | TC-USB-006   | Verify important actions are easy to identify         |        |       |
