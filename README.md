# Software Project Documentation Skill

An Agent Skill for discovering, analyzing, estimating, and documenting software products and client projects.

## Installation

Copy the `software-project-documentation` directory into the skills directory supported by your coding agent. For agents that support the Agent Skills convention, the directory should contain `SKILL.md` at its root.

Example project-local location:

```text
your-project/
└── .agents/
    └── skills/
        └── software-project-documentation/
            ├── SKILL.md
            └── references/
```

The exact skills directory can differ between agents. Check your agent's documentation for its supported location and skill discovery rules.

## Usage

Ask your agent things like:

- "I have a new SaaS idea. Help me document it."
- "Interview me about this client's project and build the PRD."
- "Turn these notes into functional requirements."
- "Review the architecture and database model for inconsistencies."
- "Update the budget after this scope change."

The skill is designed to ask one question at a time, distinguish facts from assumptions, and build documentation progressively.

## Included references

- PRD
- Functional requirements
- Non-functional requirements
- Budget and estimation
- C4 architecture
- Database model
- Shared documentation conventions
