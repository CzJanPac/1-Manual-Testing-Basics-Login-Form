# Feature Analysis – Login Function

## 1. Purpose
The goal of this test is to verify the function of the login form in website https://www.saucedemo.com/ with functional positive and negative tests. 

## 2. Test Scope
### In Scope
two input form fields - Username and Password
error messages
successfully redirect after submit login
button Login
frontend

### Out of Scope
- Backend and API
- Visual and UI

## 3. Identified Risks
| Risk | Impact | Probability | Notes |
|------|--------|--------------|-------|
| Nonvalid input in form fields | High | High | Can make system crash or security problem |
| Missing error messages | Medium | High | User can be confused |
| Incorrect redirect | Medium | Low | User cant use application or product |
| Login button dont submit form | High | Medium | Function of login form be broke |
| Many clicks of Login button | High | Low | Can cause system crash |

## 4. Test Objectives
Positive test of login form fields
Negative test of login form fields
Verify the error message is shown after negative test
Redirecting after submit positive login
Verify the user remain logged in 
After log out the user must be logged out

## 5. Assumptions
- Browser: Chrome (latest)  
- OS: Windows 11  
- Test account: standard_user / secret_sauce

