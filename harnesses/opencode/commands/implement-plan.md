
---
description: Implement the latest approved plan in the current conversation
agent: build
---

Implement the latest explicitly approved implementation plan
in the current conversation.

Act as an expert engineer in the current repository's technology stack.

## Preconditions
- Locate the latest explicitly approved plan, including approved revisions.
- Verify that it applies to the current repository and is not superseded.
- Do not treat a proposed or discussed plan as approved.
- If no approved plan exists, or its scope is ambiguous:
  - Do not modify any files.
  - Stop immediately and report:
    "BLOCKED: No unambiguous, approved implementation plan
    is available. Create and approve a plan before proceeding."

## Engineering Standards
- Production-quality implementation only.
- Follow applicable AGENTS.md and existing repository patterns.
- Make minimal, safe, focused changes.
- No unrelated refactoring or speculative abstractions.
- Preserve existing behavior unless explicitly required.
- Apply relevant stack-specific engineering expertise.
- Add/update unit tests as needed.

## Implementation & Verification
- Implement only the approved plan; do not expand its scope.
- Handle relevant edge cases, errors, and integration points.
- Run applicable automated tests and checks.
- Verify acceptance criteria where applicable.
- Report failures, blockers, and deviations honestly.
- If the plan requires material changes, stop and request approval.

## Completion Summary
Report:
1. **Files changed:** Paths and purpose.
2. **Behavior implemented:** Functionality delivered.
3. **Tests:** Added/updated tests and execution results.
4. **Manual verification:** Steps and expected outcomes.
5. **Outstanding issues:** Risks, blockers, or deviations.

Do not update external systems or create commits automatically.
Stop after implementing the approved plan.
