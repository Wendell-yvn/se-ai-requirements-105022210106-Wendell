# Project Inception and Stakeholder Discovery

## Purpose

Identify the business problem, project goals, stakeholders, scope, assumptions, constraints, and open questions for the Student Task Management System.

## When to Use

Use this skill at the beginning of the requirements engineering process before elicitation, specification, prioritization, validation, or change management.

## Inputs

- `CASE.md`
- `inputs/stakeholder-notes.md`
- `inputs/assumptions.md`

## Required Context

The AI must read the case description, stakeholder notes, and assumptions before generating output. The AI must separate facts from assumptions and must not invent unsupported project details.

## Workflow

1. Summarize the business problem in no more than two paragraphs.
2. Separate the problem from possible solutions.
3. Identify business goals.
4. Identify primary and secondary stakeholders.
5. Describe each stakeholder's needs.
6. Define in-scope and out-of-scope items.
7. Identify assumptions and constraints.
8. Mark missing information as `OPEN QUESTION`.
9. Run quality checks before finalizing the output.

## Output Format

Create a Markdown document with these sections:

1. Business Problem
2. Project Goals
3. Stakeholders
4. Stakeholder Needs
5. Scope
6. Assumptions
7. Constraints
8. Open Questions
9. Quality Check Result

## Rules

- Do not define features before the business problem is understood.
- Do not assume all stakeholders have the same needs.
- Label every assumption with `ASSUMPTION`.
- Label unavailable information with `OPEN QUESTION`.
- Keep scope boundaries clear.

## Quality Checks

- The business problem is not written only as a technical solution.
- Every stakeholder has at least one need.
- Scope includes both in-scope and out-of-scope items.
- Assumptions are separated from facts.
- Goals can be evaluated.

## Failure Conditions

Stop and ask for clarification if:

- The case description is missing.
- Stakeholders cannot be identified.
- Scope is contradictory.
- The AI cannot separate facts from assumptions.

## Example Invocation

Read `CASE.md`, `inputs/stakeholder-notes.md`, and `inputs/assumptions.md`. Execute `skills/01-inception/SKILL.md` exactly as written. Save the raw output to `outputs/raw/inception-ai-output.md`.

## Expected Output Example

```markdown
## Business Problem
Assignment data is scattered across different channels, making it difficult for lecturers and students to track deadlines, submissions, grades, and feedback.

## Stakeholders
- Lecturer: creates assignments, reviews submissions, gives grades.
- Student: views tasks, submits files, monitors status.
```
