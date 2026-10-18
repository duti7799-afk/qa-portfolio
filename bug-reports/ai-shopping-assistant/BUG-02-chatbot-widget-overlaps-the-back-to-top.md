# BUG-02: Chatbot widget overlaps the “Back to Top” button at the bottom of the page

| Field | Value |
|---|---|
| **Project** | AI Shopping Assistant |
| **Priority** | High |
| **Environment** | Lenovo ThinkPad laptop · Windows 11 Pro (build 26200) · Google Chrome 147 |
| **Reproducibility** | 100% |

## Steps to Reproduce
1. Open the website.
2. Search for any product (e.g. “phone”).
3. Scroll to the very end of the search results.
4. Look at the bottom-right corner where the “Back to Top” button is located.

## Expected Result
The “Back to Top” button is clearly visible and clickable; there is enough spacing between the chatbot widget and the navigation buttons.

## Actual Result
The chatbot icon sits directly on top of the “Back to Top” button. Because there is no footer to add padding, the button is almost completely hidden and hard to click.

## Attachments
_Screenshots/videos are not included (confidential client material)._
