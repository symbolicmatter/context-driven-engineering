# Context-Driven Engineering

![Living Document](https://img.shields.io/badge/Status-Living%20Document-blue?style=for-the-badge) [![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-orange?style=for-the-badge)](./LICENSE)

Context-Driven Engineering (CDE) is an approach to software development that treats **context as the primary artifact** and code as a secondary, derived outcome.

In CDE, vision, specifications, architecture, and design constraints are made explicit, kept coherent, and used directly by both humans and AI coding agents.

This repository serves as a **conceptual reference and school of thought** for Context-Driven Engineering (CDE).

<br>

<img src="assets/cde-authority-flow.jpg"
     alt="Conceptual authority flow in Context-Driven Engineering"
     width="650">

---

## How to read this (especially for first-time readers)

This repository describes Context-Driven Engineering (CDE) as a general approach. It does not apply CDE to itself.

In this repository, AI agents are discussed conceptually. Operational agent instructions belong to applied CDE projects and worked examples. Worked examples and applied practices live elsewhere (for example in `example-domain/` or related repositories).

It is intentionally broader and more opinionated than what most teams would adopt at once.

When engaging with CDE in exploratory or pilot contexts (for example within an existing organization):

- CDE does not require all context to be externalized at once.
- Partial engagement is possible, provided that any explicitly captured context is treated coherently.
- This repository intentionally focuses on the mental model and document relationships, not on a finished example domain.

The goal is not methodological purity, but learning how explicit, coherent context
changes the quality and reliability of AI-assisted development in real projects.

## Contents

- [How to read this (especially for first-time readers)](#how-to-read-this-especially-for-first-time-readers)
- [Contents](#contents)
- [Why Context-Driven Engineering?](#why-context-driven-engineering)
- [Isn’t this just a lot of upfront specification?](#isnt-this-just-a-lot-of-upfront-specification)
- [What This Repository Contains](#what-this-repository-contains)
- [From Concept to Practice](#from-concept-to-practice)
- [Who This Is For](#who-this-is-for)
- [Status](#status)
- [License](#license)
- [Stewardship](#stewardship)

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

## *Isn’t this just a lot of upfront specification?*

A common concern when first encountering Context-Driven Engineering is that it appears to require a large amount of upfront specification before any code can be written — similar to traditional outsourcing or forms of “big design up front”.

That is **not** the intent.

CDE does not aim to fully specify a system before development starts. Instead, it makes **design intent explicit at the moment it becomes relevant**, rather than leaving it implicit in code, conventions, or individual developer judgment.

A few important clarifications:

- **Specifications are iterative**, not final contracts.  
    They can start as hypotheses and evolve alongside the code.

- **CDE does not eliminate thinking**, it relocates it.  
    The design decisions you do not write down will still be made — just implicitly, during implementation, reviews, debugging, or refactoring, where they are harder to see and harder to revisit.

- **Context is not written “for the AI”**, but for the project.  
    AI agents are consumers of this context, just like future developers, reviewers, or maintainers.

- **If something is too costly to make explicit**, it is often also too unstable to automate reliably.  
    CDE treats explicit context as a quality filter, not as overhead.

In practice, many teams will find that CDE reduces total effort by:

- lowering rework,
- reducing misalignment,
- and making design discussions more focused and repeatable.

CDE shifts effort from *explaining after the fact* to *deciding with intent* — especially important when code generation itself is no longer the bottleneck.

CDE does not ask you to specify everything upfront — it asks you to stop paying the cost of implicit decisions later.

## What This Repository Contains

- **[docs/CDE.md](./docs/CDE.md)**  
  A concise description of Context-Driven Engineering as a practice.

- **[docs/CDE_EXPLAINED.md](./docs/CDE_EXPLAINED.md)**  
  A deeper explanation of the mental model behind CDE.

- **[docs/DESIGN_WORLDVIEW.md](./docs/DESIGN_WORLDVIEW.md)**  
  An example of an explicit design worldview (Object-Centric Design).
  CDE itself is worldview-agnostic.

- **example-domain/**  
  A placeholder for worked examples applying CDE in practice.  
  Currently contains template-based documents only. *(Work in progress.)*

## From Concept to Practice

This repository describes Context-Driven Engineering (CDE) as a **conceptual framework**, not as a complete operational workflow.

For readers interested in how CDE ideas can be applied concretely in day-to-day AI-assisted development, see:

- **Context-Driven Development Workflow (CDDW)**  
  <https://github.com/symbolicmatter/context-driven-development-workflow>

CDDW is an opinionated, practical workflow that operationalizes CDE principles by treating learning as a first-class artifact and enforcing explicit consolidation over time.

You can engage with CDE without adopting CDDW.
CDDW represents one possible interpretation, not a requirement.

## Who This Is For

This repository is intended for:

- Senior engineers and architects
- Solo builders using AI seriously
- Teams struggling with design drift
- Anyone who suspects that “just generating code faster” is not enough

If you are primarily looking for a framework, this is probably not for you.

## Status

This is a living body of work.

The ideas here are opinionated, incomplete, and evolving.
That is intentional.

This repository has been used as background material in exploratory discussions within organizations.

## License

This work is licensed under the  
**Creative Commons Attribution–NonCommercial–ShareAlike 4.0 International License (CC BY-NC-SA 4.0)**.

You are free to:

- **Share** — copy and redistribute the material in any medium or format  
- **Adapt** — remix, transform, and build upon the material  

Under the following terms:

- **Attribution** — You must give appropriate credit and indicate if changes were made  
- **NonCommercial** — You may not use the material for commercial purposes  
- **ShareAlike** — If you remix, transform, or build upon the material, you must distribute your contributions under the same license  

This license applies to **all conceptual content, documentation, and written material** in this repository unless explicitly stated otherwise.

For the full legal text, see the [`LICENSE`](./LICENSE) file.

## Stewardship

This work is published and maintained by **Symbolic Matter**.

Symbolic Matter is a research-driven studio exploring the intersection of
software design, meaning, and emerging AI-assisted development practices.
