# BUG-08: Chatbot returns the wrong product when a catalog item is selected by ordinal (“the third one”)

| Field | Value |
|---|---|
| **Project** | AI Shopping Assistant |
| **Priority** | High |
| **Environment** | Google Pixel 7 · Android 16 · Google Chrome 148 |
| **Reproducibility** | 100% |

## Steps to Reproduce
1. Open the website and the chatbot.
2. Send “Help me choose a laptop” (in Georgian).
3. When the catalog appears, send “third” as a normal message (without Reply).
4. Observe the response.
5. Now reply directly to the catalog message and type “third”.

## Expected Result
The bot resolves “third” to the third item of the returned catalog and shows its correct details, whatever the input method.

## Actual Result
In both cases the bot fails to identify the right product and returns details of an unrelated item.

## Notes
AI / LLM context-handling issue.

## Attachments
_Screenshots/videos are not included (confidential client material)._
