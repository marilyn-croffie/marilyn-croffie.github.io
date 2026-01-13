---
layout: project
title: "Software Lifecycle Documentation Suite"
context: "Scheduling Software • Genetic Algorithm"
role: "Team Lead, Software Engineer, Technical Writer"
stack: "Technical documentation, Project management, Algorithm documentation, Requirements analysis, Database design, Testing frameworks, Knowledge transfer"
repo: "https://github.com/tbd"
featured: true
excerpt: "Complete software development lifecycle documentation suite (80+ pages across 6 documents) for a scheduling system deployed Spring 2023, now used as program templates throughout the project-based Computer Science program."
---

## My Role & Unique Positionality

I was team lead and senior engineer for a four-person team building an automated scheduling system for MavPASS, our university's peer-facilitated academic support program. But I brought three perspectives that shaped not just the solution, but how it was documented:

**1. Domain Expert:** I was actively working as a MavPASS leader while building this system. I understood the program from the inside—what makes a good schedule from a leader's perspective, what constraints actually matter in practice, what pain points exist that clients might not articulate clearly.

**2. Student:** I understood student accessibility challenges. I knew which session times worked, which didn't, and why variety mattered for students with recurring conflicts.

**3. Senior Engineer with Junior Team:** I was leading three junior engineers. Documentation couldn't just record decisions—it had to teach the team, enable their contributions, and transfer knowledge to future teams who'd pick up the project.

This triple positionality was critical. During requirements gathering, I could steer conversations between non-technical program directors and my junior engineering team in ways that made sense for everyone. I could ask the right clarifying questions because I knew what "optimal scheduling" actually meant operationally, not just theoretically. I could translate domain knowledge into technical requirements my team could implement.

## The Documentation Challenge

This wasn't "write some docs for the project." I faced several interrelated challenges:

**Teaching while building:** My team needed to understand genetic algorithms, constraint optimization, database normalization, and professional documentation standards—all while delivering production software. Documentation had to be teaching material, not just reference.

**Enabling continuity:** This was a semester project, but the scheduling system needed to run for years. Teams would graduate. Staff would change. The documentation needed to be the permanent source of truth.

**Serving multiple audiences:** Program directors needed user guides. Future developers needed technical specs. The CS program needed evidence that we followed professional standards. Each audience required different documentation without duplication.

**Making the complex comprehensible:** Genetic algorithms aren't straightforward. Scheduling constraints are nuanced. I needed to transform complex technical decisions into clear explanations that future teams could build on without me there to explain.

## What I Built: Documentation as Infrastructure

I created six interconnected documents covering the complete software development lifecycle. But the key wasn't just producing documents—it was designing a documentation system that would enable long-term maintainability.

### The Pedagogical Approach: Fitness Scores Document

The 25-page Fitness Scores document exemplifies my documentation philosophy. This isn't just "here's how the algorithm works"—it's teaching material that explains genetic algorithm design.

For each scheduling constraint, I structured the documentation to teach decision-making logic:

**Constraint definition:** What does this measure and why does it matter for student accessibility? (Not just "what" but "why it matters")

**Importance rationale:** Why is this constraint critical? Backed by research on attendance patterns and student needs.

**Scoring rules:** Detailed tables with worked examples showing edge cases (perfect variety, partial variety, no variety, mixed configurations).

**Student impact analysis:** Real scenarios showing consequences. Example: "Student with Monday work conflicts loses access to both sessions if both are Monday, but can attend one of two if variety exists."

**Design decisions:** Why we chose this approach over alternatives. I documented rejected options and trade-offs so future teams understand *why* we made these choices, not just what we chose.

**Edge cases:** Special handling for single-session leaders, availability constraints, online vs in-person sessions.

**Why this level of depth?** Future teams need to understand not just what the scoring function does, but why constraints are weighted the way they are. Without this, someone might change a weight without realizing it undermines the core value proposition. This documentation prevents that.

### Making Implicit Knowledge Explicit: Handover Document

My insider knowledge as a MavPASS leader couldn't stay in my head—it had to become documentation. The 13-page Handover document makes explicit things like:

**Why we renegotiated scope:** We cut UI development mid-project to focus on the core algorithm. The Handover explains why (complexity exceeded time available), what we delivered vs didn't, and where the next team should start. This prevents them from wasting time re-discovering our decisions.

**What technical debt exists:** I documented unfinished work (code modularization, optimization, testing coverage) with specific recommendations for where to focus next.

**What questions we couldn't answer:** Research gaps like fitness score upper bounds and implications of adding too many constraints. Being explicit about unknowns is as important as documenting knowns.

### Audience-Specific but Interconnected

Each document serves a specific audience but they work as a system:

- **Requirements Analysis:** Non-technical clients understand what we're building and why
- **Database Design:** Database engineers see entity relationships and normalization decisions
- **Fitness Scores:** Algorithm developers understand constraint logic and weight justifications
- **Test Plan:** QA engineers have testing frameworks and defect tracking processes
- **User Documentation:** Program directors (non-technical) can operate the software independently
- **Handover:** Future teams get complete project context to continue work

The Handover document ties them all together, creating a complete knowledge base.

## The Impact

**Successfully deployed for Spring 2023:** The software was used in production to schedule 100+ sessions. Not a prototype—an actual deployment solving a real problem for real clients.

**Became program templates:** The CS program now uses this documentation suite as blueprints for how project teams should document their work. The structure—requirements, design, implementation (with pedagogical depth), testing, user guides, handover—became the program standard.

**Enabled project continuity:** A second team successfully picked up the project because the Handover document gave them complete context without me there to explain.

**Made algorithm maintainable:** The Fitness Scores document means anyone modifying the scoring logic understands *why* weights are set the way they are, preventing well-intentioned changes from breaking carefully considered design decisions.

## What This Demonstrates

**Domain expertise translated to technical solutions:** My positionality as both MavPASS leader and software engineer meant I could bridge the gap between domain needs and technical implementation. I knew what questions to ask because I understood the program from the inside.

**Senior engineer leadership:** Managing a junior team meant documentation couldn't just be reference material—it had to teach. The suite educated my team while enabling them to contribute meaningfully to a complex project.

**Pedagogical documentation:** The Fitness Scores document could be used as teaching material for genetic algorithm design. It doesn't just describe—it teaches the decision-making logic behind every scoring rule. That's a higher standard than typical software documentation.

**Institutional thinking:** I didn't just document our project—I built documentation infrastructure that would serve multiple teams across multiple semesters. This shows understanding that documentation outlives individual projects.

**Complete lifecycle coverage:** Requirements, design, implementation, testing, user guides, handover—this demonstrates understanding of professional software development, not just "write some code and docs."

**Making the complex comprehensible:** Genetic algorithms are hard. Scheduling constraints are nuanced. I transformed complex technical decisions into clear explanations that future teams can build on, maintaining project knowledge even as people graduate and move on.

The suite wasn't just project documentation—it was the infrastructure that enabled coordination, knowledge transfer, and long-term maintainability. That's the difference between documenting work and building documentation systems.
