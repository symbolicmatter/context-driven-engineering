# Context-Driven Engineering

Context-Driven Engineering (CDE) is an approach to software development that treats
**context as the primary artifact** and code as a secondary, derived outcome.

In CDE, vision, specifications, architecture, and design constraints are made explicit,
kept coherent, and used directly by both humans and AI coding agents.

This repository serves as a **public reference implementation** of the CDE approach.

---

## Why Context-Driven Engineering?

Modern software development faces a paradox:

- Code is easier to produce than ever
- Understanding what the code *should mean* is harder than ever

AI amplifies this gap.

CDE addresses this by asserting that:

- Code without explicit context is a liability
- AI is only as reliable as the context it operates within
- Design intent must be externalized, not inferred

CDE shifts effort from writing code to **designing intent**.

Without explicit, coherent context, AI accelerates design drift rather than preventing it.
Faster code generation amplifies ambiguity, inconsistency, and misplaced responsibility.

CDE exists to make intent durable in a world where code is cheap.

---

## What This Repository Contains

- **CDE.md**  
  A concise description of Context-Driven Engineering as a practice.

- **CDE_EXPLAINED.md**  
  A deeper explanation of the mental model behind CDE.

- **DESIGN_WORLDVIEW.md**  
  An example of an explicit design worldview (Object-Centric Design).
  CDE itself is worldview-agnostic.

- **AGENTS.md**  
  An operating manual for AI coding agents working in a CDE environment.

- **example-domain/**  
  A small but non-trivial domain demonstrating CDE and object-centric design
  in practice, including real specifications and code.

---

## Who This Is For

This repository is intended for:

- Senior engineers and architects
- Solo builders using AI seriously
- Teams struggling with design drift
- Anyone who suspects that “just generating code faster” is not enough

If you are primarily looking for a framework, this is probably not for you.

---

## Status

This is a living body of work.

The ideas here are opinionated, incomplete, and evolving.
That is intentional.

---

## Stewardship

This work is published and maintained by **Symbolic Matter**.

Symbolic Matter is a research-driven studio exploring the intersection of
software design, meaning, and emerging AI-assisted development practices.
