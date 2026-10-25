# BUG-22: Search preferences (age range and gender) reset after the app is force-closed

| Field | Value |
|---|---|
| **Project** | Dating Mobile App |
| **Priority** | High |
| **Environment** | Production · Google Pixel 7 · Android 16 · app v2.0.2 |
| **Reproducibility** | 100% |

## Preconditions
User is logged in.

## Steps to Reproduce
1. Open the app and open the preferences on the home screen.
2. Choose the partner’s gender and age range (e.g. 18–25).
3. Confirm.
4. Force-close the app from recent apps.
5. Open the app again and check the search preferences.

## Expected Result
The selected filters are saved and kept after the app is closed.

## Actual Result
The saved preferences are lost and reset to the default values.

## Attachments
_Screenshots/videos are not included (confidential client material)._
