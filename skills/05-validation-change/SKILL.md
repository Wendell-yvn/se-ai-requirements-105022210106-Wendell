# Requirements Validation and Change Management

## Purpose

Validate requirements for clarity, completeness, consistency, feasibility, testability, and traceability. Manage requirement changes through impact analysis and decision records.

## When to Use

Use this skill after requirements, user stories, and prioritization have been reviewed.

## Inputs

- `outputs/reviewed/03-requirements.md`
- `outputs/reviewed/04-user-stories.md`
- `outputs/reviewed/05-prioritization.md`
- `outputs/reviewed/requirements-traceability.md`

## Required Context

The AI must read requirements, user stories, prioritization, and traceability matrix. It must validate existing requirements and avoid introducing unsupported features unless recorded as a change request.

## Workflow

1. Select at least five requirements for validation.
2. Check each selected requirement for clarity.
3. Check completeness and consistency.
4. Check feasibility and testability.
5. Check traceability to stakeholder, source, user story, acceptance criteria, and priority.
6. Recommend revisions where needed.
7. Create at least one change request.
8. Analyze impact on requirements, user stories, acceptance criteria, priority, and scope.
9. Record a decision: approve, reject, or defer.
10. Run quality checks.

## Output Format

Create two Markdown outputs:

1. `outputs/reviewed/07-validation.md`
2. `outputs/reviewed/08-change-request.md`

Validation output must include:

- Validation Criteria
- Requirement Validation Table
- Issues Found
- Revisions
- Quality Check Result

Change request output must include:

- Change Request ID
- Description
- Reason
- Affected Requirements
- Impact Analysis
- Decision
- Rationale

## Rules

- Do not approve unclear or untestable requirements.
- Do not add new requirements without change analysis.
- Every validation issue must reference a requirement ID.
- Every change request must have a decision and impact analysis.
- Traceability must be updated if a change is approved.

## Quality Checks

- At least five requirements are validated.
- Every issue has a proposed correction.
- Every correction keeps the requirement testable.
- Change impact is clear.
- Decision rationale is documented.

## Failure Conditions

Stop and ask for clarification if:

- Requirements are missing.
- Traceability data is missing.
- A change request affects scope but no decision authority is identified.

## Example Invocation

Read `outputs/reviewed/03-requirements.md`, `outputs/reviewed/04-user-stories.md`, `outputs/reviewed/05-prioritization.md`, and `outputs/reviewed/requirements-traceability.md`. Execute `skills/05-validation-change/SKILL.md`.

## Expected Output Example

```markdown
CR-01: Allow late submission marking.
Decision: Approved.
Impact: Updates FR-04, US-03, AC-06, and prioritization rationale.
```
