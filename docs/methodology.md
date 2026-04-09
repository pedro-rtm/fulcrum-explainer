# Technology Due Diligence Framework v0.1

**Practice:** Fulcrum (working name)
**Author:** Pedro Rivera Torres Moir
**Date:** April 2026

---

## Overview

Structured technology assessment for PE-backed transactions. 7-dimension framework producing quantified risk scoring, cost-to-fix estimates, and IC-ready value creation roadmaps in 10–15 working days.

---

## The 7 Assessment Dimensions

### 1. Architecture & Infrastructure
**Question:** Can the technology scale to support the value creation plan?

- Cloud maturity (lift-and-shift vs cloud-native vs on-prem)
- System topology (monolith, SOA, microservices, serverless)
- Technical debt inventory (quantified in GBP: remediation cost, timeline, complexity)
- Scalability ceiling (at what revenue/user level does architecture break?)
- Single points of failure (SPOFs)
- Third-party dependencies and vendor lock-in risk
- API architecture and integration layer health
- Data storage and backup infrastructure

**Output:** Architecture risk score (1–5), technical debt estimate (GBP), scalability assessment

### 2. Team & Organization
**Question:** Can this team deliver the technology roadmap?

- Engineering headcount and composition (frontend/backend/infra/data/QA ratio)
- Seniority distribution (junior/mid/senior/lead/architect)
- Key-person risk (who leaves and everything breaks?)
- Outsourcing mix (in-house vs contractors vs offshore)
- Engineering management structure (span of control, reporting lines)
- Hiring plan feasibility (can they actually hire what they need in this market?)
- Conway's Law assessment (does org structure match architecture?)
- Culture signals (Glassdoor, GitHub activity, Slack/comms patterns)

**Output:** Team risk score (1–5), key-person risk assessment, hiring cost estimate

### 3. Security & Compliance
**Question:** What is the exposure surface and what will remediation cost?

- OWASP Top 10 vulnerability assessment
- SOC 2 readiness (Type I vs Type II gap analysis)
- GDPR / NIS2 compliance posture
- Penetration test history and findings (review existing reports)
- Identity and access management (IAM) maturity
- Encryption at rest and in transit
- Incident response plan existence and quality
- Third-party security risk (supply chain assessment)
- Regulatory exposure by jurisdiction

**Output:** Security risk score (1–5), compliance gap list, remediation cost estimate

### 4. Data & Analytics
**Question:** Is the data an asset or a liability?

- Data quality assessment (completeness, accuracy, timeliness, consistency)
- Data governance maturity (ownership, lineage, cataloging)
- Integration health (how many systems, how connected, data latency)
- Analytics capability (BI maturity, self-serve vs IT-dependent)
- AI readiness score (data pipeline quality, feature engineering capability, model infrastructure)
- Data privacy and retention policies
- Master data management status

**Output:** Data maturity score (1–5), AI readiness assessment, data remediation estimate

### 5. Cost Structure
**Question:** How much does the technology actually cost, and how much should it cost?

- Total technology spend (capex + opex breakdown)
- Cloud cost analysis (current spend, optimization potential, benchmark vs revenue)
- License and subscription audit (unused licenses, renewal risk, vendor negotiation leverage)
- Run-rate analysis (what does "keeping the lights on" cost monthly?)
- Cost-to-fix estimate (technical debt remediation, security hardening, infrastructure upgrades)
- Build vs buy analysis for critical systems
- Headcount cost vs output benchmarking

**Output:** Current cost breakdown, optimization potential (GBP), cost-to-fix estimate (phased 6/12/24 months)

### 6. Delivery Capability
**Question:** Can this team ship reliably?

- Release cadence (how often does code reach production?)
- CI/CD maturity (automated testing, deployment pipelines, rollback capability)
- QA practices (unit tests, integration tests, E2E tests, coverage metrics)
- DevOps maturity (infrastructure as code, monitoring, alerting, observability)
- Incident management (MTTR, on-call practices, post-mortem culture)
- Project management methodology (agile maturity, sprint predictability)
- Product backlog health (age, prioritization, technical debt balance)

**Output:** Delivery capability score (1–5), DevOps maturity assessment, velocity benchmark

### 7. Strategic Alignment
**Question:** Does the technology roadmap support the business plan?

- Technology roadmap vs business strategy alignment
- M&A integration readiness (can this system absorb or be absorbed?)
- Platform vs product positioning (is technology a cost center or value driver?)
- Innovation pipeline (R&D investment, patent portfolio if applicable)
- Competitive technology moat assessment
- First-100-day technology priorities (what must happen immediately post-close)

**Output:** Strategic alignment score (1–5), 90-day priority roadmap, 12-month technology plan

---

## Standardized Scoring

| Score | Label | Definition |
|-------|-------|-----------|
| 1 | Critical | Immediate risk to business operations. Requires emergency intervention |
| 2 | Significant | Major gaps that will impact value creation plan. 6-month remediation |
| 3 | Moderate | Functional but suboptimal. 12-month improvement roadmap |
| 4 | Good | Minor gaps. Optimization opportunities exist |
| 5 | Excellent | Best-in-class for company size/stage. Competitive advantage |

---

## DD Engagement Structure

### Week 1: Discovery & Data Collection
- Day 1–2: Kickoff, document requests, system access, stakeholder mapping
- Day 3–5: Technical interviews (CTO, lead engineers, DevOps, security), codebase review, infrastructure walkthrough
- Weekend: Data synthesis, preliminary scoring

### Week 2: Analysis & Report
- Day 6–8: Deep-dive analysis, cost modeling, benchmark comparison
- Day 9–10: Report drafting, findings validation with management team
- Day 11: Final report delivery, executive presentation

### Week 3 (optional): Value Creation Workshop
- Day 12–15: 90-day value creation roadmap workshop with management team

---

## Deliverables

1. **Executive Summary** (2 pages) — IC-ready. Risk scorecard, top findings, cost-to-fix, recommendation
2. **Full Assessment Report** (20–40 pages) — Detailed findings across all 7 dimensions
3. **Risk Scorecard** (1 page) — Standardized 1–5 scores with visual heatmap
4. **Cost-to-Fix Estimate** (1 page) — Phased remediation costs (GBP) over 6/12/24 months
5. **Value Creation Roadmap** (3–5 pages) — 90-day quick wins + 12-month plan with expected ROI

---

## Data Capture Protocol

Every engagement captures standardized data for the proprietary dataset (internal only — never disclosed to clients):

```
{
  "company": { sector, revenue_band, geography, stage, employee_count },
  "tech_stack": { cloud_providers, architecture_type, core_systems, tooling },
  "team": { headcount, composition, seniority, outsourcing_pct },
  "problems": [{ category, severity_1to5, affected_systems }],
  "scores": { architecture, team, security, data, cost, delivery, strategic },
  "cost_to_fix": { immediate_gbp, 6mo_gbp, 12mo_gbp, 24mo_gbp },
  "predictions": { cost_savings_pct, timeline_months, risk_probability },
  "actuals": { TBD — captured post-engagement in Phase 1 work }
}
```

---

## Tools & Access Typically Required

- Source code repository access (GitHub, GitLab, Bitbucket)
- Cloud console access (AWS, Azure, GCP — read-only)
- CI/CD pipeline access (Jenkins, GitHub Actions, CircleCI)
- Monitoring/observability dashboards (Datadog, New Relic, Grafana)
- Architecture diagrams and system documentation
- Org chart and team composition data
- Financial data: technology spend breakdown, vendor contracts
- Recent penetration test reports
- Incident logs (last 12 months)
- Product roadmap and backlog
