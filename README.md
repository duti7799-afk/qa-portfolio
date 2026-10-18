# QA Portfolio — Nino Zaitseva

Manual QA tester. This repository collects real bug reports and product improvement recommendations I wrote while testing web and mobile applications, including **AI-powered products** (AI chatbot and AI search).

> **Confidentiality:** all reports come from commercial projects covered by an NDA. Product names, company names, URLs and attachments have been removed or replaced with generic descriptions.

## Skills shown here

- Functional, UI/UX and regression testing of web and Android apps
- Testing AI chatbots: context handling, hallucination-type issues, handoff to live operators
- Boundary and negative testing (working-hours logic, validation, duplicate data)
- Security & access-control checks (password policy, role separation)
- Localization testing (Georgian / English)
- Test design: test cases and regression checklists derived from real defects
- Clear bug reports: environment, preconditions, steps, expected vs. actual result
- Tools: Jira, ClickUp, Postman, Swagger, Chrome DevTools

## Summary

| Project | Description | Bug reports | Recommendations |
|---|---|:---:|:---:|
| AI Shopping Assistant | E-commerce website with an AI chatbot, AI product search and live-operator handoff (web, desktop & Android) | 13 | 8 |
| Kids' Interactive Storytelling Website | Website with animated stories and mini-games for children aged 3+ | 6 | 4 |
| Job Board & Community Platform | Job listings, blogs, comments, notifications and an admin panel | 1 | 5 |
| Dating Mobile App | Android dating app with swipe-based matching and profile verification | 2 | 3 |
| Online Debate App | Android app for live voice debate sessions | 1 | 0 |
| HR / Recruitment Platform | Web platform with separate candidate and company accounts | 2 | 0 |
| Mobile App — Account Settings | Android app, profile and password management | 1 | 0 |
| Language Learning Website | Bilingual (Georgian / English) learning website | 1 | 0 |
| Fashion E-commerce Website | Online clothing store with categories and product filters | 1 | 0 |
| **Total** | | **28** | **20** |

## Bug reports


### AI Shopping Assistant

| ID | Title | Priority |
|---|---|---|
| [BUG-01](bug-reports/ai-shopping-assistant/BUG-01-search-clear-x-button-clears-the-results.md) | Search clear (X) button clears the results grid but leaves the query in the search field | Normal |
| [BUG-02](bug-reports/ai-shopping-assistant/BUG-02-chatbot-widget-overlaps-the-back-to-top.md) | Chatbot widget overlaps the “Back to Top” button at the bottom of the page | High |
| [BUG-03](bug-reports/ai-shopping-assistant/BUG-03-user-is-routed-to-a-live-operator.md) | User is routed to a live operator outside working hours when the shift end time is later than 17:00 | High |
| [BUG-04](bug-reports/ai-shopping-assistant/BUG-04-operator-status-indicator-shows-green-online-during.md) | Operator status indicator shows green (online) during non-working hours | High |
| [BUG-05](bug-reports/ai-shopping-assistant/BUG-05-chatbot-leaks-data-from-the-unfiltered-catalog.md) | Chatbot leaks data from the unfiltered catalog instead of staying in the current filtered context | High |
| [BUG-06](bug-reports/ai-shopping-assistant/BUG-06-clicking-a-quoted-replied-message-in-the.md) | Clicking a quoted (replied) message in the chat does not scroll to the original message | Normal |
| [BUG-07](bug-reports/ai-shopping-assistant/BUG-07-reply-on-an-item-in-an-older.md) | “Reply” on an item in an older catalog uses the context of the latest search results | High |
| [BUG-08](bug-reports/ai-shopping-assistant/BUG-08-chatbot-returns-the-wrong-product-when-a.md) | Chatbot returns the wrong product when a catalog item is selected by ordinal (“the third one”) | High |
| [BUG-09](bug-reports/ai-shopping-assistant/BUG-09-negative-feedback-message-sends-the-user-to.md) | Negative feedback message sends the user to an operator without asking for confirmation | High |
| [BUG-10](bug-reports/ai-shopping-assistant/BUG-10-chatbot-cannot-find-the-nearest-store-by.md) | Chatbot cannot find the nearest store by landmark or area name | Normal |
| [BUG-11](bug-reports/ai-shopping-assistant/BUG-11-background-blur-makes-products-unreadable-while-the.md) | Background blur makes products unreadable while the chat is open, even after resizing the chat | Normal |
| [BUG-12](bug-reports/ai-shopping-assistant/BUG-12-several-accounts-can-be-registered-with-the.md) | Several accounts can be registered with the same mobile number (admin panel) | High |
| [BUG-13](bug-reports/ai-shopping-assistant/BUG-13-chat-icon-does-not-always-show-a.md) | Chat icon does not always show a notification when the answer arrives while the chat is minimised | Normal |

### Kids' Interactive Storytelling Website

| ID | Title | Priority |
|---|---|---|
| [BUG-14](bug-reports/kids-storytelling-site/BUG-14-hamburger-menu-disappears-and-reappears-while-scrolling.md) | Hamburger menu disappears and reappears while scrolling | Normal |
| [BUG-15](bug-reports/kids-storytelling-site/BUG-15-phone-number-disappears-from-the-contact-information.md) | Phone number disappears from the contact information in the hamburger menu | Normal |
| [BUG-16](bug-reports/kids-storytelling-site/BUG-16-age-rating-badge-shows-a-wrong-counting.md) | Age rating badge shows a wrong counting animation (1+ → 3+) on page load | High |
| [BUG-17](bug-reports/kids-storytelling-site/BUG-17-clicking-the-already-active-language-reloads-the.md) | Clicking the already active language reloads the page and causes a 404 console error | High |
| [BUG-18](bug-reports/kids-storytelling-site/BUG-18-brand-name-text-on-the-services-page.md) | Brand name text on the Services page is invisible (white text on white background) | Normal |
| [BUG-19](bug-reports/kids-storytelling-site/BUG-19-contact-form-can-be-sent-with-an.md) | Contact form can be sent with an empty message | Normal |

### Job Board & Community Platform

| ID | Title | Priority |
|---|---|---|
| [BUG-20](bug-reports/job-board-platform/BUG-20-clicking-a-reaction-to-your-comment-notification.md) | Clicking a “reaction to your comment” notification opens the home page instead of the related post | Normal |

### Dating Mobile App

| ID | Title | Priority |
|---|---|---|
| [BUG-21](bug-reports/dating-app/BUG-21-header-elements-overlap-the-status-bar-safe.md) | Header elements overlap the status bar / safe area on every screen | Normal |
| [BUG-22](bug-reports/dating-app/BUG-22-search-preferences-age-range-and-gender-reset.md) | Search preferences (age range and gender) reset after the app is force-closed | High |

### Online Debate App

| ID | Title | Priority |
|---|---|---|
| [BUG-23](bug-reports/debate-app/BUG-23-microphone-shows-as-unmuted-but-no-audio.md) | Microphone shows as unmuted but no audio is broadcast during a debate session | High |

### HR / Recruitment Platform

| ID | Title | Priority |
|---|---|---|
| [BUG-24](bug-reports/hr-platform/BUG-24-no-error-message-when-registering-with-an.md) | No error message when registering with an email that is already registered | High |
| [BUG-25](bug-reports/hr-platform/BUG-25-candidate-credentials-log-the-user-in-to.md) | Candidate credentials log the user in to the Company portal without a company registration | High |

### Mobile App — Account Settings

| ID | Title | Priority |
|---|---|---|
| [BUG-26](bug-reports/mobile-account-app/BUG-26-password-strength-is-not-validated-when-changing.md) | Password strength is not validated when changing the password | Urgent |

### Language Learning Website

| ID | Title | Priority |
|---|---|---|
| [BUG-27](bug-reports/language-learning-site/BUG-27-switching-the-site-language-to-english-translates.md) | Switching the site language to English translates only the menu bar | High |

### Fashion E-commerce Website

| ID | Title | Priority |
|---|---|---|
| [BUG-28](bug-reports/fashion-ecommerce/BUG-28-product-sorting-filter-e-g-discount-does.md) | Product sorting/filter (e.g. “Discount”) does not work inside a category | High |

## Recommendations


### AI Shopping Assistant

| ID | Title | Priority | Status |
|---|---|---|---|
| [REC-01](recommendations/ai-shopping-assistant/REC-01-handle-multi-product-questions-find-stores-that.md) | Handle multi-product questions (find stores that have all requested items) | Normal | Submitted |
| [REC-02](recommendations/ai-shopping-assistant/REC-02-ask-clarifying-questions-when-the-request-is.md) | Ask clarifying questions when the request is too broad | High | Submitted |
| [REC-03](recommendations/ai-shopping-assistant/REC-03-allow-the-chat-window-to-be-resized.md) | Allow the chat window to be resized and moved | Normal | Submitted |
| [REC-04](recommendations/ai-shopping-assistant/REC-04-support-excel-file-upload-in-the-chatbot.md) | Support Excel file upload in the chatbot | Normal | Submitted |
| [REC-05](recommendations/ai-shopping-assistant/REC-05-configure-operator-working-hours-per-operator-not.md) | Configure operator working hours per operator, not globally | High | Submitted |
| [REC-06](recommendations/ai-shopping-assistant/REC-06-add-a-short-pre-chat-identification-form.md) | Add a short pre-chat identification form | — | Submitted |
| [REC-07](recommendations/ai-shopping-assistant/REC-07-replace-the-technical-word-header-in-the.md) | Replace the technical word “header” in the out-of-office message | Normal | Submitted |
| [REC-08](recommendations/ai-shopping-assistant/REC-08-show-the-registered-phone-number-in-the.md) | Show the registered phone number in the operator’s profile | Normal | Submitted |

### Kids' Interactive Storytelling Website

| ID | Title | Priority | Status |
|---|---|---|---|
| [REC-09](recommendations/kids-storytelling-site/REC-09-let-children-move-to-the-next-stage.md) | Let children move to the next stage when they finish a task early | Normal | Submitted |
| [REC-10](recommendations/kids-storytelling-site/REC-10-hide-the-sound-settings-in-a-dropdown.md) | Hide the sound settings in a dropdown behind a settings icon | — | Submitted |
| [REC-11](recommendations/kids-storytelling-site/REC-11-keep-sound-controls-available-during-the-game.md) | Keep sound controls available during the game | Low | Submitted |
| [REC-12](recommendations/kids-storytelling-site/REC-12-put-all-contact-information-in-one-place.md) | Put all contact information in one place | Low | Submitted |

### Job Board & Community Platform

| ID | Title | Priority | Status |
|---|---|---|---|
| [REC-13](recommendations/job-board-platform/REC-13-make-the-close-comment-window-message-clearer.md) | Make the “close comment window” message clearer | Normal | Implemented |
| [REC-14](recommendations/job-board-platform/REC-14-add-an-unblock-user-action-to-the.md) | Add an “Unblock user” action to the admin panel | High | Implemented |
| [REC-15](recommendations/job-board-platform/REC-15-warn-the-user-before-leaving-a-blog.md) | Warn the user before leaving a blog post that is being written | Normal | Implemented |
| [REC-16](recommendations/job-board-platform/REC-16-add-a-separate-saved-jobs-section-to.md) | Add a separate “Saved jobs” section to the user profile | Normal | Accepted |
| [REC-17](recommendations/job-board-platform/REC-17-publish-clear-rules-for-when-a-user.md) | Publish clear rules for when a user can be blocked | High | Accepted |

### Dating Mobile App

| ID | Title | Priority | Status |
|---|---|---|---|
| [REC-18](recommendations/dating-app/REC-18-add-an-undo-rewind-action-for-accidental.md) | Add an Undo / Rewind action for accidental swipes | — | In review |
| [REC-19](recommendations/dating-app/REC-19-prevent-deleting-the-only-verified-face-photo.md) | Prevent deleting the only verified face photo after verification | — | In review |
| [REC-20](recommendations/dating-app/REC-20-add-onboarding-hints-for-swipe-right-left.md) | Add onboarding hints for swipe right / left | — | In review |

## Test cases

Written from the bug reports above — each test case would catch the related bug and covers nearby positive, negative and boundary scenarios.

| Project | Test cases | File |
|---|:---:|---|
| AI Shopping Assistant | 16 | [test-cases/ai-shopping-assistant.md](test-cases/ai-shopping-assistant.md) |
| Kids' Interactive Storytelling Website | 9 | [test-cases/kids-storytelling-site.md](test-cases/kids-storytelling-site.md) |
| Job Board & Community Platform | 5 | [test-cases/job-board-platform.md](test-cases/job-board-platform.md) |
| Dating Mobile App | 4 | [test-cases/dating-app.md](test-cases/dating-app.md) |
| Online Debate App | 2 | [test-cases/debate-app.md](test-cases/debate-app.md) |
| HR / Recruitment Platform | 3 | [test-cases/hr-platform.md](test-cases/hr-platform.md) |
| Mobile App — Account Settings | 3 | [test-cases/mobile-account-app.md](test-cases/mobile-account-app.md) |
| Language Learning Website | 2 | [test-cases/language-learning-site.md](test-cases/language-learning-site.md) |
| Fashion E-commerce Website | 2 | [test-cases/fashion-ecommerce.md](test-cases/fashion-ecommerce.md) |
| **Total** | **46** | |

## Checklists

Quick regression checklists per product, based on the areas where bugs were found.

| Project | Items | File |
|---|:---:|---|
| AI Shopping Assistant | 23 | [checklists/ai-shopping-assistant.md](checklists/ai-shopping-assistant.md) |
| Kids' Interactive Storytelling Website | 14 | [checklists/kids-storytelling-site.md](checklists/kids-storytelling-site.md) |
| Job Board & Community Platform | 9 | [checklists/job-board-platform.md](checklists/job-board-platform.md) |
| Dating Mobile App | 10 | [checklists/dating-app.md](checklists/dating-app.md) |
| Online Debate App | 5 | [checklists/debate-app.md](checklists/debate-app.md) |
| HR / Recruitment Platform | 7 | [checklists/hr-platform.md](checklists/hr-platform.md) |
| Mobile App — Account Settings | 5 | [checklists/mobile-account-app.md](checklists/mobile-account-app.md) |
| Language Learning Website | 4 | [checklists/language-learning-site.md](checklists/language-learning-site.md) |
| Fashion E-commerce Website | 4 | [checklists/fashion-ecommerce.md](checklists/fashion-ecommerce.md) |
| **Total** | **81** | |

## Templates

- [Bug report template](templates/bug-report-template.md)
- [Recommendation template](templates/recommendation-template.md)
- [Test case template](templates/test-case-template.md)

## Recommendation status

- **Implemented** — implemented by the development team
- **Accepted** — approved for implementation
- **Submitted / In review** — proposed, under review
