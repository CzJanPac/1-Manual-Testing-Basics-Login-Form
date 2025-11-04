# 🔗 Requirements Traceability Matrix – Login Function

**Project:** SauceDemo – Login Function  
**Tester:** Jan Páč  
**Date:** 2025-11-04  


## 🧩 Real Test Execution (All Passed)

| Requirement ID | Requirement Description | Test Case ID(s) | Bug ID(s) | Status |
|----------------|--------------------------|-----------------|------------|---------|
| REQ_LOGIN_001 | User can open the login page successfully | TC_LOGIN_001 | - | ✅ Tested |
| REQ_LOGIN_002 | User can log in with valid credentials | TC_LOGIN_002 | - | ✅ Tested |
| REQ_LOGIN_003 | System validates incorrect credentials and displays an error message | TC_LOGIN_003 | - | ✅ Tested |
| REQ_LOGIN_004 | Password input is masked while typing | TC_LOGIN_004 | - | ✅ Tested |
| REQ_LOGIN_005 | User can log out successfully | TC_LOGIN_005 | - | ✅ Tested |
| REQ_LOGIN_006 | User cannot access private pages after logout | TC_LOGIN_006 | - | ✅ Tested |


## 🧪 Simulated Bug Scenario (For Training Purposes)

| Requirement ID | Requirement Description | Test Case ID(s) | Bug ID(s) | Status |
|----------------|--------------------------|-----------------|------------|---------|
| REQ_LOGIN_001 | User can open the login page successfully | TC_LOGIN_001 | - | ✅ Tested |
| REQ_LOGIN_002 | User can log in with valid credentials | TC_LOGIN_002 | - | ✅ Tested |
| REQ_LOGIN_003 | System validates incorrect credentials and displays an error message | TC_LOGIN_003 | BUG_LOGIN_001 | ❌ Failed |
| REQ_LOGIN_004 | Password input is masked while typing | TC_LOGIN_004 | BUG_LOGIN_002 | ❌ Failed |
| REQ_LOGIN_005 | User can log out successfully | TC_LOGIN_005 | BUG_LOGIN_003 | ❌ Failed |
| REQ_LOGIN_006 | User cannot access private pages after logout | TC_LOGIN_006 | - | ⚠️ Blocked |


### Legend
| Symbol | Meaning |
|---------|----------|
| ✅ | Tested and passed |
| ❌ | Test failed (bug reported) |
| ⚠️ | Test blocked – not executable |


### Notes
- All tests were executed manually based on the defined Test Cases.  
- The **first table** represents actual execution results (all passed).  
- The **second table** shows *simulated defects* used for demonstration and learning purposes.  


✅ **Prepared by:** Jan Páč  
🗓️ **Date:** 2025-11-04  
