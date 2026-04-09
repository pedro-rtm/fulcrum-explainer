# Knowledge Gap Analysis — Can Pedro Deliver This DD?

**Date:** April 2026
**Purpose:** Honest assessment of current capability vs. what each DD dimension requires

---

## Scoring

| Level | Meaning | Can you assess this in a DD? |
|:-----:|---------|------------------------------|
| **5** | Deep practitioner | Yes — you've done this repeatedly and can score it with confidence |
| **4** | Strong working knowledge | Yes — you can assess it, may need to reference frameworks for edge cases |
| **3** | Intermediate | Partially — you understand the concepts but haven't formally assessed them. Need prep before engagement |
| **2** | Awareness | No — you know what it is but can't credibly score it yet. Study required |
| **1** | Gap | No — new territory. Structured learning needed |

---

## Dimension 1: Architecture & Infrastructure

| Sub-area | Pedro now | Evidence | Gap to close |
|----------|:--------:|---------|--------------|
| Cloud maturity assessment | **3** | Used AWS/Azure/GCP across projects. Built on cloud but hasn't formally assessed cloud maturity at architecture level | Learn AWS Well-Architected Framework. Run it against a real system. ~8h |
| System topology evaluation | **4** | Built/integrated monoliths, ERPs, IoT systems, APIs across 80+ engagements. Understands how systems connect | Formalize vocabulary: learn TOGAF taxonomy for describing architecture patterns. ~4h |
| Technical debt quantification | **3** | Has identified and fixed tech debt repeatedly. Hasn't used formal quantification models (CAST, SIG) | Learn CAST/SIG scoring models. Practice quantifying debt in GBP on 2-3 Velkan cases. ~6h |
| Scalability assessment | **3** | Understands when systems break (lived it). Hasn't formally modeled scalability ceilings | Learn load testing concepts, horizontal vs vertical scaling patterns. ~4h |
| SPOFs identification | **4** | Has built redundant systems (99.8% uptime). Knows what fails | Minimal gap. Formalize into a checklist. ~2h |
| Third-party dependency audit | **3** | Has managed vendor relationships. Hasn't done formal vendor lock-in assessment | Build a vendor risk checklist. ~2h |

**Dimension 1 overall: 3.3/5 — Credible with 2-3 weeks of prep**

---

## Dimension 2: Team & Organisation

| Sub-area | Pedro now | Evidence | Gap to close |
|----------|:--------:|---------|--------------|
| Engineering headcount/composition analysis | **4** | Built and managed technical teams across 80+ engagements. Knows what good looks like | Formalize into ratios and benchmarks. ~2h |
| Key-person risk assessment | **4** | Has encountered and mitigated this repeatedly. Built handoff processes | Create a scoring rubric. ~2h |
| Outsourcing evaluation | **4** | Has managed outsourced teams. Understands cost/quality/IP tradeoffs | Minimal gap |
| Hiring plan validation | **3** | Has hired across multiple companies. Less familiar with UK/EU tech hiring market rates and timelines | Research current UK engineering salary benchmarks and hiring timelines. ~4h |
| Conway's Law assessment | **3** | Understands org→architecture relationship intuitively. Hasn't used it as a formal assessment tool | Read Team Topologies (skim). Formalize into assessment questions. ~4h |
| DORA metrics interpretation | **2** | Knows what deployment frequency and lead time mean. Hasn't measured them formally or benchmarked them | Study DORA State of DevOps Report. Learn what "elite" vs "low" performers look like. ~6h |
| Developer productivity assessment | **2** | Managed developers but hasn't used formal productivity frameworks | Read McKinsey "Measuring Developer Productivity." Learn Space framework. ~4h |

**Dimension 2 overall: 3.1/5 — Credible with targeted prep on DORA + productivity metrics**

---

## Dimension 3: Security & Compliance

| Sub-area | Pedro now | Evidence | Gap to close |
|----------|:--------:|---------|--------------|
| OWASP Top 10 assessment | **2** | Awareness-level. Knows what SQL injection and XSS are. Hasn't assessed systems against OWASP formally | Study OWASP Top 10 (2025). Learn how to identify each in a codebase review. ~8h |
| SOC 2 readiness assessment | **1** | New territory. Hasn't worked with SOC 2 | Learn SOC 2 trust service criteria. Study a SOC 2 gap analysis template (Vanta/Drata). ~10h |
| GDPR/NIS2 compliance evaluation | **2** | General awareness. Hasn't assessed compliance formally | Study GDPR assessment checklist for technology systems. Read NIS2 requirements (ENISA). ~6h |
| Penetration test interpretation | **2** | Knows what pentests are. Hasn't read a full pentest report or interpreted CVSS scores | Read 2-3 sample pentest reports. Learn CVSS v3.1 scoring. ~4h |
| IAM maturity assessment | **2** | Has set up access controls (Azure AD, Google Workspace). Hasn't assessed IAM formally at security depth | Learn IAM maturity model. Study common IAM failures. ~4h |
| Incident response evaluation | **2** | Has dealt with incidents operationally. Hasn't assessed incident response plans formally | Study NIST incident response framework. Build assessment checklist. ~4h |
| Third-party security risk | **2** | Vendor management experience but not security-specific assessment | Learn vendor security questionnaire patterns. ~2h |

**Dimension 3 overall: 1.9/5 — THIS IS THE BIGGEST GAP. Needs 30-40h of focused study before first engagement**

---

## Dimension 4: Data & Analytics

| Sub-area | Pedro now | Evidence | Gap to close |
|----------|:--------:|---------|--------------|
| Data quality assessment | **3** | Built data pipelines (Waffle: 5M+ items). Understands data quality issues. Hasn't used formal assessment frameworks | Learn DAMA-DMBOK quality dimensions. Build scoring rubric. ~4h |
| Data governance maturity | **2** | Awareness-level. Hasn't assessed governance formally | Study DAMA-DMBOK governance framework. Learn maturity models. ~6h |
| Integration health evaluation | **4** | Built 4 ERP integrations, 20+ app integrations. Knows what breaks | Formalize into assessment checklist. ~2h |
| AI readiness scoring | **4** | Built production AI (RAG, LLMs, vector DBs). Can assess AI infrastructure credibly | Build a scoring rubric based on own experience. ~2h |
| MLOps maturity assessment | **3** | Built ML pipelines at Waffle. Less familiar with formal MLOps maturity models | Study Google MLOps maturity model. ~3h |
| Master data management | **2** | Understands the concept. Hasn't assessed MDM implementations | Study MDM assessment patterns. ~4h |

**Dimension 4 overall: 3.0/5 — Credible, especially on AI. Data governance needs work**

---

## Dimension 5: Cost Structure

| Sub-area | Pedro now | Evidence | Gap to close |
|----------|:--------:|---------|--------------|
| Total spend analysis | **4** | Has managed technology budgets across 80+ engagements. Reported to CEO/Board | Formalize into a decomposition template. ~2h |
| Cloud cost optimization | **3** | Used AWS/Azure/GCP. Understands billing. Hasn't done deep FinOps analysis | Study FinOps Foundation framework. Learn reserved instances, right-sizing, cost allocation. ~8h |
| License audit | **3** | Has managed SaaS subscriptions and ERP licenses. Hasn't done formal audit at DD level | Build a license audit checklist. ~2h |
| Cost-to-fix estimation | **3** | Has estimated project costs repeatedly. Less familiar with PE-style phased remediation costing | Practice building 3 cost-to-fix estimates using Velkan portfolio data. ~6h |
| Benchmarking vs industry | **2** | Knows own costs. Doesn't have industry benchmark datasets | Study Gartner IT Key Metrics, Flexera State of IT, Deloitte CIO Survey. ~6h |
| Capex/opex classification | **2** | New in PE context. Critical: how technology spend is classified affects EBITDA and valuation | Study capex vs opex rules for technology spend. Critical for PE conversations. ~4h |

**Dimension 5 overall: 2.8/5 — Good instincts, but needs formal frameworks especially on benchmarking and capex/opex**

---

## Dimension 6: Delivery Capability

| Sub-area | Pedro now | Evidence | Gap to close |
|----------|:--------:|---------|--------------|
| CI/CD maturity assessment | **3** | Has used CI/CD (GitHub Actions, various). Hasn't formally assessed pipeline maturity | Study CI/CD maturity models. Learn what to check in a pipeline review. ~4h |
| QA practices evaluation | **3** | Has managed QA processes. Understands testing types. Hasn't benchmarked formally | Learn test coverage benchmarks, testing pyramid, E2E vs unit trade-offs at assessment level. ~3h |
| DevOps maturity assessment | **2** | Used DevOps tools. Hasn't used formal maturity frameworks | Study DevOps maturity model (DORA + capability catalog). ~6h |
| Backlog health evaluation | **3** | Has managed product backlogs. Understands prioritization | Formalize into assessment criteria (age distribution, debt ratio, velocity). ~2h |
| Incident management assessment | **3** | Has dealt with incidents. Built operational protocols | Study MTTR benchmarks, on-call maturity patterns. ~2h |
| Release cadence analysis | **2** | Understands deployment concepts. Hasn't benchmarked release frequency formally | Learn DORA deployment frequency benchmarks by performance tier. ~2h (overlaps with Dim 2) |

**Dimension 6 overall: 2.7/5 — Needs formal DevOps/DORA framework knowledge. ~15-20h**

---

## Dimension 7: Strategic Alignment

| Sub-area | Pedro now | Evidence | Gap to close |
|----------|:--------:|---------|--------------|
| Technology roadmap evaluation | **4** | Has built and evaluated technology roadmaps across 80+ engagements | Minimal gap. Formalize criteria. ~2h |
| M&A integration readiness | **2** | No M&A integration experience. New territory for PE context | Study post-acquisition technology integration playbooks (Crosslake, Beyond M&A content). ~8h |
| Competitive technology moat assessment | **4** | Has evaluated technology positioning. Built products (Waffle). Understands defensibility | Minimal gap |
| Innovation pipeline evaluation | **3** | Has built R&D capability. Less formal in assessment mode | Build assessment criteria. ~2h |
| First-100-day technology planning | **3** | Has built 90-day roadmaps repeatedly. Hasn't done it in PE post-acquisition context specifically | Study PE 100-day plan frameworks (Hello Operator, PEI content). ~6h |

**Dimension 7 overall: 3.2/5 — Credible except for M&A integration readiness**

---

## Summary Heatmap

| Dimension | Current level | Hours to credible | Priority |
|-----------|:------------:|:-----------------:|:--------:|
| 1. Architecture | 3.3 | ~26h | Medium |
| 2. Team | 3.1 | ~22h | Medium |
| **3. Security** | **1.9** | **~38h** | **CRITICAL** |
| 4. Data | 3.0 | ~21h | Medium |
| 5. Cost | 2.8 | ~28h | High |
| 6. Delivery | 2.7 | ~19h | High |
| 7. Strategic | 3.2 | ~18h | Medium |
| **Total** | **2.9** | **~172h** | |

---

## Honest Assessment

**Can Pedro do a DD today?** Partially. Dimensions 1, 2, 4, 7 are close enough. The track record of 80+ transformations provides genuine depth in identifying what's broken and estimating what it costs to fix.

**Where he'd embarrass himself:** Security (Dimension 3) is the critical gap. An operating partner who asks "what did you find on SOC 2 readiness?" or "walk me through the CVSS scores from the pentest" would expose the gap immediately. Security is also the dimension PE firms care about most after a string of high-profile breaches at portfolio companies.

**Where he'd shine:** AI readiness (Dimension 4), team assessment (Dimension 2), architecture intuition (Dimension 1), cost quantification (Dimension 5 — the instincts are there, just needs formal frameworks), and strategic alignment (Dimension 7).

---

## Recommended Sequence (fastest path to "credible DD")

### Phase 1: Make Security Non-Embarrassing (38h, 3 weeks)
This is the gating factor. No DD is credible without security assessment.
1. OWASP Top 10 deep study — 8h
2. SOC 2 trust service criteria + gap analysis template — 10h
3. Read 3 real pentest reports, learn CVSS scoring — 4h
4. GDPR/NIS2 assessment checklists — 6h
5. IAM maturity + incident response frameworks — 8h
6. Practice: assess one Velkan system's security posture — 2h

### Phase 2: Formalize What You Already Know (30h, 2 weeks)
Turn intuition into structured, repeatable assessment.
1. DORA metrics + DevOps maturity model — 8h
2. FinOps + cloud cost optimization — 8h
3. Capex/opex classification for PE — 4h
4. Technical debt quantification (CAST/SIG) — 6h
5. Cost-to-fix estimation practice (3 Velkan cases) — 4h

### Phase 3: Fill PE-Specific Gaps (20h, 2 weeks)
What makes this DD and not just technology assessment.
1. M&A integration readiness — 8h
2. Industry benchmarking (Gartner, Flexera, Deloitte) — 6h
3. PE 100-day plan frameworks — 6h

### Phase 4: Practice (20h)
1. Mock DD against a public company using full framework — 15h
2. Write up findings as a full report using the template — 5h

**Total: ~108h of focused work over 8-10 weeks to be credibly ready for the first DD engagement.**

The remaining ~64h from the full 172h estimate are nice-to-have depth (data governance, developer productivity frameworks, MLOps maturity) that can be learned on-the-job after the first engagement.

---

## The Shortcut

Pedro doesn't need to be an expert in all 7 dimensions alone. The "firm of one" problem has a solution:

**For the first 2-3 engagements, subcontract the security dimension** to a specialist (ex-CISO, penetration tester, compliance consultant) at GBP 800-1,200/day for 2-3 days per engagement. This is exactly what Crosslake does — they have specialist teams per dimension. Pedro runs the engagement, the security specialist handles Dimension 3, Pedro learns from them, and by engagement 4-5, Pedro can handle security assessment independently.

Cost: ~GBP 2-3K per engagement. Worth it to avoid credibility risk on the hardest dimension while learning.
