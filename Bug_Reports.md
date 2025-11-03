# Bug Reports – Login Function


## BUG_LOGIN_001 – Error Message Not Displayed for Blank Password
**Related Test Case:** TC_LOGIN_003  
**Severity:** Medium  
**Priority:** High  
**Status:** Open  
**Reported By:** Jan Páč  
**Date:** 2025-11-04  

**Environment:**  
- Website: https://www.saucedemo.com  
- Browser: Google Chrome (latest)  
- OS: Windows 11  

**Preconditions:**  
n/a

**Steps to Reproduce:**  
1. Open the login page: https://www.saucedemo.com.  
2. Enter a valid username (`standard_user`).  
3. Leave the password field blank.  
4. Click the **Login** button.  

**Expected Result:**  
The error message *“Epic sadface: Password is required”* should be displayed.  

**Actual Result:**  
No error message appears after clicking the Login button.  

**Evidence:**  
Screencast_Login_NoError.mpg


## BUG_LOGIN_002 – Password Characters Are Visible
**Related Test Case:** TC_LOGIN_004  
**Severity:** High  
**Priority:** Medium  
**Status:** Open  
**Reported By:** Jan Páč  
**Date:** 2025-11-04  

**Environment:**  
- Website: https://www.saucedemo.com  
- Browser: Google Chrome (latest)  
- OS: Windows 11  

**Preconditions:**  
n/a

**Steps to Reproduce:**  
1. Open the login page: https://www.saucedemo.com. 
2. Click in the Password field.  
3. Type any password.  

**Expected Result:**  
Password characters should be masked (displayed as dots or asterisks).  

**Actual Result:**  
Password characters are visible as plain text.  

**Evidence:**  
Screenshot_PasswordVisible.png  


## BUG_LOGIN_003 – Logout Option Does Not Respond
**Related Test Case:** TC_LOGIN_005  
**Severity:** High  
**Priority:** High  
**Status:** Open  
**Reported By:** Jan Páč  
**Date:** 2025-11-04  

**Environment:**  
- Website: https://www.saucedemo.com  
- Browser: Google Chrome (latest)  
- OS: Windows 11  

**Preconditions:**  
User is logged in with valid credentials.

**Steps to Reproduce:**  
1. Click the menu button in the top left corner.  
2. Click on **Logout**.  

**Expected Result:**  
User should be logged out and redirected to the login page.  

**Actual Result:**  
Clicking the Logout option does not respond. User remains on the same page.  

**Evidence:**  
Screencast_LogoutNotWorking.mpg  

