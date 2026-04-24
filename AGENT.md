# AGENT.md

## Mission
Help build software fast, clearly, and reliably using a structured workflow:
REQ → CONTEXT → STATE → TDD → DESIGN

---

## Source of Truth

- **REQ.md** — defines what we are building and why it matters
- **CONTEXT.md** — explains system structure, tech stack, and global rules
- **STATE.md** — shows current progress, tasks, and next steps
- **TDD.md** — defines how quality is validated through testing
- **DESIGN.md** — defines UI, visual system, and interaction rules

---

## Routing Rules

Every task must be mapped to a document before execution:

- Business goals / product value → update **REQ.md**
- Architecture / constraints / tech decisions → update **CONTEXT.md**
- Progress / tasks / planning → update **STATE.md**
- Testing / bugs / validation → update **TDD.md**
- UI / UX / styling → update **DESIGN.md**

---

## Working Process

1. Read **REQ.md** and **CONTEXT.md** to understand the system
2. Check **STATE.md** for current progress and active tasks
3. Define expected behavior using **TDD.md**
4. Implement the solution
5. Update **STATE.md** with results, blockers, and next steps
6. If UI is affected → update **DESIGN.md**

---

## Quality Rules

- No feature without clear requirements in **REQ.md**
- No architecture changes without updating **CONTEXT.md**
- No task is complete without updating **STATE.md**
- No feature is complete without validation from **TDD.md**

---

## Documentation Rules

- Each file must include:
    - Last updated
    - Owner
    - Status

- Keep content:
    - Short
    - Clear
    - Verifiable

- Avoid duplication across files