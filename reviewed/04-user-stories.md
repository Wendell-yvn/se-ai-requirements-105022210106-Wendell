# 04 - User Stories and Acceptance Criteria

## User Stories

| ID | User Story | Related FR |
|---|---|---|
| US-01 | As a lecturer, I want to create assignments for my course so that students receive clear task instructions and deadlines. | FR-01 |
| US-02 | As a lecturer, I want to view submitted files so that I can review student work. | FR-07 |
| US-03 | As a lecturer, I want to enter grades and feedback so that students can understand their performance. | FR-08 |
| US-04 | As a student, I want to view active assignments so that I know what tasks I must complete. | FR-03 |
| US-05 | As a student, I want to upload my assignment file so that I can submit my work through the system. | FR-04, FR-05 |
| US-06 | As a student, I want to view my assignment status, grade, and feedback so that I can monitor my academic progress. | FR-06, FR-09 |
| US-07 | As an administrator, I want to manage users and roles so that system access is controlled correctly. | FR-10 |
| US-08 | As an administrator, I want to manage courses and view assignment reports so that academic operations can be monitored. | FR-11, FR-12 |

## Acceptance Criteria

| ID | User Story | Acceptance Criteria |
|---|---|---|
| AC-01 | US-01 | Given a lecturer is logged in, when the lecturer enters title, description, course, deadline, and instructions, then the system saves the assignment. |
| AC-02 | US-01 | Given required assignment fields are missing, when the lecturer submits the form, then the system displays validation errors and does not save the assignment. |
| AC-03 | US-02 | Given a lecturer opens an assignment, when submissions exist, then the system displays the submitted files by student. |
| AC-04 | US-02 | Given no student has submitted, when the lecturer opens submissions, then the system displays an empty submission message. |
| AC-05 | US-03 | Given a submission exists, when the lecturer enters grade and feedback, then the system saves the assessment record. |
| AC-06 | US-03 | Given a grade is outside the allowed score range, when the lecturer saves it, then the system rejects the grade and shows an error. |
| AC-07 | US-04 | Given a student is enrolled in a course, when the student opens the dashboard, then active assignments for that course are displayed. |
| AC-08 | US-04 | Given an assignment is closed, when the student opens active assignments, then the closed assignment is not shown as active. |
| AC-09 | US-05 | Given an assignment is open, when the student uploads a valid file, then the system stores the file and shows confirmation with timestamp. |
| AC-10 | US-05 | Given the upload fails, when the student submits a file, then the system shows an error and does not mark the assignment as submitted. |
| AC-11 | US-06 | Given a student submitted an assignment, when the student views status, then the system shows submitted, late, open, or closed status. |
| AC-12 | US-06 | Given the lecturer has published grades, when the student opens the assignment result, then grade and feedback are displayed. |
| AC-13 | US-07 | Given an administrator is logged in, when the administrator creates or updates a user, then the system saves the user record with role information. |
| AC-14 | US-07 | Given a non-administrator tries to manage users, when the user accesses user management, then access is denied. |
| AC-15 | US-08 | Given an administrator creates or updates a course, when required data is valid, then the system saves the course record. |
| AC-16 | US-08 | Given assignment activity exists, when the administrator opens reports, then assignment count, submission count, missing submissions, and grading status are displayed. |

## Quality Check Result

Passed. Each user story follows the required format and has at least two testable acceptance criteria.
