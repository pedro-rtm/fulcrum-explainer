# Learning Syllabus 2.0 — DD-Ready in 10 Weeks

**Date:** April 2026
**Goal:** Close the gap between what Pedro knows and what a credible DD engagement requires
**Source:** Merged from knowledge gap analysis (honest capability assessment) + original learning syllabus
**Total hours to credible first DD:** ~108h (10 weeks at ~11h/week)
**Total hours including PE fluency + secondary depth:** ~190h (6 months)

---

## How to read this

**Phases 1-4** = the critical path to surviving the first DD engagement (108h, 10 weeks). Ordered by the gap analysis: biggest gaps first.

**Track A** = PE conversational fluency. Run in parallel with Phases 1-4. Not required for the DD itself but required to not sound like an outsider when talking to PE operating partners.

**Track B** = secondary depth. Learn on-the-job after the first engagement. Nice to have, not gating.

**Track C** = ongoing market intelligence. 2-3h/week, never stops.

---

## Current state (from gap analysis)

| DD Dimension | Pedro now | Target | Gap | Hours to close |
|-------------|:---------:|:------:|:---:|:--------------:|
| 1. Architecture | 3.3/5 | 4/5 | Small | 26h |
| 2. Team | 3.1/5 | 4/5 | Small | 22h |
| **3. Security** | **1.9/5** | **3.5/5** | **CRITICAL** | **38h** |
| 4. Data | 3.0/5 | 3.5/5 | Small | 21h |
| **5. Cost** | **2.8/5** | **4/5** | **High** | **28h** |
| **6. Delivery** | **2.7/5** | **3.5/5** | **High** | **19h** |
| 7. Strategic | 3.2/5 | 4/5 | Medium | 18h |

**Shortcut:** Subcontract security (Dimension 3) to a specialist for the first 2-3 engagements at GBP 2-3K/deal. Pedro runs the engagement, specialist handles the dimension Pedro can't yet, Pedro learns from them.

---

## Phase 1: Security — Make It Non-Embarrassing (38h, 3 weeks)

This is the gating factor. An operating partner asking "walk me through the CVSS scores" will expose the gap immediately. Security is also the dimension PE firms care about most right now.

### 1.1 OWASP Top 10 (8h)
**Current level:** 2/5. Awareness only.
**Target:** Can identify each vulnerability class in a codebase review and explain business impact.

- Read the OWASP Top 10:2025 taxonomy (2-3h) — understand each category, data methodology, and what to flag in a DD report
- Hands-on labs: TryHackMe OWASP Top 10 2025 module (6-8h) — three guided rooms with attack VMs covering IAAA failures, application design flaws, insecure data handling
- Alternatively or additionally: PortSwigger Web Security Academy "Server-side" and "Client-side" learning paths (15-20h for the full path — overkill for DD but excellent if you want real depth)

**Resources:**
- OWASP Top 10:2025 Official — https://owasp.org/Top10/2025/ (free, the canonical source)
- TryHackMe OWASP module — https://tryhackme.com/module/owasp-top-10-2025 (~$14/month, guided, pre-configured VMs)
- PortSwigger Web Security Academy — https://portswigger.net/web-security (free, 190+ hands-on labs, industry standard)
- OWASP Cheat Sheet Series — https://cheatsheetseries.owasp.org/ (free, quick reference per vulnerability)

### 1.2 SOC 2 Readiness Assessment (10h)
**Current level:** 1/5. New territory.
**Target:** Can assess a company's SOC 2 gap and estimate remediation cost/timeline.

- Read the actual AICPA Trust Services Criteria (4-5h) — the 5 categories (Security, Availability, Processing Integrity, Confidentiality, Privacy) and the "points of focus" under each criterion. This is what auditors examine
- Study Type I vs Type II distinction, audit timeline, evidence requirements, and common control gaps (2-3h)
- Understand cost and timeline: typically 6-12 months, GBP 100-200K for mid-market SaaS. Key DD question: "Does this company have SOC 2 Type II, and if not, how far away?"
- Talk to Lorenzo about what Hg Capital required from CTAIMA on compliance

**Resources:**
- AICPA Trust Services Criteria (2022 revision) — https://www.aicpa-cima.com/resources/download/2017-trust-services-criteria-with-revised-points-of-focus-2022 (free PDF, the primary source)
- Drata SOC 2 Type 2 Guide — https://drata.com/grc-central/soc-2/type-2 (free, best vendor-produced explanation)
- Secureframe Trust Services Criteria Guide — https://secureframe.com/hub/soc-2/trust-services-criteria (free, maps criteria to practical controls)

### 1.3 Penetration Test Interpretation (4h)
**Current level:** 2/5.
**Target:** Can read a pentest report, interpret CVSS scores, and translate findings into business risk + remediation cost.

- Learn CVSS v4.0 scoring (1-2h) — base, temporal, environmental metrics. Also learn v3.1 since most existing reports still use it. Use the interactive calculator to score 5-10 hypothetical findings
- Read 3-4 real/redacted pentest reports end-to-end (2-3h) — build pattern recognition for finding structures, executive summaries, risk ratings, remediation recommendations

**Resources:**
- FIRST CVSS v4.0 User Guide — https://www.first.org/cvss/v4.0/user-guide (free, canonical)
- FIRST CVSS v4.0 Calculator — https://www.first.org/cvss/calculator/4.0 (interactive, practice scoring)
- FIRST CVSS v3.1 Calculator — https://www.first.org/cvss/calculator/3-1 (for interpreting existing reports)
- Sample pentest reports (all free PDFs):
  - PurpleSec sample — https://purplesec.us/wp-content/uploads/2019/12/Sample-Penetration-Test-Report-PurpleSec.pdf
  - Version 2 anonymised — https://version-2.com/wp-content/uploads/2022/08/Anonymised-Web-Application-Penetration-Testing-Report.pdf
  - Report URI real report (2024) — https://cdn.report-uri.com/pdf/Report%20URI%20-%20Penetration%20Test%20Report%20Latest.pdf
- Binsec CVSS in Pentesting Guide — https://binsec.com/en/pentest/cvss/ (bridges theory to practice)

### 1.4 GDPR & NIS2 Assessment (6h)
**Current level:** 2/5.
**Target:** Can assess a company's GDPR compliance posture and NIS2 readiness, identify gaps, estimate remediation.

- GDPR (2h): key technology-relevant articles (Art. 25 privacy by design, Art. 32 security, Art. 35 DPIA, Art. 30 records of processing). Build a DD assessment checklist
- NIS2 (3-4h): skim the ENISA Technical Implementation Guidance (170 pages — focus on incident handling, supply chain, governance sections). Run the HvS self-assessment tool against a hypothetical company to build intuition. Build a NIS2 DD checklist

**Resources:**
- ENISA NIS2 Technical Implementation Guidance (v1.0, June 2025) — https://www.enisa.europa.eu/publications/nis2-technical-implementation-guidance (free PDF, the authoritative source. 170 pages — skim, don't read cover to cover)
- HvS-Consulting NIS-2 Self-Assessment Tool — https://www.hvs-consulting.de/en/ressourcen/nis-2-self-assessment-tool (free Excel, maps NIS2 to ISO 27001 and CIS Controls. Usable as a DD quick-assessment)
- UpGuard NIS2 Compliance Checklist — https://www.upguard.com/blog/nis2-compliance-checklist (free, concise practitioner checklist)
- ICO (UK) GDPR guidance for technology companies — https://ico.org.uk/for-organisations/ (free)
- DLA Piper GDPR Data Protection Handbook — https://www.dlapiperdataprotection.com/ (free, jurisdiction-by-jurisdiction)

### 1.5 IAM & Incident Response (8h)
**Current level:** 2/5.
**Target:** Can assess IAM maturity and incident response readiness.

- IAM (4h): learn maturity levels (shared credentials → individual access → RBAC → ABAC → zero trust). Common failure patterns. MFA adoption assessment. Build a DD IAM checklist: "How do engineers access production? How are credentials rotated? Who has admin?"
- Incident response (4h): NIST SP 800-61 framework (6 phases: preparation, detection, containment, eradication, recovery, lessons learned). Key DD question: "Does this company have a tested incident response plan, and when was the last tabletop exercise?"

**Resources:**
- NIST SP 800-61 Rev. 2 — https://csrc.nist.gov/publications/detail/sp/800-61/rev-2/final (free PDF, the canonical IR framework)
- CIS Controls v8 — https://www.cisecurity.org/controls (free, IAM controls are in Control Groups 5-6)
- Microsoft IAM maturity model — search "Microsoft identity maturity model" (free, 5-level progression)
- PagerDuty Incident Response guide — https://response.pagerduty.com/ (free, practitioner-written, excellent)

### 1.6 Practice: Assess a Velkan System (2h)
- Pick one Velkan portfolio company's technology
- Run the full Dimension 3 assessment against it from memory
- Score each sub-area. Identify what you'd flag in a DD report
- Note where you got stuck — that's what needs more study

---

## Phase 2: Formalize What You Already Know (30h, 2 weeks)

Turn intuition into structured, repeatable, benchmarkable assessment.

### 2.1 DORA Metrics + DevOps Maturity (8h)
**Current level:** 2/5. Covers Dimensions 2 + 6.
**Target:** Can benchmark a team's delivery capability against DORA's 4 key metrics and identify the performance tier.

- Read *Accelerate* (6-8h) — the foundational text. Establishes the 4 metrics, the statistical proof they predict org performance, and the capability model. Winner of Shingo Publication Award. This is the book PE-backed CTOs cite
- Use the DORA Quick Check (30 min) — 5-minute survey producing a benchmarked 0-10 score. In a DD, you could have the target's engineering team complete this
- Study the capabilities catalog (2-3h) — 27 technical, process, and cultural capabilities (continuous delivery, trunk-based development, loosely coupled architecture, etc.)
- Note: 2024 report introduced 7 team performance profiles replacing the old elite/high/medium/low model. 2025 report focuses on AI-assisted development

**Resources:**
- Book: *Accelerate* by Forsgren, Humble, Kim — https://www.amazon.com/dp/1942788339 (~EUR 20, essential)
- DORA Quick Check — https://dora.dev/quickcheck/ (free, interactive benchmark tool)
- DORA Capabilities Catalog — https://dora.dev/capabilities/ (free, the 27 levers)
- State of DevOps Report 2024/2025 — https://cloud.google.com/devops/state-of-devops (free PDF)

### 2.2 FinOps + Cloud Cost Optimisation (8h)
**Current level:** 3/5 on cloud, 2/5 on FinOps. Covers Dimension 5.
**Target:** Can decompose a cloud bill, identify optimisation opportunities, and estimate savings with confidence.

- Read the FinOps Foundation framework (4-5h) — Inform/Optimise/Operate lifecycle, the 2025 "Scopes" concept (extends beyond cloud to SaaS, data centres, licences), maturity model
- Alternatively: take the free FinOps intro course (2-3h) for the minimum viable understanding
- Key levers to know: reserved instances/savings plans, right-sizing, spot instances, storage lifecycle, dev/staging scheduling
- Know the benchmarks: cloud cost as % of revenue by stage (seed: 15-25%, Series B: 10-18%, PE-backed: 8-12%)

**Resources:**
- FinOps Foundation Framework (2025 update) — https://www.finops.org/insights/2025-finops-framework/ (free)
- Free FinOps Introduction Course — https://learn.finops.org/ (free, 2-3h)
- FinOps Certified Practitioner (if going deep) — https://learn.finops.org/page/finops-certified-practitioner-self-paced ($500, 16-20h, valid 24 months)
- AWS Well-Architected Cost Optimization pillar — https://docs.aws.amazon.com/wellarchitected/latest/cost-optimization-pillar/ (free)

### 2.3 Capex vs Opex for PE (4h)
**Current level:** 2/5. CRITICAL for PE conversations. Covers Dimension 5.
**Target:** Can classify any technology expense as capex or opex and explain the EBITDA impact.

- Why it matters: PE firms value companies on EBITDA multiples. Capitalising development costs moves spend from opex → capex → off the P&L → higher EBITDA → higher valuation. DD must assess whether capitalisation policy is defensible or inflated
- Learn IAS 38 (IFRS) 6 criteria + ASC 350-40 (US GAAP) 3-stage model (1-2h). Note: ASU 2025-06 replaces the 3-stage model with principles-based threshold (effective Dec 2027)
- Common DD findings: over-capitalising to inflate EBITDA, capitalising maintenance as development, inconsistent policy across acquired entities
- Practice: classify 10 common tech expenses (cloud hosting, SaaS licences, custom dev, hardware, contractor costs, open-source contributions)

**Resources:**
- Swarmia: "The Hitchhiker's Guide to Capitalizing Software Development Costs" — https://www.swarmia.com/blog/capitalizing-software-development-costs/ (free, best practitioner guide. Covers IAS 38 + ASC 350-40 side by side, explains EBITDA impact for PE)
- Benchmark International: "The Impact of CAPEX on EBITDA Adjustments" — https://www.benchmarkintl.com/insights/the-impact-of-capex-on-ebitda-adjustments/ (free, M&A advisory perspective)
- PwC: ASU 2025-06 Software Capitalisation changes — https://www.pwc.com/us/en/services/consulting/deals/library/new-software-capitalization-standard.html (free, the new standard PE firms need to understand)

### 2.4 Technical Debt Quantification (6h)
**Current level:** 3/5. Covers Dimension 1.
**Target:** Can estimate technical debt in GBP with phased remediation costs.

- Learn the CAST methodology (3-4h) — automated violation detection × remediation effort estimate. Key benchmark: $3.61/line of code average across 1,400 applications / 550M lines (the most-cited figure in PE tech DD). CAST Highlight is the tool Crosslake and other DD firms use
- SIG/TÜViT maintainability model (1-2h) — ISO 25010-based, 8 system properties scored 1-5 stars. Used by European PE firms
- Install SonarQube Community Edition and scan a codebase (2h) — produces remediation cost in time, tech debt ratio, maintainability rating A-E. Even if you never run it yourself, understand how it produces numbers
- Practice: retrospectively quantify tech debt in GBP for 2-3 Velkan engagements

**Resources:**
- CAST Tech Debt Estimation — https://www.castsoftware.com/glossary/technical-dept-estimation (free methodology docs)
- CAST Highlight benchmarks by technology — https://doc.casthighlight.com/technical-debt-estimates-stats-technology/ (free, benchmark data)
- SonarQube metrics docs — https://docs.sonarsource.com/sonarqube-server/user-guide/code-metrics/metrics-definition (free)
- SIG Maintainability research paper — https://www.researchgate.net/publication/340267633 (free, compares Maintainability Index, SIG, and SQALE on 20 open-source projects)

### 2.5 Cost-to-Fix Estimation Practice (4h)
**Current level:** 3/5. Covers Dimension 5.
**Target:** Can produce a phased cost-to-fix estimate that an IC member would trust.

- Practice exercise: pick 3 Velkan portfolio companies
- For each: estimate the technology remediation backlog in GBP
- Phase into P1 (0-3 months), P2 (3-12 months), P3 (12-24 months)
- Estimate ROI for each phase
- Compare to what actually happened — calibrate your estimation accuracy

---

## Phase 3: PE-Specific Gaps (20h, 2 weeks)

What makes this DD and not just technology assessment.

### 3.1 M&A Integration Readiness (8h)
**Current level:** 2/5. Covers Dimension 7.
**Target:** Can assess whether a target's technology can absorb bolt-on acquisitions or be absorbed by an acquirer, and estimate integration costs.

- Read the Umbrex PMI Playbook (3-4h) — free, written by ex-McKinsey/Bain consultants. Covers 100-day plan, workstream organisation, synergy tracking. IT integration section is directly relevant
- Read *Mergers and Acquisitions in the Software Industry* by Karl Michael Popp (6-8h) — specifically for software company DD. Covers IP assessment, architecture evaluation, technical risk. Based on real acquisition experience
- Study integration patterns: lift-and-shift, re-platform, rip-and-replace, co-existence. Know the cost and timeline for each
- Optional deep dive: *M&A Information Technology Best Practices* by Roehl-Anderson (~EUR 70, 10-12h) — the most comprehensive resource, with companion checklists

**Resources:**
- Umbrex Post-Merger Integration Playbook — https://umbrex.com/wp-content/uploads/2023/06/Umbrex-Post-Merger-Integration-Playbook-First-Edition.pdf (free PDF, immediately actionable)
- Book: *Mergers and Acquisitions in the Software Industry* (Karl Michael Popp) — ~EUR 30
- Book: *M&A Information Technology Best Practices* (Roehl-Anderson, Wiley Finance) — ~EUR 70, with checklists
- Crosslake Technologies blog — https://crosslaketech.com/insights/ (free, post-acquisition integration articles)

### 3.2 Industry Benchmarking (6h)
**Current level:** 2/5. Covers Dimension 5.
**Target:** Can benchmark a company's technology spend, team size, and architecture maturity against industry peers.

- Build a personal benchmark reference sheet covering: tech spend as % of revenue (by industry + company size), engineering team ratios (by stage), cloud cost per revenue band, DORA metric percentiles
- Key sources to download and study: Flexera (free), Deloitte CIO Survey (free). Gartner requires subscription — check if accessible via university library or free excerpts

**Resources:**
- Flexera State of IT Report 2025/2026 — https://www.flexera.com/blog/it-assets/it-spend-report/ (free download, annual)
- Deloitte CIO Survey — https://www.deloitte.com/global/en/our-thinking/insights/topics/leadership/global-technology-leadership-survey.html (free annual)
- Gartner IT Key Metrics Data — subscription required but frequently excerpted in vendor reports. Check if accessible via IE library or similar
- Perspective Partners engineering benchmarking — search for their annual reports on engineering team ratios

### 3.3 PE 100-Day Plan Frameworks (6h)
**Current level:** 3/5. Covers Dimension 7.
**Target:** Can produce a technology-specific 100-day plan that aligns with how PE operating partners think.

- Read the OPX Partners 100-day whitepaper (1-2h) — structured framework showing how DD findings translate into Day 1 priorities and value creation roadmap
- Read Hello Operator's greatest hits (2-3h) — Paul Stansik (ParkerGale, mid-market B2B software PE). Key posts: "What Does An Operating Partner Do?", "Let's Get Real About Value Creation", "The Weekly Sales Metrics Playbook", "How To Work With An Operating Partner". His "Less Data, More Often" framework is directly applicable to DD recommendations
- Structure a technology-specific 100-day plan: Week 1-2 (security/risk), Week 3-6 (cost reduction/quick wins), Week 7-12 (foundation building)

**Resources:**
- OPX Partners: "The First 100 Days: Crafting a Value Creation Plan" — https://assets.ctfassets.net/ua7k6fw2m72i/3LfP6llmxva5t5NfSlhTcd/12ac4f2fe8420ea293ab17a2deaac325/The_First_100_Days_--_Crafting_a_Value_Creation_Plan__OPX_Partners_perspective_.pdf (free PDF)
- Hello Operator Greatest Hits — https://hellooperator.substack.com/p/this-is-the-best-of-hello-operator (free)
- Also: https://hellooperator.com/ (full archive)

---

## Phase 4: Practice (20h)

### 4.1 Mock DD — Full Framework (15h)
- Pick a publicly traded mid-market SaaS company (or well-documented PE-backed company)
- Run the full 7-dimension framework using public information:
  - Annual reports, investor presentations (architecture hints, cost data)
  - Job postings on LinkedIn/Greenhouse (team size, composition, tech stack)
  - BuiltWith/StackShare (technology stack)
  - Glassdoor reviews (engineering culture, management quality)
  - Security headers check, SSL Labs test (basic security posture)
  - Crunchbase/PitchBook (financial data, funding, growth)
- Produce scores for all 7 dimensions
- Estimate cost-to-fix for identified issues
- Build 90-day + 12-month value creation roadmap

### 4.2 Write Full DD Report (5h)
- Use the report template (`06-dd-report-template.md`)
- Write up mock DD findings as a complete report
- Produce executive summary with risk scorecard and recommendation
- Compare to the sample report (`06-sample-dd-report.pdf`) — is yours at the same depth?
- This becomes a second portfolio sample (different sector from the illustrative report)

---

## Track A: PE Conversational Fluency (40h, parallel with Phases 1-4)

Not required for the DD itself, but required to not sound like an outsider when talking to operating partners. Run alongside Phases 1-4 at ~5h/week.

### A1. Deal Mechanics (10h)
**Why:** Speak the language of fund economics.

- Fund structure: GP/LP split, management fees (2%), carried interest (20%), hurdle rates
- Fund lifecycle: fundraising → deployment → value creation → exit → distribution
- Commitment periods, vintage years, J-curve
- Co-investment structures, continuation vehicles, secondaries

**Resources:**
- Book: *The Masters of Private Equity and Venture Capital* (Finkel) — Chapters 1–6
- Podcast: *Private Equity Funcast* — 10 recent episodes
- Podcast: *10X Capital* — PE operating partner interviews
- Newsletter: *Road to Carry* (penewsletter.com) — subscribe, read back catalog

### A2. LBO Fundamentals (10h)
**Why:** Understand how PE firms think about value creation and how technology spend appears in the model.

- Learn Paper LBO first (1h) — do an LBO on the back of a napkin: entry equity, debt paydown, exit equity, IRR. This is the mental model that drives every PE investment decision
- Walk through the Macabacus short-form LBO template in Excel (3-4h) — see the structure without building from scratch. Understand sources & uses, debt tranches, entry/exit multiples, EBITDA adjustments
- Understand how technology spend classification (capex/opex) flows through the LBO model — this is where your DD findings directly affect the deal price

**Resources:**
- WSP Paper LBO — https://www.wallstreetprep.com/knowledge/paper-lbo/ (free, the 5-minute mental model)
- WSP Simple LBO Model — https://www.wallstreetprep.com/knowledge/financial-modeling-quick-lesson-simple-lbo-model/ (free, with video)
- Macabacus LBO Overview — https://macabacus.com/valuation/lbo-overview (free, derived from bulge bracket models)
- Macabacus LBO Templates — https://macabacus.com/lbo-model/templates (free, downloadable Excel)
- Macabacus Value Creation — https://macabacus.com/valuation/lbo-creating-value (free, explains the 3 levers)
- Book: *Investment Banking* (Rosenbaum & Pearl) — LBO chapter only, if you want textbook depth

### A3. Value Creation Plans (10h)
**Why:** Technology DD feeds directly into the value creation plan.

- Three levers: operational improvement, revenue growth, multiple expansion
- How operating partners think: 100-day plans, KPI dashboards, management assessment
- Where technology fits: cost reduction, revenue enablement, data/analytics, automation
- Portfolio-level technology strategy

**Resources:**
- McKinsey: "Creating Value in Private Equity" report (free)
- Bain: Private Equity Annual Report 2025/2026 (free)
- Newsletter: *Hello Operator* by Paul Stansik — read full back catalog
- Book: *The Private Equity Playbook* (Adam Coffey)

### A4. IC Process & DD Workflow (10h)
**Why:** Understand how your DD report gets consumed and what decisions it influences.

- Study the full PE deal process on Street of Walls (3-4h) — sourcing → screen → CIM → management meeting → LOI → DD → PIM (30-40 pages) → IC presentation → FIM → close. Critically: where tech DD fits (between LOI and FIM) and what the IC expects to see
- Read the Addepar/Stanford IC memo research brief (2-3h) — based on 54 institutional investors + 6 case studies. How IC memos actually function. Standard sections, processes, decision patterns
- Understand IC memo structure: Executive Summary, Company Overview, Market, Financial Analysis, Risks/Mitigants, Deal Structure — and where your tech DD findings slot in
- Ask Lorenzo about CTAIMA's DD experience with Hg Capital — first-hand account

**Resources:**
- Street of Walls: PE Investment Process — https://www.streetofwalls.com/finance-training-courses/private-equity-training/private-equity-investment-process/ (free, the most comprehensive free resource)
- Street of Walls: Full PE Guide — https://www.streetofwalls.com/guides-menu/private-equity/ (free, 8-10h for everything)
- Addepar/Stanford: "Investment Memos and Decision-Making" — https://longterminvesting.stanford.edu/sites/g/files/sbiybj23856/files/media/file/addepar-investment-memos-and-decision-making.pdf (free PDF, rigorous)
- Carta: Investment Memo Guide — https://carta.com/learn/private-funds/management/portfolio-management/investment-memo/ (free)
- Sergio Marrero IC Memo breakdown — https://medium.com/rbl1/the-investment-committee-memorandum-78b40bc1bd08 (free, best practitioner breakdown)

---

## Track B: Secondary Depth (learn on-the-job after first engagement)

| Topic | Hours | When | Covers |
|-------|:-----:|------|--------|
| Data governance (DAMA-DMBOK deep) | 6h | After engagement 1 | Dim 4 |
| Developer productivity (Space framework, McKinsey) | 4h | After engagement 1 | Dim 2 |
| MLOps maturity (Google model) | 3h | After engagement 1 | Dim 4 |
| Conway's Law formal assessment | 4h | After engagement 2 | Dim 2 |
| Master data management | 4h | After engagement 2 | Dim 4 |
| UK/EU engineering salary benchmarks | 4h | Before first UK engagement | Dim 2 |
| AWS Solutions Architect cert | 40h | Q3 2026 | Dims 1, 5 |
| CIO/CTO Frameworks (TOGAF, COBIT) | 20h | Q3-Q4 2026 | Dim 1 |
| AI Strategy deep track | 32h | Q4 2026 | Dim 4 |

---

## Track C: Market Intelligence (ongoing, 2-3h/week)

### Subscribe & read weekly
- **Hello Operator** (Paul Stansik, ParkerGale) — Substack, free. Gold standard
- **Road to Carry** — penewsletter.com, free. Deal case studies
- **Alt Goes Mainstream** (Broadhaven) — Substack, free. 13,700+ subs
- **G3NR8 Operational Alpha** — email, free. AI for PE operating partners
- **Growth Shuttle Insider** (Mario Peshev) — Substack
- **PE Wire Operating Partners** — Private Equity Wire, free

### Follow on LinkedIn
- Crosslake Technologies team
- West Monroe PE practice
- Paul Stansik (ParkerGale)
- Jeff Chavez (Crosslake)
- Axel Tombereau (solo DD practitioner)

### Monitor weekly
- CTO Market Tracker with PE DD-specific searches
- LinkedIn Sales Navigator: "operating partner" + "technology" in UK

---

## Weekly Schedule (Weeks 1-10)

| Week | Phase work (11h) | Track A (5h) | Track C | Key milestone |
|------|-----------------|-------------|---------|---------------|
| 1 | Phase 1: OWASP (8h) + SOC 2 start (3h) | A1 Deal Mechanics (5h) | Subscribe to all newsletters | |
| 2 | Phase 1: SOC 2 (7h) + Pentest reports (4h) | A1 (3h) + A4 IC Process (2h) | First weekly review | Can explain fund structure in conversation |
| 3 | Phase 1: GDPR/NIS2 (6h) + IAM (5h) | A2 LBO (5h) | | |
| 4 | Phase 1: Incident response (3h) + Practice (2h). Phase 2: DORA (6h) | A2 (3h) + A3 Value Creation (2h) | | Security dimension: 1.9→3.0 |
| 5 | Phase 2: FinOps (8h) + Capex/opex (3h) | A3 (5h) | | |
| 6 | Phase 2: Capex/opex (1h) + Tech debt quant (6h) + Cost-to-fix practice (4h) | A3 (3h) + A4 (2h) | | Can produce a cost-to-fix estimate |
| 7 | Phase 3: M&A integration (8h) + Benchmarking start (3h) | A4 (5h) | | Track A complete |
| 8 | Phase 3: Benchmarking (3h) + 100-day plans (6h) | — | | All frameworks learned |
| 9 | Phase 4: Mock DD (11h) | — | | |
| 10 | Phase 4: Mock DD (4h) + Write report (5h) | — | | **DD-READY** |

**Total per week:** ~16h learning + ~24h pipeline/execution work

---

## Milestones

| Week | Milestone | Test |
|------|-----------|------|
| 2 | PE conversational fluency (basic) | Can explain fund structure, carried interest, IC process to a non-PE person |
| 4 | Security gap closed to 3.0/5 | Can read a pentest report and explain findings in business terms |
| 6 | Cost dimension formalised | Can produce a phased cost-to-fix estimate with benchmarks |
| 7 | Track A complete | Can hold a 30-minute conversation with any PE professional without revealing knowledge gaps |
| 8 | All frameworks learned | Can describe the assessment approach for all 7 dimensions with specific tools and benchmarks |
| 10 | **Mock DD complete** | Have a full DD report produced from the framework. Ready for first engagement |
| 14 | Track B started (on-the-job) | Learning data governance, developer productivity, MLOps from real engagement data |
| 24 | AWS SA certified | Cloud architecture credibility signal |
