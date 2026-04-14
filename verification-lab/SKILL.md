---
name: verification-lab
description: Ensure all code changes are verified with evidence. Use before finishing any task or marking a task as [x].
---

# 🔬 Verification Lab (Prime)

## Overview

"It seems right" is the mother of all bugs. This skill mandates that every change must be backed by concrete evidence — whether it's passing unit tests, successful build logs, or visual confirmation in the browser.

## Process

### 1. Unit & Integration Verification
- Run existing test suites (`npm test`, `pnpm test`).
- Add new tests for the logic changed.
- **Beyonce Rule**: If you liked it, you shoulda put a test on it.

### 2. Manual Verification
- View the UI in the browser.
- Check responsive behavior (Mobile, Tablet, Desktop).
- Verify accessibility (Aria labels, Keyboard nav).

### 3. Log & Debug Verification
- Check browser console for errors/warnings.
- Check terminal output for clean builds.

### 4. Continuous Guard
- Ensure no regressions in performance (Check bundle size, LCP).

## Anti-Rationalization

| Excuse | Reality |
|---|---|
| "I manually tested it, it's fine." | Manual testing only checks the 'happy path' you followed. Verification gates check everything else. |
| "Tests are slow." | A broken production build is slower. Efficiency comes from correctness, not just speed. |
| "The environment is different, I can't test." | Reproduce the environment or mock it. Unverified code is liability. |

## Verification
- [ ] Evidence provided (Screenshots, Test logs, Command outputs).
- [ ] Zero console errors/warnings.
- [ ] Cross-browser/Cross-device verification confirmed.
