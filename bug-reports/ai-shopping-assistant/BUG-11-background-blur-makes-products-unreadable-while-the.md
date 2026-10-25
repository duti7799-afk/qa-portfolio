# BUG-11: Background blur makes products unreadable while the chat is open, even after resizing the chat

| Field | Value |
|---|---|
| **Project** | AI Shopping Assistant |
| **Priority** | Normal |
| **Environment** | Lenovo ThinkPad laptop · Windows 11 Pro (build 26200) · Google Chrome 147 |
| **Reproducibility** | 100% |

## Steps to Reproduce
1. Open the website and search for a product (e.g. “phone”).
2. Open the chat window.
3. Make the chat window smaller by dragging its edge.
4. Look at the page content behind it.

## Expected Result
The chat works as a non-modal element: product information stays readable and interactive during the chat.

## Actual Result
Opening the chat applies a global blur and makes the background non-interactive. Resizing does not remove the blur, so products stay unreadable.

## Attachments
_Screenshots/videos are not included (confidential client material)._
