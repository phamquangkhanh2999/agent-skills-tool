---
name: spec-driven-dev
description: Ensure a clear specification exists before any code is written. Use when starting new features, complex refactors, or projects.
---

# 📝 Spec-Driven Development (Prime)

## Overview

A specification (Spec) is the source of truth that defines *what* we're building and *why*, before we decide *how*. This skill ensures that we don't start coding until we have established a clear set of requirements, constraints, and acceptance criteria.

## Process

### 1. Initialize Spec
If no spec exists, create one in the `docs/specs/` directory (or equivalent).

### 2. Define Objectives & Tone
- **Problem**: What specific problem are we solving?
- **User Value**: Why does this matter for your **Personal/Portfolio** brand?
- **Tone**: Is the aesthetic "Luxury Minimalist", "Creative Brutalist", or "Tech-Futurist"?

### 3. Functional Requirements
- List essential features.
- Define the "Happy Path" and edge cases.

### 4. Technical Constraints
- Tech stack (e.g., Next.js 15, React 19).
- Integration points (MCPs, APIs).

### 5. Acceptance Criteria
Define **Verifiable** outcomes:
- [ ] UI matches the target aesthetic.
- [ ] Lighthouse score > 90 for performance.
- [ ] No regression in core functionality.

## Anti-Rationalization

| Excuse | Reality |
|---|---|
| "It's a simple change, I don't need a spec." | Simple changes often have hidden side effects. A spec takes 2 mins to write but saves 2 hours of rework. |
| "I'll write the documentation after I'm done." | Post-hoc documentation is a fairy tale. Writing it first clarifies your own thinking. |
| "A spec is too formal for a personal project." | High quality requires high discipline. If it's worth doing, it's worth defining. |

## Verification
- [ ] Spec is committed or documented.
- [ ] User has approved the spec.
- [ ] All stakeholders (you and the user) are aligned on the "What".
