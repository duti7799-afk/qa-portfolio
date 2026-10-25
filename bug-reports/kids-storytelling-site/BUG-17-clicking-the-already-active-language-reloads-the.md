# BUG-17: Clicking the already active language reloads the page and causes a 404 console error

| Field | Value |
|---|---|
| **Project** | Kids' Interactive Storytelling Website |
| **Priority** | High |
| **Environment** | Lenovo ThinkPad laptop · Windows 11 Pro (build 26200) · Google Chrome 149 |
| **Reproducibility** | 100% |

## Preconditions
The site interface is in Georgian.

## Steps to Reproduce
1. Open the website.
2. Open DevTools (F12) → Console.
3. Click the “GE” language button.

## Expected Result
Clicking the active language does nothing: no reload and no console errors.

## Actual Result
The page reloads and a 404 error appears in the console.

## Attachments
_Screenshots/videos are not included (confidential client material)._
