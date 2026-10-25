# Test Cases — Kids' Interactive Storytelling Website

Total: 9

| ID | Title | Type | Priority | Related |
|---|---|---|---|---|
| [TC-017](#tc-017) | Hamburger menu stays stable while scrolling | UI | Low | [BUG-14](../bug-reports/kids-storytelling-site/BUG-14-hamburger-menu-disappears-and-reappears-while-scrolling.md) |
| [TC-018](#tc-018) | Contact phone number is always shown in the hamburger menu | UI | Medium | [BUG-15](../bug-reports/kids-storytelling-site/BUG-15-phone-number-disappears-from-the-contact-information.md) |
| [TC-019](#tc-019) | Age rating badge shows “3+” on page load | UI | Medium | [BUG-16](../bug-reports/kids-storytelling-site/BUG-16-age-rating-badge-shows-a-wrong-counting.md) |
| [TC-020](#tc-020) | Clicking the active language does nothing | Functional | Medium | [BUG-17](../bug-reports/kids-storytelling-site/BUG-17-clicking-the-already-active-language-reloads-the.md) |
| [TC-021](#tc-021) | Switching language GE → EN → GE works | Localization | Medium | [BUG-17](../bug-reports/kids-storytelling-site/BUG-17-clicking-the-already-active-language-reloads-the.md) |
| [TC-022](#tc-022) | Text on all pages has enough contrast | UI / Accessibility | Medium | [BUG-18](../bug-reports/kids-storytelling-site/BUG-18-brand-name-text-on-the-services-page.md) |
| [TC-023](#tc-023) | Contact form — empty message is rejected | Negative / Validation | Medium | [BUG-19](../bug-reports/kids-storytelling-site/BUG-19-contact-form-can-be-sent-with-an.md) |
| [TC-024](#tc-024) | Contact form — valid submission | Positive | Medium | [BUG-19](../bug-reports/kids-storytelling-site/BUG-19-contact-form-can-be-sent-with-an.md) |
| [TC-025](#tc-025) | Contact form — invalid email and phone formats | Negative / Validation | Medium | [BUG-19](../bug-reports/kids-storytelling-site/BUG-19-contact-form-can-be-sent-with-an.md) |

## TC-017

**Title:** Hamburger menu stays stable while scrolling  
**Type:** UI · **Priority:** Low · **Related:** [BUG-14](../bug-reports/kids-storytelling-site/BUG-14-hamburger-menu-disappears-and-reappears-while-scrolling.md)

**Preconditions:** —

**Steps:**
1. Open the hamburger menu.
2. Scroll down and up.

**Expected result:** Menu does not disappear or flicker.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-018

**Title:** Contact phone number is always shown in the hamburger menu  
**Type:** UI · **Priority:** Medium · **Related:** [BUG-15](../bug-reports/kids-storytelling-site/BUG-15-phone-number-disappears-from-the-contact-information.md)

**Preconditions:** —

**Steps:**
1. Open the hamburger menu 5 times (with page reloads).

**Expected result:** Phone number is visible every time, next to the emails.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-019

**Title:** Age rating badge shows “3+” on page load  
**Type:** UI · **Priority:** Medium · **Related:** [BUG-16](../bug-reports/kids-storytelling-site/BUG-16-age-rating-badge-shows-a-wrong-counting.md)

**Preconditions:** —

**Steps:**
1. Open News → Latest news.
2. Refresh the page.

**Expected result:** Badge shows “3+” immediately, without a 1+ → 3+ counter animation.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-020

**Title:** Clicking the active language does nothing  
**Type:** Functional · **Priority:** Medium · **Related:** [BUG-17](../bug-reports/kids-storytelling-site/BUG-17-clicking-the-already-active-language-reloads-the.md)

**Preconditions:** Site is in Georgian; DevTools Console open

**Steps:**
1. Click “GE”.

**Expected result:** No reload and no console errors.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-021

**Title:** Switching language GE → EN → GE works  
**Type:** Localization · **Priority:** Medium · **Related:** [BUG-17](../bug-reports/kids-storytelling-site/BUG-17-clicking-the-already-active-language-reloads-the.md)

**Preconditions:** —

**Steps:**
1. Click “EN”.
2. Click “GE”.

**Expected result:** Content switches correctly each time; no 404 in the console.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-022

**Title:** Text on all pages has enough contrast  
**Type:** UI / Accessibility · **Priority:** Medium · **Related:** [BUG-18](../bug-reports/kids-storytelling-site/BUG-18-brand-name-text-on-the-services-page.md)

**Preconditions:** —

**Steps:**
1. Open every main page (Home, Service, News, Contact).
2. Check headings and labels.

**Expected result:** All text is readable (no white-on-white); contrast meets WCAG AA (4.5:1).

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-023

**Title:** Contact form — empty message is rejected  
**Type:** Negative / Validation · **Priority:** Medium · **Related:** [BUG-19](../bug-reports/kids-storytelling-site/BUG-19-contact-form-can-be-sent-with-an.md)

**Preconditions:** On the Contact page

**Steps:**
1. Fill name, phone and email.
2. Leave the message empty.
3. Click “Send”.

**Expected result:** Form is not sent; a message asks to fill in the message field.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-024

**Title:** Contact form — valid submission  
**Type:** Positive · **Priority:** Medium · **Related:** [BUG-19](../bug-reports/kids-storytelling-site/BUG-19-contact-form-can-be-sent-with-an.md)

**Preconditions:** On the Contact page

**Steps:**
1. Fill all fields with valid data, including a message.
2. Click “Send”.

**Expected result:** Success message is shown; the form is cleared.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-025

**Title:** Contact form — invalid email and phone formats  
**Type:** Negative / Validation · **Priority:** Medium · **Related:** [BUG-19](../bug-reports/kids-storytelling-site/BUG-19-contact-form-can-be-sent-with-an.md)

**Preconditions:** On the Contact page

**Steps:**
1. Enter “test@” as email and “abc” as phone.
2. Click “Send”.

**Expected result:** Field-level validation errors are shown; the form is not sent.

**Actual result:** _to be filled during execution_  
**Status:** Not run
