# 01 - Project Inception and Stakeholder Discovery

## Business Problem

The campus needs a centralized assignment management system that helps lecturers, students, and administrators manage academic assignments consistently. Without a dedicated system, assignment instructions, deadlines, submissions, grades, and feedback can become scattered, which may cause missed deadlines, unclear submission status, and inefficient grading workflows.

The core problem is not only technical. It is a coordination and information management problem involving lecturers who assign and grade work, students who submit work, and administrators who maintain users, courses, and system configuration.

## Project Goals

- Provide a centralized place for lecturers to create assignments and manage deadlines.
- Allow students to view assignments, submit files, and monitor status.
- Support grading and feedback for submitted assignments.
- Allow administrators to manage users, courses, and system configuration.
- Improve usability, security, performance, reliability, and data integrity.

## Stakeholders

| Stakeholder | Type | Role |
|---|---|---|
| Lecturer | Primary | Creates assignments, reviews submissions, gives grades and feedback. |
| Student | Primary | Views assignments, submits files, tracks status and deadlines. |
| Administrator | Primary | Manages users, courses, roles, and system settings. |
| Academic Department | Secondary | Reviews assignment completion and grading progress. |
| IT Support | Secondary | Maintains system reliability, security, and troubleshooting. |

## Stakeholder Needs

| Stakeholder | Needs |
|---|---|
| Lecturer | Create assignments, set deadlines, view submissions, grade work, provide feedback, identify missing submissions. |
| Student | View assigned tasks, understand deadlines, upload files, receive submission confirmation, view grades and feedback. |
| Administrator | Manage users, roles, courses, lecturer-course assignments, student-course enrollments, and system configuration. |
| Academic Department | Access basic reports about assignment and grading progress. |
| IT Support | Maintain secure, reliable, and auditable system operation. |

## Scope

### In Scope

- Assignment creation
- Deadline management
- Assignment viewing
- File submission
- Submission status tracking
- Grade and feedback management
- User and role management
- Course management
- Basic assignment activity reports
- Authentication and role-based access

### Out of Scope

- Real-time chat
- Online video lectures
- Automatic plagiarism detection
- Payment or finance features
- Full learning management system replacement

## Assumptions

- ASSUMPTION-01: The application is web-based.
- ASSUMPTION-02: Every user must log in before accessing system features.
- ASSUMPTION-03: The system uses lecturer, student, and administrator roles.
- ASSUMPTION-04: Students submit assignments by uploading files.
- ASSUMPTION-05: Uploaded files must be stored securely.

## Constraints

- The system must protect student academic data.
- Requirements must be testable and traceable.
- Submission data must not be lost or modified without authorization.
- Unsupported assumptions must be labeled explicitly.

## Open Questions

- OPEN QUESTION: What file types and maximum file sizes are allowed?
- OPEN QUESTION: Should students be allowed to resubmit before the deadline?
- OPEN QUESTION: Should late submissions be blocked or accepted with a late label?
- OPEN QUESTION: What detailed reports are required by academic departments?

## Quality Check Result

Passed. The business problem, stakeholders, scope, assumptions, constraints, and open questions are separated clearly.
