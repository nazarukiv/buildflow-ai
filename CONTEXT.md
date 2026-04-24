# CONTEXT.md

## Meta
Last updated: -
Owner: -
Status: active

---

## 1. System Overview

Product domain:
AI-assisted software development workflow system

Architecture:
Document-driven system where each file defines a specific part of development (requirements, state, testing, design)

Core modules:
- Requirements (REQ.md)
- System context (CONTEXT.md)
- Project state (STATE.md)
- Testing rules (TDD.md)
- Design system (DESIGN.md)

---

## 2. Tech Stack

Frontend:
Not defined (system is framework-agnostic)

Backend:
Not defined (can be applied to any stack)

Database:
Not required (file-based system)

Infrastructure:
Local filesystem + Git

CI/CD:
Optional (can integrate later)

---

## 3. Repository Structure

/  
├── AGENT.md  
├── REQ.md  
├── CONTEXT.md  
├── STATE.md  
├── TDD.md  
├── DESIGN.md  
└── README.md

---

## 4. Global Rules

Coding standards:
- Keep code simple and readable
- Prefer clarity over complexity
- Avoid over-engineering

Branching strategy:
- main = stable
- feature branches for changes

Versioning:
- Semantic versioning (optional)

Error handling:
- Fail fast
- Return clear errors

Logging:
- Keep logs simple and useful
- Avoid noise

---

## 5. Domain Model

Entities:
- Document
- Task
- Feature
- Decision

Relationships:
- REQ defines features
- CONTEXT defines structure
- STATE tracks tasks
- TDD validates features
- DESIGN defines UI

Invariants:
- Each document has a clear role
- Documents must stay consistent
- No duplicated logic across files

---

## 6. API / Interfaces

Public:
- Markdown documents used by developers and AI tools

Internal:
- Updates between documents (manual or AI-driven)

Contracts:
- Each document must follow defined structure
- Changes must be reflected across related files

Compatibility:
- Backward compatible changes preferred
- Avoid breaking structure

---

## 7. Data & Storage

Format:
- Markdown (.md)

Storage:
- Local repository

Migration:
- Manual updates

Retention:
- Full history via Git

Backup:
- GitHub / remote repo

---

## 8. Security

Authentication:
Not required

Secrets:
Should not be stored in docs

Data sensitivity:
Low (documentation only)

---

## 9. Performance

Latency:
Instant (local files)

Throughput:
Not applicable

Cost:
Zero (local system)

---

## 10. Architecture Decisions

Decision:
Use document-based system instead of traditional tooling

Reason:
More flexible and AI-friendly

Tradeoff:
Requires discipline to maintain consistency

---

## 11. Dependencies

External:
- Git
- Markdown support
- AI tools (Codex, ChatGPT, Cursor)

Limitations:
- No automation by default
- Manual updates required

---

## 12. Operations

Start:
Open project folder

Build:
Not required

Test:
Follow TDD.md

Deploy:
Push to GitHub

Rollback:
Use Git history