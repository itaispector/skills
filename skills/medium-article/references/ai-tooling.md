# AI / LLM Tooling & Workflows — Domain Reference

## Audience assumptions

Your reader is a developer who uses AI tools daily — Copilot, Claude, Cursor, ChatGPT — and is past the "wow AI can code" phase. They want to know what actually works in practice, what's hype, and how to integrate AI into serious workflows without losing engineering rigor.

## Current discourse landscape

The AI-for-developers space is noisy. Every week there's a new "AI-powered" tool. The signal-to-noise ratio is terrible. Your job is to be signal.

Key tensions to be aware of:
- "AI will replace developers" vs "AI is just autocomplete" — both are wrong, and readers are tired of both
- The gap between demo-quality AI output and production-quality code
- Context window limitations and their practical impact on real codebases (especially monorepos)
- The emerging category of "AI-native" development tools (Claude Code, Cursor, Windsurf) vs AI bolted onto existing tools
- RAG, agents, and MCP as concepts developers are evaluating but haven't fully committed to
- The prompt engineering vs "just use it" debate

## Strong angles for this domain

- Honest tool comparisons based on actual daily use, not a weekend test drive
- Workflow patterns that leverage AI without becoming dependent on it
- The specific failure modes of AI coding tools and how to work around them
- How AI changes code review, architecture decisions, and team dynamics
- The economics — when AI tools save time vs when they create hidden debt
- Practical prompt patterns that actually improve output quality for coding tasks

## Writing cautions

- **Don't be breathlessly positive.** The reader's BS detector is calibrated for AI hype. If you say something is great, show receipts.
- **Don't be reflexively dismissive either.** "AI is just a toy" takes are as lazy as the hype.
- **Be specific about models and versions.** "I tested this with Claude Sonnet 4" is useful. "AI can do this" is not.
- **Acknowledge the moving target.** What's true today about model capabilities may not be true in 3 months. Frame time-sensitive claims accordingly.
- **Avoid the word "revolutionize."** And "game-changer." And "paradigm shift." Just describe what changed and let the reader decide the magnitude.

## Vocabulary notes

- "LLM" is fine, "large language model" on first use if the audience is broader
- "Context window" not "context length"
- "Prompt" as both noun and verb is established
- "Hallucination" is the accepted term — don't try to replace it with "confabulation" unless you're making a specific point about the terminology
- "Agentic" is jargon but increasingly standard — use it but don't overuse it
- Avoid "AI-powered" as an adjective — it's become meaningless marketing language

## Title examples that work

- "I Used Claude Code for a Month on a Real Monorepo. Here's What Surprised Me."
- "The Prompt Patterns That Actually Work for Code Generation"
- "Why RAG Is Harder Than You Think (And What to Do About It)"
- "AI Coding Tools Have a Context Problem. Nobody Wants to Talk About It."
