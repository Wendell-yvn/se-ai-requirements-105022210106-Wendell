# Requirements Elaboration and Specification

## Purpose

Transform elicitation findings into functional requirements, non-functional requirements, business rules, user stories, and acceptance criteria.

## When to Use

Use this skill after elicitation findings have been reviewed.

## Inputs

- `CASE.md`
- `outputs/reviewed/01-inception.md`
- `outputs/reviewed/02-elicitation.md`
- `inputs/assumptions.md`

## Required Context

The AI must read the case, inception output, elicitation output, and assumptions. It must use requirement IDs and preserve traceability to elicitation source IDs.

## Workflow

1. Extract candidate requirements from elicitation findings.
2. Write functional requirements using IDs `FR-01`, `FR-02`, and so on.
3. Write non-functional requirements using IDs `NFR-01`, `NFR-02`, and so on.
4. Write business rules using IDs `BR-01`, `BR-02`, and so on.
5. Create user stories using IDs `US-01`, `US-02`, and so on.
6. Create at least two acceptance criteria for each user story using IDs `AC-01`, `AC-02`, and so on.
7. Ensure every requirement is clear, testable, and traceable.
8. Identify assumptions and open questions.
9. Run quality checks.

## Output Format

Create two Markdown outputs:

1. `outputs/reviewed/03-requirements.md`
2. `outputs/reviewed/04-user-stories.md`

The requirements document must include:

- Functional Requirements
- Non-Functional Requirements
- Business Rules
- Assumptions
- Open Questions
- Quality Check Result

The user stories document must include:

- User Stories
- Acceptance Criteria
- Traceability to Functional Requirements

## Rules

- Do not use vague words such as fast, easy, secure, or reliable without measurable criteria.
- Do not create unsupported features.
- Separate functional and non-functional requirements.
- Each functional requirement must have a source.
- Each user story must follow: `As a [role], I want [goal], so that [benefit].`
- Each acceptance criterion must be testable.

## Quality Checks

- At least 8 functional requirements exist.
- At least 4 measurable non-functional requirements exist.
- At least 2 business rules exist.
- At least 6 user stories exist.
- Each user story has at least 2 acceptance criteria.
- Requirements are not duplicated.
- Requirements are traceable to elicitation findings.

## Failure Conditions

Stop and ask for clarification if:

- Elicitation findings are missing.
- Requirements cannot be traced to sources.
- A requirement is not testable and cannot be improved from available context.

## Example Invocation

Read `CASE.md`, `outputs/reviewed/01-inception.md`, and `outputs/reviewed/02-elicitation.md`. Execute `skills/03-specification/SKILL.md`. Save raw output to `outputs/raw/requirements-ai-output.md`.

## Expected Output Example

```markdown
FR-01: The system shall allow lecturers to create assignments for courses they are assigned to.
Source: EL-01
```
