# Requirements Elicitation

## Purpose

Guide AI to plan and document requirements elicitation activities for the Student Task Management System, including elicitation techniques, interview questions, explicit needs, implicit needs, assumptions, and findings.

## When to Use

Use this skill after project inception and stakeholder discovery are complete.

## Inputs

- `CASE.md`
- `outputs/reviewed/01-inception.md`
- `inputs/stakeholder-notes.md`
- `inputs/interview-answers.md`

## Required Context

The AI must read the case, inception output, stakeholder notes, and interview answers. The AI must connect findings to stakeholders and source IDs.

## Workflow

1. Identify suitable elicitation techniques.
2. Create interview questions for lecturer, student, and administrator stakeholders.
3. Extract explicit needs from the input files.
4. Infer possible implicit needs only when supported by input.
5. Label every inferred need as `ASSUMPTION`.
6. Assign elicitation source IDs using `EL-01`, `EL-02`, and so on.
7. Summarize elicitation findings.
8. List unresolved questions.
9. Run quality checks.

## Output Format

Create a Markdown document with these sections:

1. Elicitation Objectives
2. Elicitation Techniques
3. Stakeholder Interview Questions
4. Elicitation Findings
5. Explicit Needs
6. Implicit Needs and Assumptions
7. Open Questions
8. Quality Check Result

## Rules

- Do not create requirements yet unless they are clearly labeled as findings.
- Every finding must have a stakeholder and source ID.
- Do not treat unsupported assumptions as facts.
- Use clear and neutral interview questions.
- Avoid leading questions.

## Quality Checks

- Each major stakeholder has interview questions.
- Findings are linked to stakeholders.
- Explicit and implicit needs are separated.
- Missing information is marked as `OPEN QUESTION`.
- Findings can be used by the specification skill.

## Failure Conditions

Stop and ask for clarification if:

- Inception output is missing.
- Stakeholder input is too limited.
- Interview answers contradict each other and cannot be resolved.

## Example Invocation

Read `CASE.md`, `outputs/reviewed/01-inception.md`, and the input files. Execute `skills/02-elicitation/SKILL.md`. Save the raw output to `outputs/raw/elicitation-ai-output.md`.

## Expected Output Example

```markdown
| ID | Stakeholder | Finding | Source |
|---|---|---|---|
| EL-01 | Lecturer | Lecturers need to create assignments by course. | interview-answers.md |
```
