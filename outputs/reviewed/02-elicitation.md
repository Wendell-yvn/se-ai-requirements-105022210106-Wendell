# 02 - Requirements Elicitation

## Elicitation Objectives

- Understand assignment management needs from lecturers, students, and administrators.
- Identify explicit and implicit needs from stakeholder notes and interview answers.
- Prepare findings that can be transformed into traceable requirements.

## Elicitation Techniques

| Technique | Purpose |
|---|---|
| Stakeholder Interview | Gather direct needs from lecturers, students, and administrators. |
| Document Analysis | Analyze case description, stakeholder notes, and assumptions. |
| Scenario Analysis | Understand how users interact with assignments from creation to grading. |
| Requirements Workshop | Resolve conflicts between submission flexibility, grading control, and administration needs. |

## Stakeholder Interview Questions

### Lecturer

1. What information must be included when creating an assignment?
2. How should deadlines be displayed and enforced?
3. How do you want to review submitted files?
4. What grading and feedback information must be recorded?
5. How should missing or late submissions be shown?

### Student

1. What assignment information do you need to see first?
2. What confirmation do you need after submitting a file?
3. How should the system show assignment status?
4. What grade and feedback information should be visible?
5. What problems do you experience when submitting near a deadline?

### Administrator

1. What user data must be managed?
2. What course data must be managed?
3. How should user roles be assigned?
4. What reports are needed?
5. What system settings should be configurable?

## Elicitation Findings

| ID | Stakeholder | Finding | Source |
|---|---|---|---|
| EL-01 | Lecturer | Lecturers need to create assignments for specific courses. | interview-answers.md |
| EL-02 | Lecturer | Lecturers need to set assignment deadlines. | interview-answers.md |
| EL-03 | Lecturer | Lecturers need to view student submissions. | stakeholder-notes.md |
| EL-04 | Lecturer | Lecturers need to enter grades and written feedback. | interview-answers.md |
| EL-05 | Lecturer | Lecturers need to identify students who have not submitted. | stakeholder-notes.md |
| EL-06 | Student | Students need to view active assignments. | interview-answers.md |
| EL-07 | Student | Students need to see assignment deadlines and status. | interview-answers.md |
| EL-08 | Student | Students need to upload assignment files. | interview-answers.md |
| EL-09 | Student | Students need confirmation after successful submission. | interview-answers.md |
| EL-10 | Student | Students need to view grades and feedback. | interview-answers.md |
| EL-11 | Administrator | Administrators need to manage users and roles. | interview-answers.md |
| EL-12 | Administrator | Administrators need to manage courses. | interview-answers.md |
| EL-13 | Administrator | Administrators need reports about assignment activity. | interview-answers.md |

## Explicit Needs

- Assignment creation by lecturers.
- Deadline management.
- Student file submission.
- Submission status tracking.
- Grade and feedback management.
- User, role, and course management.
- Assignment activity reporting.

## Implicit Needs and Assumptions

- ASSUMPTION: Authentication is required because different stakeholders have different permissions.
- ASSUMPTION: Submission confirmation should include timestamp information.
- ASSUMPTION: Administrators can manage course and user data but cannot grade student submissions.

## Open Questions

- OPEN QUESTION: Should late submissions be rejected or accepted with a late status?
- OPEN QUESTION: What file types and file sizes should be accepted?
- OPEN QUESTION: Should grade publication require a separate lecturer action?

## Quality Check Result

Passed. Each finding has a stakeholder and source ID. Explicit needs, assumptions, and open questions are separated.
