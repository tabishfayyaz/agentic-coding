
---
description: Plan production-quality implementation of a Jira ticket
agent: plan
---

Read Jira ticket $ARGUMENTS using the connected Jira MCP.

Act as an expert engineer in the current repository's technology stack.
Produce an actionable implementation plan. Do not modify code.

## Requirements
- Read the ticket, acceptance criteria, and relevant linked specifications.
- Identify dependencies, ambiguities, and missing requirements.
- Read applicable AGENTS.md instructions and inspect the codebase.
- Identify the architecture, frameworks, conventions, and relevant code.
- Follow existing patterns; flag unsafe or conflicting conventions.
- Do not invent requirements, files, or implementation details.

## Implementation Plan
Include:
1. **Approach:** Technical solution, key decisions, and tradeoffs.
2. **Files:** Exact paths, symbols, and expected changes.
3. **Existing patterns:** Specific implementations and utilities to reuse.
4. **UI/state/data flow:** Interactions, state ownership, asynchronous behavior,
   and data movement where applicable.
5. **Integration points:** Relevant APIs, services, persistence, navigation,
   dependency injection, analytics, and feature flags.
6. **Tests:** Unit tests to add/update, edge cases, and other justified tests.
7. **Risks:** Error handling, lifecycle, concurrency, security, performance,
   compatibility, and regressions where relevant.
8. **Manual verification:** Concrete steps and expected outcomes.
9. **Acceptance criteria:** Map each criterion to changes and verification.

## Implementation Granularity
- Assume the ticket is already reasonably scoped.
- Prefer one cohesive implementation for small tickets.
- Propose independently verifiable slices only when complexity or risk
  justifies them; explain the reason, scope, order, and verification.
- Do not plan work beyond the ticket or approved slice.

## Engineering Standards
- Production-quality, minimal, safe changes.
- Follow existing repository architecture and conventions.
- No unnecessary refactoring, speculative abstractions, or scope expansion.
- Preserve existing behavior unless changes are explicitly required.
- Add/update unit tests as needed.
- Apply stack-specific engineering expertise only where relevant.

## Constraints
- Do not modify code or update Jira.
- Distinguish verified findings from assumptions.
- Flag unresolved questions and blockers.
- Present a concise, actionable plan and stop for review.
