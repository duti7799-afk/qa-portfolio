# BUG-23: Microphone shows as unmuted but no audio is broadcast during a debate session

| Field | Value |
|---|---|
| **Project** | Online Debate App |
| **Priority** | High |
| **Environment** | Staging · Google Pixel 7 · Android 17 |
| **Reproducibility** | 70% |

## Preconditions
User is logged in and is in an active debate session.

## Steps to Reproduce
1. Wait for your turn to speak.
2. Make sure the microphone is unmuted.
3. Start speaking.
4. Check whether other participants receive the audio.

## Expected Result
Audio is transmitted continuously to the other participants during the speech.

## Actual Result
Other participants hear nothing, although the microphone is on and the unmuted icon is shown.

## Attachments
_Screenshots/videos are not included (confidential client material)._
