---
name: checklists-library
description: Collection of quick-reference checklists for web quality. Use to verify Accessibility, Performance, and Security.
---

# 📚 Prime Checklists Library

## ♿ Accessibility (WCAG 2.1 AA)
- [ ] **Keyboard Nav**: Every interactive element is focusable and clickable via Tab/Enter/Space.
- [ ] **ARIA**: Meaningful `aria-label` for icons/buttons; proper `label` for forms.
- [ ] **Contrast**: Min 4.5:1 for normal text (WCAG AA).
- [ ] **Structure**: One H1 per page; logical heading hierarchy.

## ⚡ Performance (Core Web Vitals)
- [ ] **LCP**: Rendering of largest contentful element < 2.5s.
- [ ] **INP**: Interaction to Next Paint < 200ms.
- [ ] **CLS**: Cumulative Layout Shift < 0.1.
- [ ] **Assets**: Images optimized (WebP/AVIF), scripts deferred/async.

## 🛡️ Security (OWASP & Hardening)
- [ ] **Inputs**: No raw `innerHTML` or unsafe script execution.
- [ ] **Headers**: Proper CSP, XSS-protection, Frame-options.
- [ ] **Secrets**: No API keys or secrets in client-side code.
- [ ] **Packages**: `npm audit` is clean.

## 📱 Responsive & Cross-Browser
- [ ] **Breakpoints**: 320px, 768px, 1024px, 1440px.
- [ ] **Touch**: Tap targets > 44px.
- [ ] **Retina**: High-res assets provided where needed.
