
---
description: Preview proposed code changes from the current implementation plan
agent: plan
---

Preview the exact proposed code changes for the latest
implementation plan in the current conversation.

Act as an expert engineer in the current repository's technology stack.

## Preconditions
- Locate the latest clear implementation plan, including agreed revisions.
- Verify that it applies to the current repository and is not superseded.
- Approval is not required to preview the plan.
- If no clear plan exists or its scope is ambiguous, stop and report:
  "BLOCKED: No clear implementation plan is available.
  Create or clarify a plan before running /preview-changes."

## Proposed Changes
Include:
1. **Files:** Exact paths of existing files to modify.
2. **Changes:** Specific classes, functions, and logic to change
   in each file, with illustrative snippets or diffs where useful.
3. **New files:** Paths, purpose, and key contents, if any.
4. **Tests:** Unit tests to add/update and scenarios to cover.
5. **Out of scope:** What will explicitly NOT be changed.
6. **Risks:** Assumptions, dependencies, edge cases, and regressions.

## Engineering Standards
- Production-quality solutions only.
- Follow applicable AGENTS.md and existing repository patterns.
- Prefer minimal, safe changes without unrelated refactoring.
- Preserve existing behavior unless explicitly required.
- Apply relevant stack-specific engineering expertise.
- Identify deviations from the existing plan.

## Constraints
- Do not modify code or update external systems.
- Do not implement proposed changes.
- Distinguish verified findings from assumptions.
- Present the proposed changes and stop for review.
