# BUG-04: Operator status indicator shows green (online) during non-working hours

| Field | Value |
|---|---|
| **Project** | AI Shopping Assistant |
| **Priority** | High |
| **Environment** | Lenovo ThinkPad laptop · Windows 11 Pro (build 26200) · Google Chrome 148 |
| **Reproducibility** | 100% |

## Preconditions
Customer tries to contact an operator through the chatbot during non-working hours.

## Steps to Reproduce
1. Open the website and the chatbot.
2. Send a message to the AI to start the chat.
3. Request a human operator.
4. Close the popup saying the operator is currently unavailable.
5. Look at the status indicator next to the operator’s profile.

## Expected Result
The indicator is grey or red, matching the operator’s real offline status.

## Actual Result
The indicator is green (online/available), while the system at the same time shows a notice that it is outside working hours.

## Attachments
_Screenshots/videos are not included (confidential client material)._
