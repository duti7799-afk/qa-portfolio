# BUG-10: Chatbot cannot find the nearest store by landmark or area name

| Field | Value |
|---|---|
| **Project** | AI Shopping Assistant |
| **Priority** | Normal |
| **Environment** | Lenovo ThinkPad laptop · Windows 11 Pro (build 26200) · Google Chrome 147 |
| **Reproducibility** | 100% |

## Steps to Reproduce
1. Open the website and the chatbot.
2. Ask for a branch near a landmark, e.g. “Where is the nearest branch to Station Square?”
3. Observe the response.

## Expected Result
The bot uses location data, recognises the area and returns the nearest branch address.

## Actual Result
The bot gives a generic answer that exact addresses near that area are not available and only says the retailer has 16+ stores in Georgia.

## Attachments
_Screenshots/videos are not included (confidential client material)._
