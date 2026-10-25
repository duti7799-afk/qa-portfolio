# BUG-12: Several accounts can be registered with the same mobile number (admin panel)

| Field | Value |
|---|---|
| **Project** | AI Shopping Assistant |
| **Priority** | High |
| **Environment** | Lenovo ThinkPad laptop · Windows 11 Pro (build 26200) · Google Chrome 148 |
| **Reproducibility** | 100% |

## Preconditions
A user is already registered with a specific mobile number.

## Steps to Reproduce
1. Open the admin panel registration form.
2. Fill in valid first name, last name, email and password.
3. Enter a mobile number that already belongs to another account.
4. Click “Sign up”.

## Expected Result
Registration fails; the phone number field is marked invalid with a message like “A user with this phone number already exists”.

## Actual Result
Registration succeeds and a new account is created with the duplicate phone number.

## Attachments
_Screenshots/videos are not included (confidential client material)._
