[README.md](https://github.com/user-attachments/files/31406294/README.md)
# Online Property Tax Payment Portal — E-Governance Internship

Project work for the **Junior Web Developer – E-Governance & Digital Services** internship
(01 Aug 2026 – 29 Aug 2026), prepared by **Palak Ramtri**. Project complete — all four
weeks delivered.

Repo: [github.com/Priym1/Online-Property-Tax-Payment-Portal](https://github.com/Priym1/Online-Property-Tax-Payment-Portal)

This repo tracks the planning, design, testing, and audit artifacts for a citizen-facing
e-governance digital service: an **Online Property Tax Payment Portal** that lets property
owners search their property, view tax dues, pay online, and receive a digital receipt.

## Contents

```
docs/
  Week1-Project-Plan-Report.docx              Week 1 — Planning & Requirements Analysis
  Week2-Responsive-Prototype-Report.docx      Week 2 — Responsive Wireframes & Design Rationale
  Week3-QA-Testing-Strategy-Report.docx       Week 3 — QA & Testing Strategy
  Week4-Performance-Accessibility-Security-Audit.docx   Week 4 — Final Audit Report
wireframes/
  week1-process-flow.png                      Citizen payment process flow (6 steps)
  week1-user-journey.png                      Citizen user journey map (emotions per stage)
  desktop-wireframes.png                      High-fidelity desktop wireframes (4 core screens)
  mobile-wireframes.png                       Responsive mobile wireframes (3 key screens)
  site-flow.png                               Site navigation / user flow diagram
testing/
  testing-pyramid.png                         Testing pyramid (unit/integration/system/UAT)
  test-execution-workflow.png                 Test execution & automation workflow
audit/
  performance-load-time.png                   Page load time vs benchmark chart
  accessibility-wcag-compliance.png            WCAG POUR compliance chart
  security-risk-matrix.png                     Security vulnerability risk matrix
```

## Week 1 — Planning & Requirements Analysis

Defines the project vision, functional and non-functional requirements, stakeholder
analysis (with two user personas), a risk register, proposed technology stack, and a
4-week project roadmap. See `docs/Week1-Project-Plan-Report.docx`.

## Week 2 — Responsive Web Prototype

Translates the Week 1 plan into a high-fidelity, responsive UI:

- **Core screens:** Login/Registration, Property Search & Bill View, Payment, Receipt/Confirmation
- **Responsive behaviour:** two-column desktop layouts collapse into single-column mobile
  layouts, with a hamburger nav and full-width touch targets
- **Design rationale:** colour palette, typography, card-based layout and status-feedback
  choices, each with reasoning

See `docs/Week2-Responsive-Prototype-Report.docx` for the full write-up.

## Week 3 — QA & Testing Strategy

Defines how the platform will be validated before release:

- **Test plan:** layered testing pyramid (unit → integration → system → manual/UAT),
  with automated vs manual execution strategy
- **Test cases:** 8 detailed scenarios covering functional, negative, security,
  performance, and responsive-UI testing
- **Risk analysis:** 6 testing-specific risks (duplicate payments, session hijacking,
  stale data, gateway outages, XSS, accessibility regressions) with mitigations
- **Test execution workflow:** write → execute → log defects → fix/retest → regression → sign-off

See `docs/Week3-QA-Testing-Strategy-Report.docx` for the full write-up.

## Week 4 — Performance, Accessibility & Security Audit

Final audit of the platform before rollout:

- **Performance:** 6 KPIs (load time, TTFB, responsiveness, resource consumption,
  concurrency, uptime) with benchmarks and measurement methods; load-time chart flags
  Property Search and Payment as over budget
- **Accessibility:** WCAG 2.1 AA compliance scored by POUR principle, with 6 findings
  and fixes (contrast, keyboard nav, screen readers, zoom, language)
- **Security:** 8 vulnerabilities (XSS, SQL injection, IDOR, CSRF, etc.) plotted on a
  likelihood × impact risk matrix, each with a mitigation
- **Improvement roadmap:** prioritized High/Medium/Low recommendations across all three areas

See `docs/Week4-Performance-Accessibility-Security-Audit.docx` for the full write-up.

## Proposed Tech Stack

| Layer | Technology |
|---|---|
| Frontend | React.js, Tailwind CSS |
| Backend | Node.js / Express REST API |
| Database | PostgreSQL / MySQL |
| Payments | PCI-DSS compliant gateway (UPI, cards, net banking) |
| Auth | OTP-based login |
| Hosting | Cloud (AWS/Azure) with auto-scaling |
| Testing | Jest/Mocha (unit), Postman/Newman (API), Playwright/Cypress (E2E) |
| Monitoring | Lighthouse/Core Web Vitals (performance), NVDA (accessibility), OWASP-aligned review (security) |

## Roadmap

| Week | Focus |
|---|---|
| 1 | Planning & Requirements Analysis ✅ |
| 2 | UI/UX Design & Responsive Wireframing ✅ |
| 3 | QA & Testing Strategy ✅ |
| 4 | Performance, Accessibility & Security Audit ✅ |
