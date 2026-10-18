# BUG-21: Header elements overlap the status bar / safe area on every screen

| Field | Value |
|---|---|
| **Project** | Dating Mobile App |
| **Priority** | Normal |
| **Environment** | Production · Google Pixel 7 · Android 16 · app v2.0.2 |
| **Reproducibility** | 100% |

## Preconditions
User is logged in.

## Steps to Reproduce
1. Open the app.
2. Use the bottom navigation to open different screens (home, profile, etc.).
3. Look at the top of each screen.

## Expected Result
The header respects the device safe area and status bar; all elements have proper top padding and are fully visible and tappable.

## Actual Result
On all screens the header is rendered at the very top edge and covers the status bar, so buttons and titles are partly cut off and cannot be tapped.

## Attachments
_Screenshots/videos are not included (confidential client material)._
