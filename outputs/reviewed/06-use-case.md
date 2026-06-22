# 06 - Use Case

## Actors

- Lecturer
- Student
- Administrator

## Use Cases

| ID | Use Case | Actor | Description |
|---|---|---|---|
| UC-01 | Create Assignment | Lecturer | Lecturer creates an assignment for a course. |
| UC-02 | View Submissions | Lecturer | Lecturer views submitted student files. |
| UC-03 | Grade Submission | Lecturer | Lecturer enters grade and feedback. |
| UC-04 | View Assignment | Student | Student views active assignments and deadlines. |
| UC-05 | Submit Assignment | Student | Student uploads an assignment file. |
| UC-06 | View Grade and Feedback | Student | Student views published grade and feedback. |
| UC-07 | Manage Users | Administrator | Administrator manages users and roles. |
| UC-08 | Manage Courses | Administrator | Administrator manages course records. |
| UC-09 | View Reports | Administrator | Administrator views assignment activity reports. |

## Use Case Diagram

The diagram source is available in:

- `diagrams/use-case-diagram.png`
- `diagrams/use-case-diagram.drawio`
- `diagrams/use-case-diagram.mmd`

## Brief Use Case Descriptions

### UC-01 Create Assignment

Lecturer enters assignment title, description, course, deadline, and instructions. The system validates and saves the assignment.

### UC-05 Submit Assignment

Student opens an active assignment, uploads a valid file, and receives confirmation with timestamp.

### UC-07 Manage Users

Administrator creates, updates, deactivates users, and assigns roles.

## Quality Check Result

Passed. The use case list includes at least three actors and more than six use cases.
