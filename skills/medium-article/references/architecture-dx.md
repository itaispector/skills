# Software Architecture & DX — Domain Reference

## Audience assumptions

Your reader is a mid-to-senior developer or tech lead who makes (or influences) architectural decisions. They've been burned by over-engineering and by under-engineering. They're skeptical of silver bullets but open to better patterns. They care about team velocity as much as technical elegance.

## Current discourse landscape

- Monorepos are mainstream but the tooling debate (Nx vs Turborepo vs Rush vs Bazel) is active
- Micro-frontends exist but many teams are finding they create more problems than they solve
- The "boring technology" philosophy (choose well-understood tools) has strong support
- DevEx/DX as a discipline is gaining legitimacy — internal platform teams, developer productivity metrics
- The pendulum between microservices and monoliths has swung back toward pragmatic modularity
- TypeScript is no longer optional — the discussion has moved to how strict and which patterns

## Strong angles for this domain

- Architecture decision records (ADRs) in practice — showing the actual tradeoff analysis
- Migration stories — how to move from X to Y without stopping feature work
- DX improvements with measurable impact (CI time, build time, onboarding time)
- The politics of technical decisions — how to advocate for the right architecture when stakeholders disagree
- Monorepo patterns and anti-patterns from real team experience
- When abstractions become liabilities — concrete examples of premature generalization

## Writing cautions

- **Don't cargo-cult.** "Netflix does X" is not an argument unless you're operating at Netflix's scale and constraints.
- **Acknowledge context.** An architecture that's perfect for a 5-person startup might be terrible for a 200-person org. Always specify who the advice is for.
- **Show the cost.** Every architectural choice has a maintenance cost. The article should make the total cost visible, not just the initial benefit.
- **Be honest about failure.** "We chose X and it turned out to be wrong" is more valuable than "we chose X and it was perfect."
- **Pragmatism over purity.** The reader doesn't care about theoretical elegance. They care about shipping and maintaining software with a real team.

## Vocabulary notes

- "DX" (Developer Experience) is established, no need to expand in this audience
- "Coupling" and "cohesion" — use precisely. Tight coupling between modules ≠ coupling in general
- "Tech debt" — be specific. "Tech debt" as a vague complaint is worthless. "This abstraction forces us to modify 4 files for every new feature" is actionable.
- "Scalability" — always specify the dimension (team size, request volume, codebase size, data volume)
- "Refactor" means behavior-preserving change. Don't say "refactor" when you mean "rewrite."
- Avoid "clean code" as a standalone justification — it means different things to different people

## Title examples that work

- "We Moved to a Monorepo. A Year Later, Here's What We'd Do Differently."
- "The Abstraction That Cost Us 6 Months"
- "Your CI Is Slow Because Your Architecture Is Wrong"
- "Why I Stopped Writing 'Clean' Code"
