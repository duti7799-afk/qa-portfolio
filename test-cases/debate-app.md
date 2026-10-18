# Test Cases — Online Debate App

Total: 2

| ID | Title | Type | Priority | Related |
|---|---|---|---|---|
| [TC-035](#tc-035) | Audio is transmitted when the microphone is unmuted | Functional / Mobile | High | [BUG-23](../bug-reports/debate-app/BUG-23-microphone-shows-as-unmuted-but-no-audio.md) |
| [TC-036](#tc-036) | Microphone icon state matches the real audio state | Functional / Mobile | High | [BUG-23](../bug-reports/debate-app/BUG-23-microphone-shows-as-unmuted-but-no-audio.md) |

## TC-035

**Title:** Audio is transmitted when the microphone is unmuted  
**Type:** Functional / Mobile · **Priority:** High · **Related:** [BUG-23](../bug-reports/debate-app/BUG-23-microphone-shows-as-unmuted-but-no-audio.md)

**Preconditions:** Two devices in the same debate session

**Steps:**
1. On device A, wait for your turn and unmute.
2. Speak for 60 seconds.
3. Listen on device B.

**Expected result:** Device B hears device A without interruption for the whole turn.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-036

**Title:** Microphone icon state matches the real audio state  
**Type:** Functional / Mobile · **Priority:** High · **Related:** [BUG-23](../bug-reports/debate-app/BUG-23-microphone-shows-as-unmuted-but-no-audio.md)

**Preconditions:** Active debate session

**Steps:**
1. Toggle mute/unmute 5 times while speaking.
2. Listen on another device.

**Expected result:** Audio is heard only when the icon shows unmuted.

**Actual result:** _to be filled during execution_  
**Status:** Not run
