# 07 - Requirements Validation

## Validation Criteria

Requirements are checked using the following criteria:

- Clarity
- Completeness
- Consistency
- Feasibility
- Testability
- Traceability

## Requirement Validation Table

| Requirement | Clarity | Completeness | Consistency | Feasibility | Testability | Traceability | Result |
|---|---|---|---|---|---|---|---|
| FR-01 | Pass | Pass | Pass | Pass | Pass | Pass | Accepted |
| FR-04 | Pass | Pass | Pass | Pass | Pass | Pass | Accepted |
| FR-05 | Pass | Pass | Pass | Pass | Pass | Pass | Accepted |
| FR-08 | Pass | Pass | Pass | Pass | Pass | Pass | Accepted |
| FR-10 | Pass | Pass | Pass | Pass | Pass | Pass | Accepted |
| NFR-01 | Pass | Pass | Pass | Pass | Pass | Pass | Accepted |
| NFR-05 | Pass | Pass | Pass | Pass | Pass | Pass | Accepted |

## Issues Found

| Issue ID | Requirement | Issue | Correction |
|---|---|---|---|
| VI-01 | NFR-01 | Earlier draft used the vague word "fast". | Rewritten as dashboard load time within 3 seconds. |
| VI-02 | FR-05 | Confirmation requirement originally did not mention timestamp. | Added status and timestamp to make confirmation testable. |
| VI-03 | FR-12 | Report requirement was broad. | Limited report content to assignment count, submission count, missing submissions, and grading status. |

## Revisions

- NFR-01 was revised to include measurable response time.
- FR-05 was revised to include submission status and timestamp.
- FR-12 was revised to define specific report fields.

## Quality Check Result

Passed. At least five requirements were validated and unclear statements were corrected.
