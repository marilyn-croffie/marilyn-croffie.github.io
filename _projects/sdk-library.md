---
layout: project
title: "Quadrilateral Modeling Library"
context: "Object-Oriented Design • Java Documentation"
role: "Software Engineer & Technical Writer"
stack: "Java, OOP principles, Javadoc, geometric algorithms, technical documentation"
repo: "[https://github.com/yourusername/quadrilateral-modeler](https://github.com/marilyn-croffie/quadrilateral-modeler)"
featured: true
excerpt: "Geometric modeling library with professional-grade Javadoc that doesn't just document the API—it teaches the design decisions, explains the 'why' behind implementation choices, and guides developers through proper usage."
---

## The Assignment

Design a Java library modeling quadrilateral shapes using inheritance. The technical requirements were straightforward: demonstrate OOP principles through a shape hierarchy. But I saw an opportunity to go further: build something robust enough for actual use, and document it thoroughly enough that anyone reading the code would understand not just *what* it does, but *why* it's designed that way.

This became two parallel challenges: defensive programming in the implementation, and pedagogical clarity in the documentation.

## The Engineering: Building It Right

**Defensive Programming**

I wanted this library to be foolproof. Real geometric calculations break in subtle ways—floating-point precision errors, edge cases with collinear points, invalid configurations that naive implementations accept. The validation architecture catches these:

- Input validation at construction time with clear error messages for invalid inputs
- Progressive validation through inheritance (each subclass adds constraints)
- Epsilon-based equality for numerical stability (floating-point comparisons within a tolerance: 1e-9)
- Automatic cyclic point sorting (users don't worry about vertex ordering)
- Immutable Point class (thread-safe, prevents aliasing bugs and state corruption)

**Software Engineering Best Practices**
- Separation of concerns (geometry utils vs shape logic) This separation keeps constructors clean and makes utilities reusable.
- DRY principle (validation chain, not repeated checks)
- Single responsibility (each class has one clear purpose)
- Professional-grade API documentation


## The Documentation: Making It Understandable

Here's where I invested equal effort. The Javadoc isn't just API reference—it's **teaching material**. Anyone reading this code should understand the design rationale, not just function signatures.

**Class-Level Context**

Each class documentation opens with a complete overview: what the class represents, where it fits in the library, and what guarantees it provides (immutability, thread safety, precision handling). This frontloads the conceptual model before diving into individual methods. A developer reading the Point class immediately knows it's immutable, thread-safe, and uses epsilon-based equality—before looking at a single method.

**Design Rationale, Not Just Behavior**

Method documentation explains *why* implementations work the way they do, not just what they return. The equals method doesn't just say "compares two points"—it explains why epsilon-based comparison is necessary for geometric calculations, what problems exact equality would cause, and what tolerance value is used. The hashCode documentation explains the bitwise operations, prime number multipliers, and why this approach follows Java conventions. Someone reading this learns best practices for floating-point equality and hash function design.

**Usage Examples**

Methods include concrete code examples showing proper API usage. These aren't trivial "call this method and get a result" examples—they demonstrate realistic scenarios: creating points via constructor vs factory method, showing that points differing by 1e-10 are considered equal, illustrating how epsilon tolerance prevents false negatives. The examples teach correct usage patterns.

**Implementation Notes**

Complex logic includes explicit implementation notes explaining technical choices. Why use tolerance-based comparison instead of exact equality? Why are coordinates final? Why does the validation chain call super.validateFurther()? These notes make implicit design decisions explicit, turning the codebase into teaching material for object-oriented design patterns.

**Professional Standards Throughout**

- Every public method has complete Javadoc (summary, parameters, return values, exceptions)
- Related methods cross-reference each other using `{@link}` tags
- Technical terms are defined in `{@code}` formatting for clarity
- Examples use `{@code}` blocks with expected output
- Complex concepts have dedicated paragraph tags with bold headings
- Author and version metadata provide attribution

This isn't documentation written to satisfy an assignment requirement. This is professional-grade API documentation that would fit in production codebases.

**Pedagogical Voice**

The documentation voice is instructional. It anticipates confusion ("Why not use exact equality?"), addresses it directly, and explains the reasoning. It teaches geometric programming considerations (floating-point precision matters), Java conventions (how to implement equals and hashCode correctly), and software design patterns (why immutability provides thread safety). The tone assumes the reader wants to understand deeply, not just copy-paste.

## What This Demonstrates

**Dual expertise:** The code demonstrates software engineering (defensive programming, clean architecture, OOP mastery). The documentation demonstrates technical writing (pedagogical clarity, design rationale, usage guidance).

**Documentation as teaching:** The Javadoc doesn't just describe—it explains. It answers "why" alongside "what." It provides context that turns API reference into learning material.

**Professional standards:** This isn't "comments because the assignment required them." This is production-quality documentation where every public method has comprehensive Javadoc, implementation notes explain complex decisions, and usage examples guide proper API use.

**Attention to audience:** The documentation assumes the reader wants to understand, not just use. It teaches geometric programming best practices (epsilon-based equality), Java conventions (hashCode implementation), and API design patterns (factory methods).

**Making implicit knowledge explicit:** Why use epsilon comparison? Why is Point immutable? Why does validation happen in a chain? The documentation makes these design decisions visible and understandable.

## The Balance

This project shows I don't just build things or just document things—I do both with equal rigor. The code is robust and defensively programmed. The documentation is comprehensive and pedagogical. Someone reading this repository learns how to build geometric libraries *and* how to document them professionally.

That's the skillset: technical depth to build it right, and communication clarity to make it understandable. The code works. The documentation teaches. Both matter equally.

This wasn't just "implement inheritance for a grade." This was designing a library with the care and rigor you'd apply to production code—robust validation, clear documentation, thoughtful architecture, and defensive programming throughout.
