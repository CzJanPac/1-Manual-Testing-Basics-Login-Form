# Test Plan – Login Function

## 1. Introduction
This document describes the testing approach for the login feature and defines how the login will be tested and which techniques will be used.

## 2. Objectives
- Ensure that the login functionality with valid and invalid credentials works correctly.
- Verify that an error message is shown after using invalid credentials.
- Confirm correct redirection after login with valid credentials.
- Ensure that the user is completely signed out after logging out.

## 3. Test Scope
### In Scope
- Functional testing of login page (positive and negative)
- Error message validation
- Redirect and logout verification

### Out of Scope
- Backend database validation
- API testing
- UI design testing

## 4. Test Approach
- Manual functional testing
- Black-box testing techniques
- Equivalence Partitioning
- Boundary Value Analysis
- Exploratory Testing

## 5. Test Environment
| Component | Description |
|------------|--------------|
| Website | https://www.saucedemo.com |
| Browser | Google Chrome (latest) |
| OS | Windows 11 |
| Network | Stable internet connection |

## 6. Test Data
| Data Type | Example | Purpose |
|------------|----------|----------|
| Valid credentials | standard_user / secret_sauce | Positive login test |
| Invalid credentials | invalid_user / wrong_pass | Negative test |
| Empty fields | "" / "" | Validation test |

## 7. Roles & Responsibilities
| Role | Responsibility |
|------|----------------|
| Tester (Jan Páč) | Execute test cases, report bugs, document results |
| Test Lead | Review documentation and provide feedback |

## 8. Entry & Exit Criteria
| Criteria | Description |
|-----------|-------------|
| Entry | The test environment and data are ready; the login page is online and accessible |
| Exit | All test cases have been executed, all bugs reported, and results documented |

## 9. Risks & Mitigation
| Risk | Mitigation |
|------|-------------|
| Unstable internet connection | Work on test documentation offline and run tests later |
| Unexpected website downtime | Reschedule testing |
| Missing test data | Prepare backup test accounts |

## 10. Deliverables
- Feature Analysis
- Test Plan (this document)  
- Test Cases  
- Bug Reports
- Final Test Summary

## 11. Schedule
| Phase | Status | Estimated Date |
|--------|----------------|--------|
| Feature Analysis | ✅ Completed | 31/10/2025 |
| Test Plan | ✅ Completed | 01/11/2025 |
| Test Cases | 🚧 In Progress | 02–03/11/2025 |
| Bug Reports | ⏳ Planned | 04/11/2025 |
| Final Report | ⏳ Planned | 05/11/2025 |
