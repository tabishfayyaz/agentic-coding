
---
description: Plan implementation of a Jira ticket
agent: plan
---

Read Jira ticket $ARGUMENTS using the connected Jira MCP.

Your task is to produce a technical implementation plan for this ticket within the current codebase.

## Step 1: Understand the requirements
- Read the ticket description and acceptance criteria.
- Identify dependencies and missing requirements.
- Do not invent requirements.

## Step 2: Investigate the codebase
- Identify relevant files, classes and interfaces.
- Understand existing architecture and conventions.
- Look for reusable implementations and patterns.
- Avoid unnecessary new abstractions.

## Step 3: Develop the implementation plan
- Explain the proposed technical approach.
- Identify files likely to require changes.
- Describe necessary tests and verification.
- Map implementation steps to acceptance criteria.
- Identify risks and unresolved questions.

## Step 4: Determine implementation granularity
- Assume the ticket is already reasonably scoped.
- Prefer one cohesive implementation.
- Recommend smaller slices only when technical complexity, dependencies or risk justify them.
- Explain why slicing is necessary if recommended.

## Constraints
- Do not modify source code.
- Do not update Jira.
- Do not perform unrelated refactoring.
- Stop after presenting the plan for review.