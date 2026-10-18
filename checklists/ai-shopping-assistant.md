# Checklist — AI Shopping Assistant

Mark each item ✅ Pass / ❌ Fail / ⏭ Skip during a test run.

## Search

- [ ] Search returns relevant results for a simple query
- [ ] Clear (X) button resets the field and the results
- [ ] Special characters and very long queries do not break the page
- [ ] Empty search is handled (message or no action)

## Chatbot — context & AI answers

- [ ] Bot respects limits and filters given by the user (e.g. “only 3”)
- [ ] Reply on an older message uses that message’s context
- [ ] Ordinal references (“the third one”) select the right item
- [ ] Bot does not invent products, prices or stock (no hallucinations)
- [ ] Broad requests get a clarifying question
- [ ] Answers stay in the language of the conversation

## Chatbot — UI

- [ ] Widget does not overlap page buttons (Back to Top, cart, etc.)
- [ ] Quoted message click scrolls to the original
- [ ] Notification appears when an answer arrives while minimised
- [ ] Long input text expands or scrolls the input box
- [ ] Chat window works on mobile screen sizes

## Operator handoff

- [ ] Routing works inside working hours
- [ ] Routing is blocked outside working hours (check boundaries)
- [ ] Operator status indicator matches real availability
- [ ] Negative feedback does not end the AI chat without confirmation
- [ ] Working hours are saved per operator

## Registration / admin

- [ ] Duplicate phone number is rejected
- [ ] Duplicate email is rejected
- [ ] Required fields are validated
