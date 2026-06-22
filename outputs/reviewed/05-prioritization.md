# 05 - Negotiation and Prioritization

## Prioritization Method

Requirements are prioritized using MoSCoW:

- Must: Required for core assignment workflow.
- Should: Important for usability or operational value.
- Could: Useful but not essential for the first baseline.
- Won't: Excluded from the current scope.

## Requirement Priority Table

| Requirement | Priority | Reason |
|---|---|---|
| FR-01 | Must | Lecturers must create assignments before students can view or submit work. |
| FR-02 | Should | Editing assignments improves flexibility, but initial creation is more critical. |
| FR-03 | Must | Students must see assignments to complete their tasks. |
| FR-04 | Must | File submission is a core purpose of the system. |
| FR-05 | Must | Submission confirmation protects students from uncertainty after upload. |
| FR-06 | Should | Status visibility improves usability and reduces confusion. |
| FR-07 | Must | Lecturers must view submissions to assess student work. |
| FR-08 | Must | Grading and feedback are core academic processes. |
| FR-09 | Should | Published grade and feedback visibility supports learning outcomes. |
| FR-10 | Must | User and role management is required for secure access. |
| FR-11 | Should | Course management supports proper assignment organization. |
| FR-12 | Could | Reports are useful for monitoring but not required for the core submission workflow. |

## Stakeholder Conflicts

| Conflict | Stakeholders | Decision |
|---|---|---|
| Students may want flexible resubmission, while lecturers may want stable grading records. | Student, Lecturer | Treat resubmission as an open question until policy is confirmed. |
| Administrators may want broad access, while privacy rules require restricted access to grades and submissions. | Administrator, Student, Lecturer | Apply role-based access and limit grade/submission access to authorized users. |
| Students may want late submission acceptance, while lecturers may want deadline enforcement. | Student, Lecturer | Mark late submissions clearly if accepted by policy. |

## Dependencies

| Requirement | Depends On | Explanation |
|---|---|---|
| FR-03 | FR-01 | Students can view assignments only after lecturers create them. |
| FR-04 | FR-01, FR-03 | Students submit to assignments that exist and are visible. |
| FR-05 | FR-04 | Confirmation occurs after file submission. |
| FR-07 | FR-04 | Lecturers view submitted files after students upload them. |
| FR-08 | FR-07 | Grading requires access to submissions. |
| FR-09 | FR-08 | Students view grades after lecturers enter and publish them. |

## Trade-Off Decisions

- Role-based security is prioritized over administrative convenience because student academic data must be protected.
- Submission confirmation is classified as Must because it reduces disputes about whether a file was submitted.
- Reports are classified as Could because the core workflow can operate without advanced reporting in the first baseline.

## Deferred Requirements

- Automatic plagiarism detection is not included in the current baseline.
- Real-time chat is not included in the current baseline.
- Detailed analytics dashboards are deferred until basic reports are validated.

## Quality Check Result

Passed. All functional requirements are prioritized and decision rationale is documented.
