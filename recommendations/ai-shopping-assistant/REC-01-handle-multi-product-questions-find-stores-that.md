# REC-01: Handle multi-product questions (find stores that have all requested items)

| Field | Value |
|---|---|
| **Project** | AI Shopping Assistant |
| **Priority** | Normal |
| **Status** | Submitted |

## Current Behavior
The chatbot answers simple availability questions well (e.g. “Where is iPhone 15 available?”). For a combined question like “Where can I buy a phone, a case and a charger together?” it cannot combine the data and just suggests buying online.

## Problem
The user has to check each item separately and compare branches manually, which adds effort and lowers the value of the chatbot.

## Proposed Solution
Add logic for multi-part questions: identify the branches where the products are available and say how many of them each branch has (e.g. 2 of 3, 1 of 3), or that none are available.

## Justification
Customers save time and get the products they want faster.
