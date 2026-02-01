# Example Templates for Context-Driven Engineering (CDE)

This document provides **example templates** for documents commonly used in Context-Driven Engineering (CDE).

The templates are intentionally concise and structured. They are meant to:

- Make intent explicit
- Reduce ambiguity for humans and AI agents
- Encourage disciplined thinking without over-specification

They are inspired by the *Four-Document Pattern* from the ContextFlow repository, adapted to the broader and more flexible scope of CDE.

These templates are illustrative, not normative.

They demonstrate one coherent way of externalizing context in written form.
Projects applying CDE are expected to adapt, omit, or restructure these documents
based on their needs and constraints.

## VISION.md

**Purpose:** Direction, ambition, long-term intent

### What problem are we ultimately trying to solve?

Describe the fundamental problem or opportunity this product exists to address. Focus on *why this matters*, not on features or solutions.

### For whom does this exist?

Describe the primary users or stakeholders at a high level. Avoid personas here, focus on strategic audience definition.

### What does success look like?

Describe the desired future state if this product succeeds. This may include qualitative outcomes, not metrics.

### Non-goals

Explicitly state what this product is **not** trying to do, even if those things seem adjacent or tempting.

## PRODUCT.md

**Purpose:** Problem framing, value, scope

### Problem statement

Describe the concrete problem(s) users experience today. Anchor this in observable pain, friction, or missed opportunity.

### Target users

List and briefly describe the key user groups. Personas may be referenced but not fully elaborated here.

### Value proposition

Explain how the product meaningfully improves the user’s situation. Focus on outcomes, not implementation.

### Scope and boundaries

Clarify what is included in the product and what is explicitly out of scope.

## DOMAIN.md

**Purpose:** Domain language, meaning, invariants

### Domain overview

Describe the domain in plain language. What kind of world does this system model or interact with?

### Core concepts

List and define the key domain concepts. Use domain language, not technical abstractions.

- Concept name

  - Description
  - Key distinctions or nuances

### Invariants and rules

Describe rules that must always hold true within the domain, regardless of implementation.

### Terminology glossary

Provide authoritative definitions for important terms used across all documents.

## CONTEXT.md

**Purpose:** Constraints, assumptions, environment

### Organizational context

Describe relevant organizational factors such as team structure, decision-making constraints, or governance.

### Technical context

List existing systems, platforms, or constraints that shape design decisions.

### Operational constraints

Describe non-functional constraints such as performance expectations, budgets, timelines, or regulatory factors.

### Assumptions and trade-offs

Explicitly state assumptions being made and the trade-offs they imply.

## ARCHITECTURE.md

**Purpose:** Technical structure and design decisions

### Architectural overview

Describe the overall structure of the system and its major components or subsystems.

### Key design decisions

Document important architectural choices and why they were made.

### Data and state

Describe how data and state are represented, owned, and evolved.

### Integration points

List external systems, APIs, or interfaces the system interacts with.

## UX_GUIDELINES.md

**Purpose:** Interaction principles and semantics

### UX principles

Describe guiding principles for user experience and interaction design.

### Interaction patterns

Document standard interaction patterns to be reused across the product.

### Accessibility and usability considerations

List accessibility goals and usability constraints.

## SPEC.md (or specs/*.md)

**Purpose:** Behavioral contracts

### Feature summary

Briefly describe the feature or capability.

### Behavioral requirements

Describe expected behavior, inputs, outputs, and state changes.

### Edge cases and failure modes

List edge cases, invalid inputs, and error conditions.

### Acceptance criteria

Define conditions under which the feature is considered correct.

## PLAN.md

**Purpose:** Sequencing and delivery intent

### Milestones

Outline major milestones or phases.

### Dependencies

List dependencies between features, teams, or systems.

### Risks and mitigations

Identify known risks and how they are being managed.

## AGENTS.md

**Purpose:** AI agent operating rules

### Role of AI agents

Describe what AI agents are expected to do and not do.

### Context usage rules

Specify which documents are authoritative and in what order they should be consulted.

### Behavioral constraints

List design and implementation constraints AI agents must respect.

### Escalation and uncertainty handling

Describe when agents should stop and ask questions.

## CONTRIBUTING.md

**Purpose:** Contribution and quality rules

### Contribution scope

Describe what kinds of contributions are welcome.

### Review expectations

Explain how changes are reviewed and accepted.

### Quality bar

Define expectations for clarity, consistency, and intent.

## Notes on Use

- Not all projects need all documents from day one.
- Documents should be added as the need for explicit context arises.
- Brevity and clarity are preferred over completeness.
- When in doubt, make assumptions explicit rather than implicit.
