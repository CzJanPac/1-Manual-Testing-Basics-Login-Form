# Feature Analysis – Login Function

## 1. Purpose
The goal of this test is to verify the functionality of the login form on the website https://www.saucedemo.com through both positive and negative functional tests.
Login is a basic function because the user needs access to their profile.

## 2. Test Scope
### In Scope
- Two input fields: Username and Password.
- Error messages for invalid inputs.
- Successful redirect after a valid login.
- Login button functionality.
- Frontend behavior only.

### Out of Scope
- Backend and API.
- Visual and UI.

## 3. Identified Risks
| Risk | Impact | Probability | Notes |
|------|--------|--------------|-------|
| Invalid input in form fields | High | High | May cause a system error or security vulnerability |
| Missing error messages | Medium | High | Users may become confused |
| Incorrect redirect | Medium | Low | User can’t access the application correctly |
| Login button does not submit the form | High | Low | Login functionality is broken |
| Repeated clicking of the Login button | High | Low | Multiple clicks on the Login button may cause performance issues or duplicate requests |
| Weak password from a security point of view | High | Medium | May cause unauthorized access to the account |

## 4. Test Objectives
- Verify positive login with valid credentials.  
- Verify negative login with invalid credentials or empty fields.  
- Ensure error messages appear for failed login attempts.  
- Confirm that users are redirected correctly after successful login.  
- Verify that the user remains logged in after navigation.  
- Ensure that after logout the user is completely signed out.

## 5. Assumptions
- Browser: Chrome (latest)  
- OS: Windows 11
- Test account: standard_user / secret_sauce
- Test user credentials are valid and active
- Internet connection is stable and the website is accessible
- The browser cache is cleared before testing

