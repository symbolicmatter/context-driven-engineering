## Object‑Centric Design Worldview

This project deliberately adopts a **Smalltalk‑inspired, message‑centric approach to object‑oriented design**. The intent is not to reproduce Smalltalk as a language, but to apply its underlying worldview when designing, reasoning about, and evolving the system.

This section defines the conceptual frame that both humans and AI coding agents are expected to operate within.

---

## 1. Objects as Lived‑In Abstractions

Objects are **not data structures** and **not service wrappers**. An object represents a *lived‑in abstraction*: a conceptual entity that owns its state, guards its invariants, and decides how to respond to requests.

An object:

* Knows things (state)
* Does things (behavior)
* Decides things (policies, rules, invariants)

Objects are designed to be *mentally inhabitable*. A developer should be able to ask: *“If I were this object, what would I reasonably do when asked this?”*

This perspective deliberately avoids treating objects as passive records manipulated by external logic.

---

## 2. Message‑Centric Interaction

All collaboration happens through **messages**, not direct state access or procedural control.

A message:

* Expresses *intent*, not implementation
* Asks an object to take responsibility for a decision or action
* Does not assume how the receiver fulfils the request

Message sending is preferred over:

* Pulling data out and reasoning elsewhere
* Passing flags or modes
* Coordinating workflows centrally

Late binding is a feature, not a risk. The sender should depend only on the *meaning* of the message, not on the concrete class or structure of the receiver.

---

## 3. Responsibility‑Driven Design (RDD)

Design starts by identifying **responsibilities**, not classes, tables, or APIs.

A responsibility answers one of two questions:

1. *What does this object know?*
2. *What does this object do?*

Responsibilities should be:

* Cohesive and conceptually clear
* Owned by exactly one object
* Expressed in domain language

If a responsibility feels vague, generic, or technical, it is probably misplaced.

---

## 4. Collaboration Over Control Flow

Objects rarely act alone. Meaning emerges from **collaboration**, not orchestration.

Design focuses on:

* Which objects collaborate
* Which messages flow between them
* How responsibilities are distributed

Avoid:

* Central “manager” or “service” objects
* Objects that merely forward calls
* God objects that know too much

Control flow should be an *emergent property* of object interaction, not a predefined script.

---

## 5. CRC Cards as a Design Tool

Class‑Responsibility‑Collaboration (CRC) cards are used as a *thinking aid*, not documentation.

Each CRC card captures:

* The object’s name (in domain language)
* Its responsibilities
* Its collaborators

CRC sessions are conversational and exploratory. They are meant to:

* Surface hidden assumptions
* Expose misplaced responsibilities
* Improve object naming and boundaries

CRC artefacts may be discarded once understanding is achieved.

---

## 6. Designing Before Structuring

Design precedes structure.

Before introducing:

* Packages or modules
* Interfaces or layers
* Framework constructs

We first establish:

* Object identities
* Responsibilities
* Message vocabulary

Code structure should *follow* object design, not drive it.

---

## 7. Guidance for AI Coding Agents

When acting as a coding agent in this project, you are expected to:

* Propose objects, not services or functions
* Introduce behavior alongside state
* Prefer sending messages over accessing data
* Keep objects small, meaningful, and accountable
* Ask clarifying questions when responsibilities are unclear

You should challenge designs that:

* Centralize logic unnecessarily
* Reduce objects to anemic data holders
* Encode workflows procedurally instead of collaboratively

If forced to choose between architectural purity and preserving object responsibilities, **preserve responsibilities**.

---

## 8. Non‑Goals

This project does **not** aim to:

* Mimic classic Smalltalk syntax
* Enforce class hierarchies for their own sake
* Model everything upfront

The goal is **conceptual integrity**, not theoretical perfection.

---

## 9. Object Thinking vs Computer Thinking

This project explicitly favors **object thinking** over **computer thinking**.

Computer thinking frames software as:

* Data structures plus procedures
* Centralized control flow
* Step‑by‑step execution by the machine

Object thinking frames software as:

* A society of autonomous objects
* Each object accountable for its own responsibilities
* Behavior emerging from collaboration

If a design primarily explains *how the computer executes steps*, it is suspect.
If it explains *how domain objects fulfill responsibilities*, it is likely sound.

When in doubt, redesign toward object thinking.

---

## 10. Responsibilities Are Not Functions

A **responsibility is not a function**.

Responsibilities express **expectations from the problem domain**, not implementation mechanics from the solution space.

Guidelines:

* State responsibilities in **active voice** ("validate payment", not "has amount")
* Each object should have **at most 6–7 responsibilities**
* Each object must have **at least one unique responsibility**
* Avoid characteristic‑specific responsibilities ("get age", "report status")

If a responsibility sounds like a getter, setter, or calculation detail, it is probably misplaced.

---

## 11. Behavior First, Data Later

Objects are discovered and defined by **behavior first**.

Do **not** start by listing attributes or data structures.

Only after responsibilities are clear do we decide:

* What the object needs to know
* What knowledge must be retained
* What knowledge can be derived or delegated

Attribute‑first design leads directly to anemic objects and procedural coordination.

---

## 12. Collaboration Is Intrinsic

Collaboration is not accidental wiring. It is part of an object’s intrinsic nature.

If an object consistently needs another object to fulfill a responsibility, that collaboration belongs **inside the encapsulation boundary**.

Excessive indirection, service locators, or orchestration layers are signals that responsibilities may be misplaced.

Coupling is acceptable when it reflects domain necessity.

---

## 13. Anthropomorphism as a Design Aid

Thinking of objects as people is encouraged.

Ask questions like:

* What is this object responsible for?
* What does it reasonably refuse to do?
* What does it need to know to fulfill its obligations?

Anthropomorphism is a cognitive tool to preserve autonomy, accountability, and integrity.

---

## Summary

Think in objects.

Let objects decide.

Distribute responsibilities deliberately.

Let collaboration emerge.

Structure follows understanding.