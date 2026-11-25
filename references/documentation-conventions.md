# Documentation Conventions

Use these conventions across project documents unless the user or existing project uses a different standard.

## Information status

- **Confirmed:** explicitly stated or approved.
- **Assumption:** plausible but unverified.
- **Recommendation:** proposed by the analyst/agent; awaiting approval.
- **Open question:** requires clarification.
- **Decision:** explicitly accepted by the user or project stakeholder.
- **Out of scope:** intentionally excluded from the current release.

Never convert one status into another without evidence or approval.

## IDs

Use stable, sequential IDs:
- `GOAL-001` — business/product goals
- `USR-001` — user types or personas
- `UC-001` — use cases or user journeys
- `FR-001` — functional requirements
- `NFR-001` — non-functional requirements
- `BR-001` — business rules
- `INT-001` — integrations
- `RISK-001` — risks
- `DEC-001` — decisions
- `Q-001` — open questions

Do not renumber existing IDs merely to make a list look tidy. Retired IDs should not be reused.

## Priority

Use MoSCoW where helpful:
- **Must:** required for the agreed release to work.
- **Should:** important, but a viable release can ship without it.
- **Could:** useful if time and budget allow.
- **Won't (this release):** explicitly deferred.

Priority is not the same as implementation order.

## Requirement quality

A good requirement is clear, singular, feasible, necessary, and verifiable. Avoid ambiguous words such as "easy", "fast", "secure", "intuitive", and "user-friendly" unless they are defined by measurable criteria.

## Traceability

Where useful, link:
- goals → user journeys → functional requirements,
- functional requirements → business rules and acceptance criteria,
- requirements → architecture elements and data entities,
- scope items → estimates and milestones.

## Change history

For meaningful changes, record date, version, change summary, reason, and approval status. Follow the project's existing versioning convention when present.

## Document quality

- Include document title, project name, status, version, owner, and last-updated date when known.
- Use tables for structured comparisons, not for long narrative explanations.
- Prefer concise, specific language.
- Mark unknown information visibly instead of filling gaps with guesses.
