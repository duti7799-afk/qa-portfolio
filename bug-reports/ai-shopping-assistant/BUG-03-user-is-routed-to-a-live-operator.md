# BUG-03: User is routed to a live operator outside working hours when the shift end time is later than 17:00

| Field | Value |
|---|---|
| **Project** | AI Shopping Assistant |
| **Priority** | High |
| **Environment** | Lenovo ThinkPad laptop · Windows 11 Pro (build 26200) · Google Chrome 148 |
| **Reproducibility** | 100% |

## Preconditions
Working hours are set to 09:00–19:00 in the admin panel. The current time is outside working hours (22:29).

## Steps to Reproduce
1. Open the website.
2. Open the chatbot and start a conversation.
3. Tap the “Operator” button in the bottom-right corner of the chat window.
4. Wait for the response.

## Expected Result
Regardless of the configured end time, operator routing is blocked outside working hours and an “Off-hours” message is shown.

## Actual Result
The user is routed to a live operator outside working hours.

## Notes
Boundary finding: the issue happens only when the shift end time is later than 17:00. With an end time of exactly 17:00, routing is correctly blocked after hours.

## Attachments
_Screenshots/videos are not included (confidential client material)._
