# REC-19: Prevent deleting the only verified face photo after verification

| Field | Value |
|---|---|
| **Project** | Dating Mobile App |
| **Priority** | — |
| **Status** | In review |

## Current Behavior
Business rules require at least one clear face photo for verification, but after verification the user can upload other (non-face) photos and delete the verified one — the system allows it.

## Problem
The verification requirement can be bypassed.

## Proposed Solution
Add validation on Edit Profile: either block deleting the last verified photo with an error message, or hide the profile from others until a new face photo is uploaded and verified again.

## Justification
Protects the business logic and trust in verified profiles.
