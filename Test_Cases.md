# Test Cases – Login Function

## Test Case 1 – Positive - Verify Login Page Opens Successfully

| Field | Description |
|--------|-------------|
| **Test ID** | TC_LOGIN_001 |
| **Title** | Verify that the login page is displayed correctly when accessed via URL |
| **Preconditions** | None |
| **Test Steps** | 1. Open the URL [SauceDemo](https://www.saucedemo.com) |
| **Expected Result** | The login page is loaded successfully. <br> Username and Password fields, Login button, and page logo are visible. |
| **Priority** | High |
| **Status** | Not executed |


## Test Case 2 – Positive - Successful Login
| Field | Description |
|--------|-------------|
| **Test ID** | TC_LOGIN_002 |
| **Title** | Verify that a user can log in with valid credentials |
| **Preconditions** | Login page is open; User has a valid account (username: standard_user / password: secret_sauce) |
| **Test Steps** | 1. Enter valid username<br>2. Enter valid password<br>3. Click the Login button |
| **Expected Result** | User is successfully redirected to the Products page |
| **Priority** | High |
| **Status** | Not executed |


## Test Case 3 – Negative - Invalid Credentials
| Field | Description |
|--------|-------------|
| **Test ID** | TC_LOGIN_003 |
| **Title** | Verify that login fails with invalid credentials and an error message is shown |
| **Preconditions** | Login page is open |
| **Test Steps** | 1. Enter Username and Password as per the Test Data table below.<br>2. Click the Login button |
| **Expected Result** | The login attempt must fail. <br>No redirect to the inventory page.<br>The correct error message is displayed according to the input (see Test Data table) |
| **Priority** | High |
| **Status** | Not executed |

### Test Data – Invalid Credentials

| ID | Username | Password | Expected Result | Notes |
|----|-----------|-----------|-----------------|--------|
| 1 | *(blank)* | *(blank)* | **Error:** "Epic sadface: Username is required" | Both fields empty |
| 2 | `standard_user` | *(blank)* | **Error:** "Epic sadface: Password is required" | Missing password |
| 3 | *(blank)* | `secret_sauce` | **Error:** "Epic sadface: Username is required" | Missing username |
| 4 | `invalid_user` | `secret_sauce` | **Error:** "Epic sadface: Username and password do not match any user in this service" | Wrong username |
| 5 | `standard_user` | `wrong_password` | **Error:** "Epic sadface: Username and password do not match any user in this service" | Wrong password |
| 6 | `locked_out_user` | `secret_sauce` | **Error:** "Epic sadface: Sorry, this user has been locked out." | Blocked account |
| 7 | `standard_user` | `/*-+%` | **Error:** "Epic sadface: Username and password do not match any user in this service" | Special characters in password |
| 8 | `/*-+%` | `secret_sauce` | **Error:** "Epic sadface: Username and password do not match any user in this service" | Special characters in username |
| 9 | `aaa... (64 chars)` | `secret_sauce` | **Error:** "Epic sadface: Username and password do not match any user in this service" | 64-char username |
| 10 | `standard_user` | `aaa... (64 chars)` | **Error:** "Epic sadface: Username and password do not match any user in this service" | 64-char password |
| 11 | `user123` | `secret_sauce` | **Error:** "Epic sadface: Username and password do not match any user in this service" | Username contains digits |
| 12 | `standard_user` | `pass123` | **Error:** "Epic sadface: Username and password do not match any user in this service" | Password contains digits |
| 13 | `ˇ=/*-+` | `ˇ=/*-+` | **Error:** "Epic sadface: Username and password do not match any user in this service" | Both fields special characters |
| 14 | `performance_glitch_user` | `wrong_pass` | **Error:** "Epic sadface: Username and password do not match any user in this service" | Valid user, wrong password |
| 15 | `invalid_user` | *(blank)* | **Error:** "Epic sadface: Password is required" | Missing password, invalid username |


## Test Case 4 – Positive - Password Field Masking
| Field | Description |
|--------|-------------|
| **Test ID** | TC_LOGIN_004 |
| **Title** | Verify that the password field masks the characters entered |
| **Preconditions** | Login page is open |
| **Test Steps** | 1. Enter any password into the password field |
| **Expected Result** | Password characters are displayed as dots or asterisks |
| **Priority** | Low |
| **Status** | Not executed |


## Test Case 5 – Positive - Logout Functionality
| Field | Description |
|--------|-------------|
| **Test ID** | TC_LOGIN_005 |
| **Title** | Verify that a user can log out successfully |
| **Preconditions** | User is logged in with valid credentials |
| **Test Steps** | 1. Click the menu button<br>2. Click the Logout option |
| **Expected Result** | User is redirected back to the login page |
| **Priority** | High |
| **Status** | Not executed |

## Test Case 6 – Negative - Click On Back Button After Logout
| Field | Description |
|--------|-------------|
| **Test ID** | TC_LOGIN_006 |
| **Title** | Verify that using the browser Back button after logout does not restore access to the user page |
| **Preconditions** | User is logged in with valid credentials |
| **Test Steps** | 1. Click the menu button<br>2. Click the Logout option<br>3. Click the browser’s Back button |
| **Expected Result** | Error message "Epic sadface: You can only access '/inventory.html' when you are logged in." is shown and access is denied. |
| **Priority** | High |
| **Status** | Not executed |
