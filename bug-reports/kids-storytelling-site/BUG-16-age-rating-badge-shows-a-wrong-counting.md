# BUG-16: Age rating badge shows a wrong counting animation (1+ → 3+) on page load

| Field | Value |
|---|---|
| **Project** | Kids' Interactive Storytelling Website |
| **Priority** | High |
| **Environment** | Lenovo ThinkPad laptop · Windows 11 Pro (build 26200) · Google Chrome 149 |
| **Reproducibility** | 90% |

## Preconditions
User is on the “News” page and refreshes it.

## Steps to Reproduce
1. Open the website.
2. Hover over “News” in the header menu.
3. Select “Latest news” from the dropdown.

## Expected Result
The age rating badge always shows “3+”, without extra animation or wrong intermediate values.

## Actual Result
While the page loads, the badge shows a counter animation that starts at 1+ and stops at 3+.

## Attachments
_Screenshots/videos are not included (confidential client material)._
