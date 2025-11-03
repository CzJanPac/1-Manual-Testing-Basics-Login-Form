# Test Execution Log – Login Function

| Test ID | Test Name | Result | Notes | Executed By | Date |
|----------|------------|---------|--------|--------------|----------|
| TC_LOGIN_001 | Verify login page opens | ✅ Pass | Page loaded correctly | Jan Páč | 2025-11-04 |
| TC_LOGIN_002 | Successful login | ✅ Pass | Redirected to the Products page | Jan Páč | 2025-11-04 |
| TC_LOGIN_003 | Invalid credentials | ✅ Pass | Error message displayed correctly | Jan Páč | 2025-11-04 |
| TC_LOGIN_004 | Password masking | ✅ Pass | Asterisks shown instead of text | Jan Páč | 2025-11-04 |
| TC_LOGIN_005 | Logout | ✅ Pass | Redirected to the login page | Jan Páč | 2025-11-04 |
| TC_LOGIN_006 | Back button after logout | ✅ Pass | Access denied as expected | Jan Páč | 2025-11-04 |

### Summary
- **Total Tests:** 6  
- **Passed:** 6
- **Failed:** 0  
- **Blocked:** 0  
- **Pass Rate:** 100%

---

# *Simulation of several bugs for learning purposes*<br>Test Execution Log – Login Function

| Test ID | Test Name | Result | Notes | Executed By | Date |
|----------|------------|---------|--------|--------------|------|
| TC_LOGIN_001 | Verify login page opens | ✅ Pass | Page loaded correctly | Jan Páč | 2025-11-04 |
| TC_LOGIN_002 | Successful login | ✅ Pass | Redirected to the Products page | Jan Páč | 2025-11-04 |
| TC_LOGIN_003 | Invalid credentials | ❌ Fail | Error message not displayed for blank password | Jan Páč | 2025-11-04 |
| TC_LOGIN_004 | Password masking | ❌ Fail | Characters in password are visible | Jan Páč | 2025-11-04 |
| TC_LOGIN_005 | Logout | ❌ Fail | Clicking the Logout option does not respond | Jan Páč | 2025-11-04 |
| TC_LOGIN_006 | Back button after logout | ⚠️ Blocked | Blocked due to logout function failure |  |  |

### Summary
- **Total Tests:** 6  
- **Passed:** 2
- **Failed:** 3  
- **Blocked:** 1  
- **Pass Rate:** 33%
