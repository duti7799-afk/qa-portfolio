# Test Cases — HR / Recruitment Platform

Total: 3

| ID | Title | Type | Priority | Related |
|---|---|---|---|---|
| [TC-037](#tc-037) | Registration with an already registered email shows an error | Negative / Validation | Medium | [BUG-24](../bug-reports/hr-platform/BUG-24-no-error-message-when-registering-with-an.md) |
| [TC-038](#tc-038) | Candidate credentials cannot log in to the company portal | Security / Access control | High | [BUG-25](../bug-reports/hr-platform/BUG-25-candidate-credentials-log-the-user-in-to.md) |
| [TC-039](#tc-039) | Company credentials cannot log in to the candidate portal | Security / Access control | High | [BUG-25](../bug-reports/hr-platform/BUG-25-candidate-credentials-log-the-user-in-to.md) |

## TC-037

**Title:** Registration with an already registered email shows an error  
**Type:** Negative / Validation · **Priority:** Medium · **Related:** [BUG-24](../bug-reports/hr-platform/BUG-24-no-error-message-when-registering-with-an.md)

**Preconditions:** Email E is already registered

**Steps:**
1. Open Registration.
2. Fill the form with email E.
3. Click “Create candidate account”.

**Expected result:** Clear message: “This email is already registered”.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-038

**Title:** Candidate credentials cannot log in to the company portal  
**Type:** Security / Access control · **Priority:** High · **Related:** [BUG-25](../bug-reports/hr-platform/BUG-25-candidate-credentials-log-the-user-in-to.md)

**Preconditions:** User registered only as a candidate

**Steps:**
1. Choose “Log in as company”.
2. Enter the candidate’s credentials.

**Expected result:** Login is rejected with a suitable message.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-039

**Title:** Company credentials cannot log in to the candidate portal  
**Type:** Security / Access control · **Priority:** High · **Related:** [BUG-25](../bug-reports/hr-platform/BUG-25-candidate-credentials-log-the-user-in-to.md)

**Preconditions:** User registered only as a company

**Steps:**
1. Choose “Log in as candidate”.
2. Enter the company’s credentials.

**Expected result:** Login is rejected with a suitable message.

**Actual result:** _to be filled during execution_  
**Status:** Not run
