
# Online Property Tax Payment Portal — E-Governance Internship

Project work for the **Junior Web Developer – E-Governance & Digital Services** internship
(01 Aug 2026 – 29 Aug 2026), prepared by **Palak Ramtri**. Project complete — all four
weeks delivered.

Repo: [github.com/Palak923/Property-Tax-Payment-Portal](https://github.com/Palak923/Property-Tax-Payment-Portal)

This repo tracks the planning, design, backend, and audit artifacts for a citizen-facing
e-governance digital service: an **Online Property Tax Payment Portal** that lets property
owners search their property, view tax dues, pay online, and receive a digital receipt.

## Contents

```
docs/
  Week1-Project-Plan-Report.docx                   Week 1 — Planning & Requirements Analysis
  Week2-Responsive-Prototype-Report.docx           Week 2 — Responsive Wireframes & Design Rationale
  Week3-Backend-Integration-Database-Management.docx  Week 3 — Backend Design, DB Schema & API Integration
  Week4-Performance-Accessibility-Security-Audit.docx Week 4 — Final Audit Report
wireframes/
  week1-process-flow.png                           Citizen payment process flow (6 steps)
  week1-user-journey.png                           Citizen user journey map (emotions per stage)
  desktop-wireframes.png                            High-fidelity desktop wireframes (4 core screens)
  mobile-wireframes.png                             Responsive mobile wireframes (3 key screens)
  site-flow.png                                     Site navigation / user flow diagram
backend/
  backend-system-architecture.png                   Service architecture & data flow diagram
  database-er-diagram.png                           Database entity-relationship diagram (7 tables)
audit/
  performance-load-time.png                         Page load time vs benchmark chart
  accessibility-wcag-compliance.png                 WCAG POUR compliance chart
  security-risk-matrix.png                          Security vulnerability risk matrix
extras/
  Week3-QA-Testing-Strategy-Report.docx             Supplementary QA/testing strategy (not part of the
                                                     official Week 3 brief — kept for reference)
  testing-pyramid.png                               Diagram supporting the extra QA report above
  test-execution-workflow.png                       Diagram supporting the extra QA report above
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

## Week 3 — Backend Integration & Database Management

Plans the backend that supports the Week 2 front-end:

- **System design:** service-oriented architecture (API Gateway, Auth/Property/Payment/
  Notification services, Redis cache, object storage, external gateways)
- **Database schema:** a normalised 7-table relational model (Citizens, Properties,
  TaxAssessments, Payments, Receipts, Grievances, AdminUsers, AuditLogs) with an ER diagram
- **API design:** 9 versioned RESTful endpoints with methods, parameters, and responses
- **Security & performance:** 8 concerns (auth, SQL injection, encryption, duplicate
  payments, caching, load, IDOR) each with a mitigation
- **Backup & recovery:** backup cadence, point-in-time recovery, DR drills, maintenance windows

See `docs/Week3-Backend-Integration-Database-Management.docx` for the full write-up.

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
| Cache | Redis (sessions, bill lookups) |
| Payments | PCI-DSS compliant gateway (UPI, cards, net banking) |
| Auth | OTP-based login, JWT sessions |
| Hosting | Cloud (AWS/Azure) with auto-scaling |
| Testing | Jest/Mocha (unit), Postman/Newman (API), Playwright/Cypress (E2E) |
| Monitoring | Lighthouse/Core Web Vitals (performance), NVDA (accessibility), OWASP-aligned review (security) |

## Roadmap

| Week | Focus |
|---|---|
| 1 | Planning & Requirements Analysis ✅ |
| 2 | UI/UX Design & Responsive Wireframing ✅ |
| 3 | Backend Integration & Database Management ✅ |
| 4 | Performance, Accessibility & Security Audit ✅ |
