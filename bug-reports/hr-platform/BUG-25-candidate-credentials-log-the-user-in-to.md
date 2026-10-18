# BUG-25: Candidate credentials log the user in to the Company portal without a company registration

| Field | Value |
|---|---|
| **Project** | HR / Recruitment Platform |
| **Priority** | High |
| **Environment** | Lenovo laptop · Windows 11 Pro (build 26100) · Google Chrome 141 |
| **Reproducibility** | 100% |

## Preconditions
User is registered only as a candidate.

## Steps to Reproduce
1. Open the website and choose “Log in”.
2. Click “Log in as company”.
3. Enter the candidate’s email and password.
4. Click “Log in”.

## Expected Result
Login is rejected because the user has no company account.

## Actual Result
The candidate is logged in to the company side with the same credentials.

## Notes
Access-control / role separation issue.

## Attachments
_Screenshots/videos are not included (confidential client material)._
