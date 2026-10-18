# Test Cases — AI Shopping Assistant

Total: 16

| ID | Title | Type | Priority | Related |
|---|---|---|---|---|
| [TC-001](#tc-001) | Clear (X) button resets both the search field and the results | Functional | Medium | [BUG-01](../bug-reports/ai-shopping-assistant/BUG-01-search-clear-x-button-clears-the-results.md) |
| [TC-002](#tc-002) | Clear (X) button is hidden or disabled when the search field is empty | UI | Low | [BUG-01](../bug-reports/ai-shopping-assistant/BUG-01-search-clear-x-button-clears-the-results.md) |
| [TC-003](#tc-003) | “Back to Top” button is visible and clickable with the chatbot widget on screen | UI | High | [BUG-02](../bug-reports/ai-shopping-assistant/BUG-02-chatbot-widget-overlaps-the-back-to-top.md) |
| [TC-004](#tc-004) | Operator routing is blocked after working hours (end time later than 17:00) | Boundary | High | [BUG-03](../bug-reports/ai-shopping-assistant/BUG-03-user-is-routed-to-a-live-operator.md) |
| [TC-005](#tc-005) | Operator routing at the working-hours boundaries | Boundary | High | [BUG-03](../bug-reports/ai-shopping-assistant/BUG-03-user-is-routed-to-a-live-operator.md) |
| [TC-006](#tc-006) | Operator status indicator matches real availability | UI | Medium | [BUG-04](../bug-reports/ai-shopping-assistant/BUG-04-operator-status-indicator-shows-green-online-during.md) |
| [TC-007](#tc-007) | Chatbot respects a limited (filtered) result set | AI / Context | High | [BUG-05](../bug-reports/ai-shopping-assistant/BUG-05-chatbot-leaks-data-from-the-unfiltered-catalog.md) |
| [TC-008](#tc-008) | Clicking a quoted message scrolls to the original | Functional | Low | [BUG-06](../bug-reports/ai-shopping-assistant/BUG-06-clicking-a-quoted-replied-message-in-the.md) |
| [TC-009](#tc-009) | “Reply” on an older catalog uses that catalog’s context | AI / Context | High | [BUG-07](../bug-reports/ai-shopping-assistant/BUG-07-reply-on-an-item-in-an-older.md) |
| [TC-010](#tc-010) | Ordinal reference selects the correct catalog item | AI / Context | High | [BUG-08](../bug-reports/ai-shopping-assistant/BUG-08-chatbot-returns-the-wrong-product-when-a.md) |
| [TC-011](#tc-011) | Negative feedback does not end the AI conversation without confirmation | AI / UX | Medium | [BUG-09](../bug-reports/ai-shopping-assistant/BUG-09-negative-feedback-message-sends-the-user-to.md) |
| [TC-012](#tc-012) | Store search by landmark or area name | AI | Low | [BUG-10](../bug-reports/ai-shopping-assistant/BUG-10-chatbot-cannot-find-the-nearest-store-by.md) |
| [TC-013](#tc-013) | Product page stays usable while the chat is open | UI / UX | Low | [BUG-11](../bug-reports/ai-shopping-assistant/BUG-11-background-blur-makes-products-unreadable-while-the.md) |
| [TC-014](#tc-014) | Registration with an already used mobile number is rejected | Negative / Validation | High | [BUG-12](../bug-reports/ai-shopping-assistant/BUG-12-several-accounts-can-be-registered-with-the.md) |
| [TC-015](#tc-015) | Chat icon shows a notification when an answer arrives while minimised | Functional | Low | [BUG-13](../bug-reports/ai-shopping-assistant/BUG-13-chat-icon-does-not-always-show-a.md) |
| [TC-016](#tc-016) | Per-operator working hours are saved independently | Functional | High | [REC-05](../recommendations/ai-shopping-assistant/REC-05-configure-operator-working-hours-per-operator-not.md) |

## TC-001

**Title:** Clear (X) button resets both the search field and the results  
**Type:** Functional · **Priority:** Medium · **Related:** [BUG-01](../bug-reports/ai-shopping-assistant/BUG-01-search-clear-x-button-clears-the-results.md)

**Preconditions:** Search results are shown for a query

**Steps:**
1. Type “phone” in the search field and run the search.
2. Click the X (clear) button.

**Expected result:** Search field is empty and the results grid is cleared.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-002

**Title:** Clear (X) button is hidden or disabled when the search field is empty  
**Type:** UI · **Priority:** Low · **Related:** [BUG-01](../bug-reports/ai-shopping-assistant/BUG-01-search-clear-x-button-clears-the-results.md)

**Preconditions:** Search field is empty

**Steps:**
1. Open the website.
2. Look at the search field.

**Expected result:** X button is not shown (or does nothing) while the field is empty.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-003

**Title:** “Back to Top” button is visible and clickable with the chatbot widget on screen  
**Type:** UI · **Priority:** High · **Related:** [BUG-02](../bug-reports/ai-shopping-assistant/BUG-02-chatbot-widget-overlaps-the-back-to-top.md)

**Preconditions:** Long list of search results

**Steps:**
1. Search for “phone”.
2. Scroll to the end of the results.
3. Click “Back to Top”.

**Expected result:** Button is not covered by the chatbot widget; the page scrolls to the top.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-004

**Title:** Operator routing is blocked after working hours (end time later than 17:00)  
**Type:** Boundary · **Priority:** High · **Related:** [BUG-03](../bug-reports/ai-shopping-assistant/BUG-03-user-is-routed-to-a-live-operator.md)

**Preconditions:** Working hours 09:00–19:00; current time 19:30

**Steps:**
1. Open the chatbot and start a chat.
2. Click “Operator”.

**Expected result:** An off-hours message is shown; the user is not routed to an operator.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-005

**Title:** Operator routing at the working-hours boundaries  
**Type:** Boundary · **Priority:** High · **Related:** [BUG-03](../bug-reports/ai-shopping-assistant/BUG-03-user-is-routed-to-a-live-operator.md)

**Preconditions:** Working hours 09:00–19:00

**Steps:**
1. Request an operator at 08:59, 09:00, 18:59 and 19:00 (change system time or test at those times).

**Expected result:** 08:59 and 19:00 → off-hours message; 09:00 and 18:59 → routed to an operator.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-006

**Title:** Operator status indicator matches real availability  
**Type:** UI · **Priority:** Medium · **Related:** [BUG-04](../bug-reports/ai-shopping-assistant/BUG-04-operator-status-indicator-shows-green-online-during.md)

**Preconditions:** Outside working hours

**Steps:**
1. Open the chatbot and request an operator.
2. Close the “operator unavailable” popup.
3. Check the status dot next to the operator.

**Expected result:** Indicator is grey/red (offline), not green.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-007

**Title:** Chatbot respects a limited (filtered) result set  
**Type:** AI / Context · **Priority:** High · **Related:** [BUG-05](../bug-reports/ai-shopping-assistant/BUG-05-chatbot-leaks-data-from-the-unfiltered-catalog.md)

**Preconditions:** —

**Steps:**
1. Ask “Show me only the first 3 phones”.
2. Reply to that message: “Tell me about the 4th phone”.

**Expected result:** Bot says there is no 4th item in the current list or offers to show more; it does not invent or pull a hidden item.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-008

**Title:** Clicking a quoted message scrolls to the original  
**Type:** Functional · **Priority:** Low · **Related:** [BUG-06](../bug-reports/ai-shopping-assistant/BUG-06-clicking-a-quoted-replied-message-in-the.md)

**Preconditions:** A reply to a bot message exists in the chat

**Steps:**
1. Click the quoted header inside your reply.

**Expected result:** Chat scrolls to the original message and highlights it briefly.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-009

**Title:** “Reply” on an older catalog uses that catalog’s context  
**Type:** AI / Context · **Priority:** High · **Related:** [BUG-07](../bug-reports/ai-shopping-assistant/BUG-07-reply-on-an-item-in-an-older.md)

**Preconditions:** Two catalogs in one chat: “phone”, then “iPad”

**Steps:**
1. Scroll up to the “phone” catalog.
2. Click “Reply” on the first phone and ask “Tell me more”.

**Expected result:** Answer is about the selected phone, not about an iPad.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-010

**Title:** Ordinal reference selects the correct catalog item  
**Type:** AI / Context · **Priority:** High · **Related:** [BUG-08](../bug-reports/ai-shopping-assistant/BUG-08-chatbot-returns-the-wrong-product-when-a.md)

**Preconditions:** Bot has returned a laptop catalog

**Steps:**
1. Send “the third one” as a normal message.
2. Repeat as a Reply to the catalog.

**Expected result:** In both cases the bot describes the 3rd laptop in the list.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-011

**Title:** Negative feedback does not end the AI conversation without confirmation  
**Type:** AI / UX · **Priority:** Medium · **Related:** [BUG-09](../bug-reports/ai-shopping-assistant/BUG-09-negative-feedback-message-sends-the-user-to.md)

**Preconditions:** Active AI chat

**Steps:**
1. Send “You are answering incorrectly”.

**Expected result:** Bot acknowledges the feedback and asks what went wrong, or asks the user to confirm before transferring to an operator.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-012

**Title:** Store search by landmark or area name  
**Type:** AI · **Priority:** Low · **Related:** [BUG-10](../bug-reports/ai-shopping-assistant/BUG-10-chatbot-cannot-find-the-nearest-store-by.md)

**Preconditions:** Store location data is available

**Steps:**
1. Ask “Where is the nearest branch to Station Square?”

**Expected result:** Bot returns the nearest branch address, or clearly says location search is not supported.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-013

**Title:** Product page stays usable while the chat is open  
**Type:** UI / UX · **Priority:** Low · **Related:** [BUG-11](../bug-reports/ai-shopping-assistant/BUG-11-background-blur-makes-products-unreadable-while-the.md)

**Preconditions:** Product results are shown

**Steps:**
1. Open the chat.
2. Resize the chat window to a smaller size.
3. Try to read and click a product behind it.

**Expected result:** Behaviour matches the design spec (non-modal chat: products readable and clickable).

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-014

**Title:** Registration with an already used mobile number is rejected  
**Type:** Negative / Validation · **Priority:** High · **Related:** [BUG-12](../bug-reports/ai-shopping-assistant/BUG-12-several-accounts-can-be-registered-with-the.md)

**Preconditions:** A user exists with phone number X

**Steps:**
1. Open the registration form.
2. Fill valid data and phone number X.
3. Click “Sign up”.

**Expected result:** Registration fails with “A user with this phone number already exists”; the field is highlighted.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-015

**Title:** Chat icon shows a notification when an answer arrives while minimised  
**Type:** Functional · **Priority:** Low · **Related:** [BUG-13](../bug-reports/ai-shopping-assistant/BUG-13-chat-icon-does-not-always-show-a.md)

**Preconditions:** —

**Steps:**
1. Ask a question.
2. Minimise the chat before the answer arrives.
3. Repeat 5 times.

**Expected result:** Every time, the chat icon shows a badge/animation when the answer is ready (5/5).

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-016

**Title:** Per-operator working hours are saved independently  
**Type:** Functional · **Priority:** High · **Related:** [REC-05](../recommendations/ai-shopping-assistant/REC-05-configure-operator-working-hours-per-operator-not.md)

**Preconditions:** Two operators, A and B

**Steps:**
1. Change working hours for operator A.
2. Open operator B’s profile.

**Expected result:** Operator B’s hours are unchanged.

**Actual result:** _to be filled during execution_  
**Status:** Not run
