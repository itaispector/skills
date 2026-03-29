# Frontend / React / Web Dev — Domain Reference

## Audience assumptions

Your reader is a working frontend developer with 2+ years of experience. They know what JSX is, they've used hooks, they've probably shipped a production app. Don't explain fundamentals — explain *insights about* fundamentals.

## Current discourse landscape (calibrate to this)

The React ecosystem in 2025-2026 is in a transitional period. Server Components are real but adoption is uneven. The meta-framework debate (Next.js vs Remix vs Astro vs others) is ongoing. Signals are gaining traction outside React. The bundler landscape has shifted (Vite dominance, Turbopack emerging). 

When writing about React, be aware of:
- The tension between React's direction (RSC, compiler) and what most teams actually ship
- The growing "React is too complex" counter-movement
- The practical reality that most production React apps are still CSR SPAs with React Router
- The Nx/monorepo ecosystem and its DX implications

## Strong angles for this domain

- "I tried X in production and here's what actually happened" — experience reports beat speculation
- Challenging accepted patterns with evidence (e.g., "You probably don't need that custom hook")
- Performance insights backed by actual profiling, not synthetic benchmarks
- Component API design philosophy — why certain abstractions work and others don't
- The gap between conference talks and production reality

## Code example standards

- Use TypeScript in examples (it's the default now)
- Use functional components exclusively unless the article is specifically about class components
- Prefer modern APIs: `useId`, `useSyncExternalStore`, `use()` where relevant
- Show real-ish component names and props, not `Foo` and `Bar`
- If comparing approaches, show both side by side with clear labels

## Vocabulary notes

- Say "re-render" not "re-rendering cycle"
- Say "component" not "component instance" unless the distinction matters
- "Server Component" (capital C) for the RSC concept, "server component" for general SSR components
- Avoid "performant" — say "fast" or be specific about what metric improved
- Don't say "boilerplate" as a blanket criticism — specify what's repetitive and why it matters

## Title examples that work

- "React Server Components Broke My Mental Model — Here's My New One"
- "The Real Cost of Prop Drilling (It's Not What You Think)"
- "Stop Abstracting Your Fetch Calls"
- "What Signals Get Right That React Hooks Don't"
