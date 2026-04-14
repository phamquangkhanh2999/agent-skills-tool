---
name: task-breakdown
description: Decompose specifications into atomic, verifiable tasks. Use when you have a spec and are ready to start planning the execution.
---

# 🗺️ Task Breakdown & Planning (Prime)

## Overview

Execution without a plan leads to messiness. This skill transforms a high-level Specification into a sequence of small, manageable tasks that can be independently verified.

## Process

### 1. Map Dependencies
- Identify which tasks must happen first.
- Cluster related changes together.

### 2. Create Atomic Tasks
Each task should be:
- **Small**: < 100 lines of code.
- **Independent**: Can be tested on its own.
- **Verifiable**: Has clear "Done" criteria.

### 3. Order Strategy
- **Infrastructure First**: Setup types, schemas, and API end-points.
- **Vertical Slices**: Complete one small feature from UI to Backend rather than doing all UI then all Backend.

### 4. Task tracking
Create or update the `task.md` artifact to track progress. Mark items as `[/]` (in progress) and `[x]` (completed).

## Anti-Rationalization

| Excuse | Reality |
|---|---|
| "I'll just remember what to do next." | Memory is a leak. A written task list offloads cognitive load for better coding focus. |
| "Breakdown takes too much time." | Thinking through the steps *before* typing code prevents logic errors and structural failures. |
| "I can do these 5 things in one commit." | Atomic tasks prevent "commit bloat" and make debugging significantly easier. |

## Verification
- [ ] Tasks are documented in `task.md`.
- [ ] Each task has a clear verification criteria.
- [ ] Sequence is logical and minimizes rework.
