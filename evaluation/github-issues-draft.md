# GitHub Issues Draft

Use the following text to create the required GitHub Issues manually in the repository.

## Issue 1

### Title

`[SKILL IMPROVEMENT] Prevent unsupported assumptions`

### Body

## Problem

Some AI outputs included assumptions that were not directly supported by the case description or stakeholder input.

## Proposed Improvement

Update each `SKILL.md` to require assumptions to be labeled explicitly with `ASSUMPTION` and unsupported missing information to be labeled as `OPEN QUESTION`.

## Affected Skill

- `skills/01-inception/SKILL.md`
- `skills/02-elicitation/SKILL.md`
- `skills/03-specification/SKILL.md`

## Decision

Approved. The skills were revised to make assumption labeling mandatory.

## Issue 2

### Title

`[CHANGE REQUEST] Add late submission status`

### Body

## Description

Add a late submission status so lecturers and students can distinguish on-time submissions from submissions made after the deadline.

## Reason

Deadline handling is important for grading fairness and academic process consistency.

## Affected Requirements

- FR-04
- FR-05
- FR-06
- US-05
- US-06
- AC-09
- AC-11

## Impact

The change affects assignment submission, status display, confirmation, and validation. It does not change the core system scope because deadline status is already part of assignment tracking.

## Proposed Decision

Approve with condition. The final late submission policy must be confirmed by the academic department.
