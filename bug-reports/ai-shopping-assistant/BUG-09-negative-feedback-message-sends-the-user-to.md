# BUG-09: Negative feedback message sends the user to an operator without asking for confirmation

| Field | Value |
|---|---|
| **Project** | AI Shopping Assistant |
| **Priority** | High |
| **Environment** | Lenovo ThinkPad laptop · Windows 11 Pro (build 26200) · Google Chrome 149 |
| **Reproducibility** | 100% |

## Steps to Reproduce
1. Open the website and the chatbot.
2. Send a normal query (e.g. “Help me choose a laptop”).
3. Send a negative feedback phrase (e.g. “You are answering incorrectly”).

## Expected Result
The bot continues the conversation, acknowledges the feedback and asks what went wrong.

## Actual Result
The bot immediately hands the user over to an operator with no confirmation, and the AI conversation ends. During working hours it shows “Your request has been sent to an operator”; outside working hours a modal says no operator is available.

## Attachments
_Screenshots/videos are not included (confidential client material)._
