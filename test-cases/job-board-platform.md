# Test Cases — Job Board & Community Platform

Total: 5

| ID | Title | Type | Priority | Related |
|---|---|---|---|---|
| [TC-026](#tc-026) | Reaction notification opens the related post | Functional | Medium | [BUG-20](../bug-reports/job-board-platform/BUG-20-clicking-a-reaction-to-your-comment-notification.md) |
| [TC-027](#tc-027) | Closing a comment with unsaved text shows a clear warning | UX | Medium | [REC-13](../recommendations/job-board-platform/REC-13-make-the-close-comment-window-message-clearer.md) |
| [TC-028](#tc-028) | Leaving the blog editor with unsaved text asks for confirmation | UX | Medium | [REC-15](../recommendations/job-board-platform/REC-15-warn-the-user-before-leaving-a-blog.md) |
| [TC-029](#tc-029) | Admin can block and unblock a user | Functional | High | [REC-14](../recommendations/job-board-platform/REC-14-add-an-unblock-user-action-to-the.md) |
| [TC-030](#tc-030) | Saved jobs appear in the profile section | Functional | Low | [REC-16](../recommendations/job-board-platform/REC-16-add-a-separate-saved-jobs-section-to.md) |

## TC-026

**Title:** Reaction notification opens the related post  
**Type:** Functional · **Priority:** Medium · **Related:** [BUG-20](../bug-reports/job-board-platform/BUG-20-clicking-a-reaction-to-your-comment-notification.md)

**Preconditions:** User has a comment with a reaction

**Steps:**
1. Open notifications.
2. Click the reaction notification.

**Expected result:** The related blog/job post opens, scrolled to the comment.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-027

**Title:** Closing a comment with unsaved text shows a clear warning  
**Type:** UX · **Priority:** Medium · **Related:** [REC-13](../recommendations/job-board-platform/REC-13-make-the-close-comment-window-message-clearer.md)

**Preconditions:** User typed text in the comment field

**Steps:**
1. Click Close.

**Expected result:** Message “Your text will not be saved” with “Close” and “Continue editing”; each button works as named.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-028

**Title:** Leaving the blog editor with unsaved text asks for confirmation  
**Type:** UX · **Priority:** Medium · **Related:** [REC-15](../recommendations/job-board-platform/REC-15-warn-the-user-before-leaving-a-blog.md)

**Preconditions:** User is writing a blog post

**Steps:**
1. Click another menu item.

**Expected result:** Confirmation dialog (Yes / No); “No” keeps the text.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-029

**Title:** Admin can block and unblock a user  
**Type:** Functional · **Priority:** High · **Related:** [REC-14](../recommendations/job-board-platform/REC-14-add-an-unblock-user-action-to-the.md)

**Preconditions:** Admin is logged in

**Steps:**
1. Block user U.
2. Unblock user U.
3. Log in as U.

**Expected result:** U cannot act while blocked and has full access after unblocking.

**Actual result:** _to be filled during execution_  
**Status:** Not run

## TC-030

**Title:** Saved jobs appear in the profile section  
**Type:** Functional · **Priority:** Low · **Related:** [REC-16](../recommendations/job-board-platform/REC-16-add-a-separate-saved-jobs-section-to.md)

**Preconditions:** User has saved 3 jobs

**Steps:**
1. Open Profile → Saved jobs.

**Expected result:** All 3 jobs are listed, sorted by date.

**Actual result:** _to be filled during execution_  
**Status:** Not run
