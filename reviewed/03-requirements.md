# 03 - Requirements

## Functional Requirements

| ID | Requirement | Source |
|---|---|---|
| FR-01 | The system shall allow lecturers to create assignments with title, description, course, deadline, and submission instructions. | EL-01, EL-02 |
| FR-02 | The system shall allow lecturers to edit assignment details before the deadline. | EL-01, EL-02 |
| FR-03 | The system shall display active assignments to students enrolled in the related course. | EL-06 |
| FR-04 | The system shall allow students to upload assignment submission files for active assignments. | EL-08 |
| FR-05 | The system shall display a submission confirmation with submission status and timestamp after a successful upload. | EL-09 |
| FR-06 | The system shall allow students to view assignment deadline status as open, submitted, late, or closed. | EL-07 |
| FR-07 | The system shall allow lecturers to view submitted assignment files by course and assignment. | EL-03 |
| FR-08 | The system shall allow lecturers to enter grades and written feedback for student submissions. | EL-04 |
| FR-09 | The system shall allow students to view published grades and feedback for their own submissions. | EL-10 |
| FR-10 | The system shall allow administrators to create, update, deactivate, and assign user roles. | EL-11 |
| FR-11 | The system shall allow administrators to create, update, and archive course records. | EL-12 |
| FR-12 | The system shall provide assignment activity reports showing assignment count, submission count, missing submissions, and grading status. | EL-13, EL-05 |

## Non-Functional Requirements

| ID | Requirement | Measurement |
|---|---|---|
| NFR-01 | The system shall load the student assignment dashboard within 3 seconds under normal campus network conditions. | Response time <= 3 seconds |
| NFR-02 | The system shall restrict lecturer, student, and administrator features based on authenticated role permissions. | 100% role-based access test cases pass |
| NFR-03 | The system shall store submission records with timestamp and user ID to support data integrity. | Every submission record has timestamp and user ID |
| NFR-04 | The system shall maintain 99% monthly availability during academic assignment periods. | Availability >= 99% per month |
| NFR-05 | The system shall prevent students from viewing other students' submissions, grades, or feedback. | Unauthorized access test cases fail safely |

## Business Rules

| ID | Rule |
|---|---|
| BR-01 | A student can submit an assignment only if the student is enrolled in the course linked to that assignment. |
| BR-02 | Only the lecturer assigned to a course can grade submissions for assignments in that course. |
| BR-03 | Students can view grades and feedback only after the lecturer publishes them. |

## Assumptions

- ASSUMPTION: Students are already enrolled in courses before assignments are distributed.
- ASSUMPTION: Assignment upload uses file submission, not text-only submission.
- ASSUMPTION: Late submissions are allowed but marked as late unless future policy rejects them.

## Open Questions

- OPEN QUESTION: What is the maximum upload file size?
- OPEN QUESTION: Which file formats are allowed?
- OPEN QUESTION: Should students be allowed to resubmit before the deadline?

## Quality Check Result

Passed. Requirements are separated into functional, non-functional, and business rules. Ambiguous terms were replaced with measurable criteria where needed.
