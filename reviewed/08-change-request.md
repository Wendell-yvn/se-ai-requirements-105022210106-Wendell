# 08 - Change Request

## Change Request ID

CR-01

## Title

Add Late Submission Status

## Description

Add a clear late submission status when a student submits an assignment after the deadline, if the system policy allows late submission.

## Reason

Students and lecturers need clarity about whether a submission was made on time or after the deadline. Without a late status, lecturers may have difficulty applying grading policies consistently.

## Affected Requirements

- FR-04: Student file submission
- FR-05: Submission confirmation
- FR-06: Assignment deadline status
- US-05: Student uploads assignment file
- US-06: Student views assignment status, grade, and feedback
- AC-09: Successful upload confirmation
- AC-11: Assignment status display

## Impact Analysis

| Area | Impact |
|---|---|
| Functional Requirements | FR-06 already includes late status, so the change confirms and strengthens this behavior. |
| User Stories | US-06 must include late status visibility. |
| Acceptance Criteria | AC-11 must verify that late status is displayed when applicable. |
| Priority | FR-06 remains Should because core submission can work without full late policy automation. |
| Scope | Still within assignment status tracking scope. |
| Risk | Policy ambiguity remains if the campus does not define late submission rules. |

## Decision

Approved with condition.

## Rationale

The change supports transparency and grading consistency. However, the exact late submission policy must be confirmed by the academic department.

## Follow-Up Open Question

- OPEN QUESTION: Should late submissions be accepted automatically, blocked, or accepted only with lecturer approval?
