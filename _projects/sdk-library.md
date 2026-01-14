---
layout: project
title: "Quadrilateral Modeling Library"
context: "Object-Oriented Design • Java Documentation"
role: "Software Engineer & Technical Writer"
stack: "Java • OOP principles • Javadoc • Geometric algorithms • Technical documentation • Defensive programming"
repo_label: "GitHub"
repo: "https://github.com/marilyn-croffie/quadrilateral-modeler"
featured: true
order: 5
excerpt: "Geometric modeling library with professional-grade Javadoc that documents the API, teaches the design decisions, explains the 'why' behind implementation choices, and guides developers through proper usage."
---

## The Context
This assignment asked for a Java library modeling quadrilateral shapes using inheritance. The technical requirement was simple: demonstrate OOP principles.

I treated it like a real library.

Instead of optimizing for the assignment, I focused on two things that matter in practice but rarely show up in coursework: defensive engineering and documentation that explains design decisions, not just usage.

## The Work
I designed the library to fail safely and predictably, even in messy real-world scenarios.

Validation happens at construction time, with clear error messages. Constraints are layered through inheritance, so each shape adds its own guarantees. Floating-point comparisons use an epsilon tolerance (1e-9) to avoid precision errors. Vertices are ordered automatically, and the Point class is immutable to prevent state corruption.

I put equal effort into the documentation. The Javadoc is written as teaching material, not just API reference. Class-level comments explain what each abstraction represents and what guarantees it provides. Method documentation explains why decisions were made — especially around floating-point equality, immutability, and validation chains — and includes realistic usage examples rather than trivial calls.

The goal was that anyone reading the code could understand the design without needing me to explain it.

## The Outcome
This project reflects how I approach even small systems: build defensively, document intentionally, and assume the code will be read long after it’s written.

I chose to use this assignment as an opportunity to practise what production-quality code and documentation actually look like — robust implementation paired with explanations that make future readers successful.
