# 📋 Software Project Documentation Skill

An [Agent Skill](https://code.claude.com/docs/en/skills) for discovering, analyzing, estimating, and documenting software products and client projects. 🚀

The skill acts as a product discovery partner, business analyst, and technical documentation assistant. It guides you from an early-stage idea or client brief to a clear, testable, internally consistent documentation set — without inventing facts along the way.

## 🎯 What it produces

Working with you, one question at a time, the skill can build and maintain:

| Document | Purpose |
|---|---|
| 📝 Product Requirements Document | Problem, goals, users, scope, and workflows |
| ✅ Functional Requirements | Testable requirements with stable IDs (`FR-001`) |
| 📊 Non-Functional Requirements | Measurable quality targets (security, performance, availability…) |
| 🏗️ C4 Architecture | System context, containers, and data flows |
| 🗄️ Database Model | Entities, relationships, constraints, and trade-offs |
| 💰 Budget and Estimation | Effort and cost ranges with stated assumptions |

## ⚙️ Requirements

- A coding agent that supports the Agent Skills convention (`SKILL.md`), such as **Claude Code**, **OpenCode**, or **Cursor**
- Git (to clone the repository)

## 📥 Installation

The skill is a folder containing `SKILL.md` plus reference templates. Pick the location matching your agent and scope — personal (all your projects) 🌐 or project-level (shared with the team) 🤝.

### 🤖 Claude Code

```sh
# 👤 Personal (all your projects)
git clone https://github.com/Abo3baziz/software-project-documentation.git ~/.claude/skills/software-project-documentation

# 📁 Project-level (inside your project's root)
git clone https://github.com/Abo3baziz/software-project-documentation.git .claude/skills/software-project-documentation
```

### ⌨️ OpenCode

```sh
# 🌐 Global
git clone https://github.com/Abo3baziz/software-project-documentation.git ~/.config/opencode/skills/software-project-documentation

# 📁 Project-level (inside your project's root)
git clone https://github.com/Abo3baziz/software-project-documentation.git .opencode/skills/software-project-documentation
```

### 🖱️ Cursor

```sh
# 👤 User-level
git clone https://github.com/Abo3baziz/software-project-documentation.git ~/.cursor/skills/software-project-documentation

# 📁 Project-level (inside your project's root)
git clone https://github.com/Abo3baziz/software-project-documentation.git .cursor/skills/software-project-documentation
```

### 🔗 Other agents

Many agents (including OpenAI Codex, Cursor, and OpenCode) also read the shared `.agents/skills/` convention, which keeps one copy working across several tools:

```sh
git clone https://github.com/Abo3baziz/software-project-documentation.git .agents/skills/software-project-documentation
```

If your agent uses a different skills directory, clone (or copy) the folder there — just make sure `SKILL.md` sits at the root of the `software-project-documentation` folder. Check your agent's documentation for its supported location.

### 🔍 Verify it's installed

Start a new agent session in any project and ask something like *"What are your available skills?"* — `software-project-documentation` should be listed. In OpenCode you can also load it directly by mentioning `@software-project-documentation` in your prompt.

### 🔄 Update

Since the skill is a git clone, updating is just:

```sh
git -C <skills-dir>/software-project-documentation pull
```

### 📦 Manual install (no Git)

Download the repository ZIP from GitHub, extract it, and copy the `software-project-documentation` folder into your agent's skills directory.

## 💬 Usage

Ask your agent things like:

- "I have a new SaaS idea. Help me document it."
- "Interview me about this client's project and build the PRD."
- "Turn these notes into functional requirements."
- "Review the architecture and database model for inconsistencies."
- "Update the budget after this scope change."

The skill is designed to:

- ❓ **Ask one question at a time** instead of dumping a questionnaire on you.
- 🏷️ **Distinguish facts from assumptions.** Everything is labeled *Confirmed*, *Assumption*, *Recommendation*, *Open question*, or *Decision* — nothing is silently invented.
- 🧱 **Build documentation progressively**, starting with discovery before any solution or technology choices.
- 🔁 **Keep documents synchronized.** When a requirement changes, it identifies every affected document and updates them consistently.
- ⚠️ **Never present estimates as quotes.** Budgets always state assumptions, exclusions, uncertainty, and confidence.

## 📂 What's inside

```text
software-project-documentation/
├── SKILL.md           # 🧠 The skill's instructions and 7-stage workflow
├── README.md
└── references/
    ├── prd-template.md
    ├── functional-requirements-template.md
    ├── non-functional-requirements-template.md
    ├── budget-template.md
    ├── c4-architecture-template.md
    ├── database-model-template.md
    └── documentation-conventions.md
```

## 🛠️ How it works

The skill follows a seven-stage workflow:

1. 🧭 **Understand the engagement** — new product, client project, existing product, or a change to documented work.
2. 🔍 **Product discovery** — problem, users, journeys, business rules, constraints, and MVP boundaries.
3. 📝 **Create the PRD** — what and why, without prescribing implementation.
4. ✅ **Define requirements** — functional and non-functional, with stable IDs and testable language.
5. 🏗️ **Architecture and data model** — C4 diagrams and database entities derived from real workflows.
6. 💰 **Estimate budget and effort** — broken down by deliverable, with ranges and stated assumptions.
7. 🔎 **Review and maintain** — consistency checks across the whole documentation set, and impact-aware updates when scope changes.
