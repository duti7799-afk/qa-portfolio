# Test Cases — Mobile App — Account Settings

Total: 3

| ID | Title | Type | Priority | Related |
|---|---|---|---|---|
| [TC-040](#tc-040) | Weak passwords are rejected on password change | Security / Negative | High | [BUG-26](../bug-reports/mobile-account-app/BUG-26-password-strength-is-not-validated-when-changing.md) |
| [TC-041](#tc-041) | Strong password is accepted on password change | Positive | High | [BUG-26](../bug-reports/mobile-account-app/BUG-26-password-strength-is-not-validated-when-changing.md) |
| [TC-042](#tc-042) | Mismatched password confirmation is rejected | Negative | Medium | [BUG-26](../bug-reports/mobile-account-app/BUG-26-password-strength-is-not-validated-when-changing.md) |

## TC-040

**Title:** Weak passwords are rejected on password change  
**Type:** Security / Negative · **Priority:** High · **Related:** [BUG-26](../bug-reports/mobile-account-app/BUG-26-password-strength-is-not-validated-when-changing.md)

**Preconditions:** User is logged in

**Steps:**
1. Profile → Change password.
2. Try “1234567”, “abcdefg”, “abc12”.

**Expected result:** Each is rejected with a password-strength message.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-041

**Title:** Strong password is accepted on password change  
**Type:** Positive · **Priority:** High · **Related:** [BUG-26](../bug-reports/mobile-account-app/BUG-26-password-strength-is-not-validated-when-changing.md)

**Preconditions:** User is logged in

**Steps:**
1. Profile → Change password.
2. Enter a password with letters, digits and a symbol (8+ chars) twice.
3. Tap SAVE.

**Expected result:** Password is changed; user can log in with the new password.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-042

**Title:** Mismatched password confirmation is rejected  
**Type:** Negative · **Priority:** Medium · **Related:** [BUG-26](../bug-reports/mobile-account-app/BUG-26-password-strength-is-not-validated-when-changing.md)

**Preconditions:** User is logged in

**Steps:**
1. Enter different values in the two password fields.
2. Tap SAVE.

**Expected result:** Error: passwords do not match; nothing is saved.

**Actual result:** _to be filled during execution_  
**Status:** Not run
