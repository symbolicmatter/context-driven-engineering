# AGENTS.md  
## Operating Rules for AI Coding Agents

This document defines how AI coding agents are expected to operate in this repository.
It is normative, not advisory.

If instructions conflict, escalate by asking questions. Do not guess.

---

## 1. Purpose

AI agents in this project exist to **execute intent**, not to invent direction.

All code, structure, and behavior must be derived from the documented context.
Context is authoritative. Code is secondary.

---

## 2. Context Hierarchy (Read Order)

Before writing or modifying code, read documents in this order:

1. VISION.md  
2. PRODUCT.md  
3. DOMAIN.md
4. DESIGN_WORLDVIEW.md (if present)  
5. ARCHITECTURE.md
6. CONTEXT.md
7. SPEC.md or the relevant spec in `specs/`  
8. UX_GUIDELINES.md (if relevant)  
9. CONTRIBUTING.md  

If any document is missing or ambiguous, stop and ask.

---

## 3. Design Worldview Enforcement

This project declares a design worldview in DESIGN_WORLDVIEW.md.

When present, this worldview is **binding**.

For Object-Centric Design specifically, agents must:

- Propose objects, not services or procedural modules
- Place behavior with the object that owns the responsibility
- Prefer message-sending over data access
- Avoid central orchestration logic
- Challenge anemic domain models explicitly

If an architectural pattern conflicts with object responsibilities, **preserve responsibilities**.

---

## 4. Spec-Driven Behavior

Specifications define **behavioral contracts**, not implementation steps.

When implementing a SPEC:

- Treat the spec as a contract
- Do not invent additional behavior
- Do not omit edge cases
- Reflect state changes explicitly in code

If the spec is incomplete or underspecified, ask for clarification before proceeding.

---

## 5. What You May NOT Do

AI agents must not:

- Introduce new architectural layers without justification
- Refactor structure for aesthetic or stylistic reasons
- Replace object collaboration with service abstractions
- Introduce frameworks or libraries not mentioned in ARCHITECTURE.md
- “Improve” designs by centralizing logic

Optimization without explicit intent is considered a defect.

---

## 6. Asking Questions Is a Feature

Stopping to ask a question is preferred over guessing.

Ask questions when:

- Responsibilities are unclear
- Object boundaries feel forced
- A spec contradicts the design worldview
- Architectural trade-offs are implicit rather than stated

Phrase questions in terms of responsibilities and intent, not implementation.

---

## 7. Incremental Work Discipline

Work in small, reviewable steps.

After each significant change:

- Verify alignment with SPEC
- Verify alignment with DESIGN_WORLDVIEW
- Note any assumptions made

Large, sweeping changes without checkpoints are discouraged.

---

## 8. Definition of Done (for Agents)

Work is considered complete when:

- Behavior matches the SPEC
- Design aligns with the declared worldview
- No undocumented assumptions remain
- Code structure reflects responsibilities, not convenience

If these conditions cannot be met, stop and report why.

---

## 9. Final Rule

When in doubt, prioritize:

1. Conceptual integrity
2. Responsibility ownership
3. Behavioral clarity

Structure follows understanding.