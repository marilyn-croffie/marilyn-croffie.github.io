---
layout: project
title: "Software Lifecycle Documentation Suite"
context: "Scheduling Software • Genetic Algorithms"
role: "Team Lead, Software Engineer, Technical Writer"
stack: "Technical documentation • Project management • Requirements analysis • Database design • Testing • Knowledge transfer"
repo: "https://github.com/marilyn-croffie/project-documentation-suite"
featured: true
excerpt: "Complete software development lifecycle documentation suite (80+ pages across 6 documents) for a scheduling system deployed Spring 2023, now used as program templates throughout the project-based Computer Science program."
---

## The Context
I led a four-person team building an automated core scheduling engine for MavPASS, a peer-facilitated academic support program at MSU, Mankato. The goal was to generate schedules that placed sessions at times that actually worked for both student leaders running the sessions and students trying to attend them.

The software needed to balance student accessibility, leader availability, and operational constraints, and it was intended to be developed into a full application across semesters by rotating student teams.

From the outset, it was clear that documentation would determine whether the system survived beyond the original developers.

## The Challenge
This was not a case of writing documentation after the fact. The team needed to understand unfamiliar concepts — genetic algorithms, constraint optimization, database design — while building production software under time and resource constraints.

At the same time, the documentation had to serve multiple audiences: non-technical program directors, junior engineers on the team, and future teams who would inherit the system without direct access to its original authors.

## My Approach
I designed documentation as a system rather than a single artifact. Instead of one monolithic document, I created a suite covering the full software lifecycle, with each document serving a specific purpose while reinforcing shared assumptions and decisions.

Two documents were especially central:
- Fitness Scores, which explains not just how the scheduling algorithm works, but why each constraint and weight exists, with examples, trade-offs, and edge cases.
- Handover, which preserves project context that would otherwise be lost — scope changes, known technical debt, unanswered questions, and clear recommendations for future teams.

The emphasis throughout was on making design reasoning explicit, so future contributors could make informed changes rather than reverse-engineering intent.

## The Impact
The system was deployed in production for Spring 2023, scheduling over 100 sessions. More importantly, the documentation enabled continuity.

A subsequent team successfully picked up the project without the original developers present, and the documentation suite was adopted by the Computer Science program as a template for future project teams.

This project marked a shift in my writing: from explaining concepts, to building documentation infrastructure that supports coordination, knowledge transfer, and long-term maintainability.
