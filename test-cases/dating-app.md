# Test Cases — Dating Mobile App

Total: 4

| ID | Title | Type | Priority | Related |
|---|---|---|---|---|
| [TC-031](#tc-031) | Header respects the status bar / safe area on all screens | UI / Mobile | High | [BUG-21](../bug-reports/dating-app/BUG-21-header-elements-overlap-the-status-bar-safe.md) |
| [TC-032](#tc-032) | Search preferences persist after force-close | Functional / Mobile | Medium | [BUG-22](../bug-reports/dating-app/BUG-22-search-preferences-age-range-and-gender-reset.md) |
| [TC-033](#tc-033) | Search preferences persist after logout / login | Functional / Mobile | Medium | [BUG-22](../bug-reports/dating-app/BUG-22-search-preferences-age-range-and-gender-reset.md) |
| [TC-034](#tc-034) | Verified face photo cannot be deleted if it is the only one | Business rule | High | [REC-19](../recommendations/dating-app/REC-19-prevent-deleting-the-only-verified-face-photo.md) |

## TC-031

**Title:** Header respects the status bar / safe area on all screens  
**Type:** UI / Mobile · **Priority:** High · **Related:** [BUG-21](../bug-reports/dating-app/BUG-21-header-elements-overlap-the-status-bar-safe.md)

**Preconditions:** Phone with a notch / punch-hole camera

**Steps:**
1. Open Home, Profile, Chats and Settings.

**Expected result:** Header elements are fully visible and tappable on every screen.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-032

**Title:** Search preferences persist after force-close  
**Type:** Functional / Mobile · **Priority:** Medium · **Related:** [BUG-22](../bug-reports/dating-app/BUG-22-search-preferences-age-range-and-gender-reset.md)

**Preconditions:** —

**Steps:**
1. Set gender and age range 18–25 and confirm.
2. Force-close the app.
3. Reopen and check the preferences.

**Expected result:** Saved values are still selected.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-033

**Title:** Search preferences persist after logout / login  
**Type:** Functional / Mobile · **Priority:** Medium · **Related:** [BUG-22](../bug-reports/dating-app/BUG-22-search-preferences-age-range-and-gender-reset.md)

**Preconditions:** —

**Steps:**
1. Set preferences.
2. Log out and log in again.

**Expected result:** Saved values are still selected (or match the spec).

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-034

**Title:** Verified face photo cannot be deleted if it is the only one  
**Type:** Business rule · **Priority:** High · **Related:** [REC-19](../recommendations/dating-app/REC-19-prevent-deleting-the-only-verified-face-photo.md)

**Preconditions:** Profile is verified with one face photo

**Steps:**
1. Go to Edit Profile.
2. Try to delete the verified photo.

**Expected result:** Deletion is blocked with an explanation, or the profile is hidden until re-verification.

**Actual result:** _to be filled during execution_  
**Status:** Not run
