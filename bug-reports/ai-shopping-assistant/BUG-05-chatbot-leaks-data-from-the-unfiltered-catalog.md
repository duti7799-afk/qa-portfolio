# BUG-05: Chatbot leaks data from the unfiltered catalog instead of staying in the current filtered context

| Field | Value |
|---|---|
| **Project** | AI Shopping Assistant |
| **Priority** | High |
| **Environment** | Lenovo ThinkPad laptop · Windows 11 Pro (build 26200) · Google Chrome 147 |
| **Reproducibility** | 100% |

## Steps to Reproduce
1. Open the website and the chatbot.
2. Ask for a limited list, e.g. “Show me only the first 3 phones”.
3. Check that exactly 3 products are shown.
4. Reply to that message and ask about an item that is not in the view: “Tell me about the 4th phone”.
5. Observe the response.

## Expected Result
The bot stays inside the filtered results and says there is no 4th item in the current selection, or offers to expand the list.

## Actual Result
The bot returns details of a “4th phone” from the original unfiltered catalog, although only 3 phones are shown in the chat. It does not keep the context of the active filter.

## Notes
AI / LLM context-handling issue.

## Attachments
_Screenshots/videos are not included (confidential client material)._
