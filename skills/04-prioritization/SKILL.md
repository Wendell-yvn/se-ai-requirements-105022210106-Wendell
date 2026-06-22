# Negotiation and Prioritization

## Purpose

Prioritize functional requirements using MoSCoW and document stakeholder conflicts, dependencies, trade-offs, and decision rationale.

## When to Use

Use this skill after requirements and user stories are drafted and reviewed.

## Inputs

- `outputs/reviewed/03-requirements.md`
- `outputs/reviewed/04-user-stories.md`
- `outputs/reviewed/02-elicitation.md`

## Required Context

The AI must read requirements, user stories, and elicitation findings. It must prioritize only existing functional requirements.

## Workflow

1. List all functional requirements.
2. Identify stakeholder value for each requirement.
3. Identify dependencies between requirements.
4. Identify possible stakeholder conflicts.
5. Assign MoSCoW priority: Must, Should, Could, or Won't.
6. Explain trade-offs and decision rationale.
7. Identify requirements that need negotiation.
8. Run quality checks.

## Output Format

Create a Markdown document with these sections:

1. Prioritization Method
2. Requirement Priority Table
3. Stakeholder Conflicts
4. Dependencies
5. Trade-Off Decisions
6. Deferred Requirements
7. Quality Check Result

## Rules

- Do not prioritize requirements that do not exist.
- Every functional requirement must receive one MoSCoW priority.
- Every priority must include a reason.
- Conflicts must identify affected stakeholders.
- Dependencies must reference requirement IDs.

## Quality Checks

- All functional requirements are prioritized.
- Must-have requirements are justified by core business value.
- Dependencies are not contradictory.
- Trade-offs are documented.
- Deferred items have reasons.

## Failure Conditions

Stop and ask for clarification if:

- Functional requirements are missing.
- Priorities cannot be justified.
- Two requirements conflict and no decision can be made from available context.

## Example Invocation

Read `outputs/reviewed/03-requirements.md` and `outputs/reviewed/04-user-stories.md`. Execute `skills/04-prioritization/SKILL.md`. Save raw output to `outputs/raw/prioritization-ai-output.md`.

## Expected Output Example

```markdown
| Requirement | Priority | Reason |
|---|---|---|
| FR-01 | Must | Assignment creation is required before students can submit work. |
```
