# REC-02: Ask clarifying questions when the request is too broad

| Field | Value |
|---|---|
| **Project** | AI Shopping Assistant |
| **Priority** | High |
| **Status** | Submitted |

## Current Behavior
When the user gives only a price limit (e.g. “up to 100 GEL”), the chatbot returns random products from different categories.

## Problem
Without a follow-up question the bot shows products that do not match the user’s need, which makes it unpractical.

## Proposed Solution
Improve the bot logic so it asks a clarifying question (e.g. which category) before showing results.

## Justification
Simpler and more relevant search for the user.
