# BUG-07: “Reply” on an item in an older catalog uses the context of the latest search results

| Field | Value |
|---|---|
| **Project** | AI Shopping Assistant |
| **Priority** | High |
| **Environment** | Google Pixel 7 · Android 16 · Chrome 148  /  Lenovo ThinkPad · Windows 11 Pro · Chrome 148 |
| **Reproducibility** | 100% on both devices |

## Steps to Reproduce
1. Open the website and the chatbot.
2. Search for a first product (e.g. “phone”) and wait for the catalog.
3. Search for a second product (e.g. “iPad”) and wait for the new catalog.
4. Click “Reply” on any item in the latest catalog.
5. Scroll up to the first (“phone”) catalog.
6. Click “Reply” on any item there (e.g. the first phone).
7. Observe the response.

## Expected Result
The bot identifies the selected item from the first catalog and answers about that product, regardless of later searches.

## Actual Result
The bot processes the selection using the most recent catalog (“iPad”) and answers about a product from the last search.

## Notes
AI / LLM context-handling issue.

## Attachments
_Screenshots/videos are not included (confidential client material)._
