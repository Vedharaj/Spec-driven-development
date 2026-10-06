# Multi-Agent Workflow

Use specialized agents according to responsibility.

## Sequence

Analysis
→ Architecture
→ Specification
→ Implementation
→ Security Review
→ QA

## Rules

- Prefer the smallest capable agent.
- Do not duplicate work between agents.
- Analysis agents should not modify application code.
- Implementation agents must follow approved specifications.
- Security and QA review completed work independently.
