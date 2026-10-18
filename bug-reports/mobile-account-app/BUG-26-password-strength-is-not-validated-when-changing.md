# BUG-26: Password strength is not validated when changing the password

| Field | Value |
|---|---|
| **Project** | Mobile App — Account Settings |
| **Priority** | Urgent |
| **Environment** | Google Pixel 7 · Android 16 |
| **Reproducibility** | 100% |

## Preconditions
User is logged in.

## Steps to Reproduce
1. Open the app.
2. Go to Profile from the bottom navigation bar.
3. Open “Change password”.
4. Enter a password made only of digits (e.g. 1234567) and repeat it.
5. Tap SAVE.

## Expected Result
Passwords made only of digits or only of letters are rejected, with a message about password strength requirements.

## Actual Result
The password is changed without any warning about its strength.

## Notes
Security issue.

## Attachments
_Screenshots/videos are not included (confidential client material)._
