# Engagement Plan: {Customer Name}

> **What is this?** The strategy document for a single sales opportunity. It plans the full engagement journey — typically multiple visits — to advance the opportunity from Prospect through Closed/Launched.
>
> 🤖 *Automatically created and updated by the AI agent. Generated even from a single call plan request — every opportunity deserves a strategic wrapper.*
>
> ✅ *After generating or updating, agent always asks sales to review and revise as needed.*

| Field | Value |
|---|---|
| **Status** | Draft / Active / Closed |
| **Last Updated** | YYYY-MM-DD |
| **Opportunity Owner** | {name} |

---

## 1. Opportunity Context

> *💡 Sales provides: customer name, opportunity name, deal value, close date. Agent researches and fills the rest. Always confirm with sales.*
>
> 🚧 *Planned: When Account Analysis and Opportunity Management references are available, agent auto-loads their insights here — populating industry context, financial profile, strategic priorities, competitive landscape, and opportunity health assessment. This becomes the single source of account intelligence for all downstream documents.*

| Field | Value |
|---|---|
| **Customer** | {company name} |
| **Industry / Segment** | {e.g., Financial Services / Enterprise} |
| **Opportunity Name** | {opportunity name} |
| **Estimated Deal Value** | {ARR or TCV} |
| **Target Close Date** | {YYYY-MM-DD or target quarter} |

### Why Now

| Dimension | Details |
|---|---|
| **Trigger Event** | {What made the customer start paying attention now?} |
| **Business Pain** | {What problem are they trying to solve?} |
| **Desired Outcome** | {What does success look like for the customer?} |
| **Cost of Inaction** | {What happens if they do nothing?} |

---

## 2. Stakeholder Map

> *💡 Initially built from Call Plan attendees. Auto-updated from each PMR (sentiment, last interaction). Agent asks sales to confirm and add missing stakeholders.*

### Overview

| Name | Title | Role | Sentiment | Last Touch |
|---|---|---|---|---|
| {name} | {title} | EB | Supportive / Neutral / Against / Unknown | {YYYY-MM-DD} |
| {name} | {title} | Champion | | |
| {name} | {title} | Influencer | | |
| {name} | {title} | User | | |

> *Roles: EB (Economic Buyer) · Champion · Decision Maker · Influencer · Technical Evaluator · Blocker · User*

### Stakeholder Details

> *One paragraph per key stakeholder. Cover the following:*
>
> *1. **Focus Area & Priorities** — What they care about most; their current initiatives and KPIs*
> *2. **Decision Influence** — How much weight they carry in this deal; who they influence or report to*
> *3. **Relationship Status** — Who owns the relationship on the AWS side; depth of engagement (High/Med/Low); history of interactions*
> *4. **Engagement Notes** — Key things to know: preferences, concerns, sensitivities, what resonates with them, what to avoid*
> *5. **For executive-level stakeholders:** Integrate CXO Persona insights (per Rule 6) into the above dimensions*

**{Name}**, {Title} — {Role}

> *{One focused paragraph covering the 4 dimensions above. For executive-level stakeholders, also integrate CXO Persona insights per Rule 6.}*

**Example:**

> **Li Wei**, VP of Engineering — Technical Evaluator
>
> Li Wei's primary focus is modernizing the company's data infrastructure and reducing deployment cycle times from weeks to days. He reports directly to the CTO and carries significant weight in technology selection decisions — the CTO typically follows his technical recommendations. AWS relationship is owned by our SA (Zhang Ming), who has met Li Wei twice (last: 2026-03-15). Engagement is medium — he's open to AWS but cautious about migration complexity. He prefers deep technical conversations with concrete architecture diagrams; avoid high-level marketing slides. Key concern: data sovereignty and compliance with local regulations. He responded positively to our Graviton performance benchmarks in the last meeting.

### Power Structure Notes

> *{Decision-making hierarchy, relationships between key people, internal politics, coalition dynamics, who influences whom, potential blockers...}*

---

## 3. Competitive Position

> *💡 Agent builds from sales input + research. Auto-updated from PMR "What Changed" section.*

| Field | Value |
|---|---|
| **Current Landscape** | {Incumbent / Greenfield / Multi-cloud} |
| **Key Competitors** | {who's in play} |
| **Win Theme** | {Our core differentiator for this deal} |

### Competitor Analysis

| Competitor | Strengths | Weaknesses | Our Counter |
|---|---|---|---|
| {competitor} | {their advantages} | {their gaps} | {how we win against them} |

### MEDDPICC Tracker

> *💡 Auto-updated after each PMR. Agent highlights gaps and suggests questions for the next Call Plan. **Gap questions in the "Gap / Next Question" column automatically flow into the next Call Plan's Information Exchange section (Section 4)** — agent should reference these when generating discovery questions.*

| Element | Known Information | Gap / Next Question | Status |
|---|---|---|---|
| Metrics | | | 🔴🟡🟢 |
| Economic Buyer | | | 🔴🟡🟢 |
| Decision Criteria | | | 🔴🟡🟢 |
| Decision Process | | | 🔴🟡🟢 |
| Paper Process | | | 🔴🟡🟢 |
| Identified Pain | | | 🔴🟡🟢 |
| Champion | | | 🔴🟡🟢 |
| Competition | | | 🔴🟡🟢 |

**Example:**

| Element | Known Information | Gap / Next Question | Status |
|---|---|---|---|
| Identified Pain | CFO concerned about margin erosion — revenue +7.5% but profit -4.2%. Finance team spending 80% of time on reporting, no capacity for strategic analysis. | Validate: Is this a funded initiative or exploratory? What's the CFO's timeline expectation? | 🟡 |
| Economic Buyer | CFO is the initial contact. Likely EB for finance-function investments. | Confirm: Does CFO have budget authority for this type of investment? What's the approval threshold? Does CEO need to sign off? | 🟡 |
| Champion | CFO expressed interest in AI for finance — potential champion. | Validate: Is CFO willing to champion internally? Or evaluating on behalf of someone else? | 🟡 |
| Decision Process | Unknown — SOE, likely structured procurement. | Ask: "How does Weichai typically evaluate and adopt new technology? Who else would be involved?" | 🔴 |

---

## 4. Value Proposition

> *💡 Agent drafts based on opportunity context and research. Sales reviews and refines.*

| Customer Pain | Our Value Proposition | Solution / Approach | Proof / Case Study |
|---|---|---|---|
| {pain point 1} | {how we address it} | {specific AWS solution} | {evidence} |
| {pain point 2} | {how we address it} | {specific AWS solution} | {evidence} |
| {pain point 3} | {how we address it} | {specific AWS solution} | {evidence} |

**Example:**

| Customer Pain | Our Value Proposition | Solution / Approach | Proof / Case Study |
|---|---|---|---|
| Monthly close takes 15+ days, finance team at capacity | Compress close cycle to 3-5 days, freeing 30% of team capacity for strategic analysis | Amazon Bedrock for document processing + Lambda for workflow automation + QuickSight for automated reporting | [Similar manufacturer] reduced close from 12 days to 4 days, saving 2,400 hours/year |
| Forecast accuracy at 65%, board losing confidence | ML-powered predictive forecasting incorporating market signals and operational data, targeting 85%+ accuracy | Amazon SageMaker for forecasting models + S3 data lake for unified financial data | [Industrial company] improved forecast accuracy from 60% to 88% in 6 months |

---

## 5. Engagement Roadmap

> *⭐ The master plan + actual record. Each row maps to one Call Plan → one PMR. Agent auto-updates Actual Date, Actual Outcome, and Link after each PMR. Agent matches rows by Customer Name + Meeting Date from the Call Plan/PMR.*

| # | Milestone | Stage | Target Date | Actual Date | Key Activity | Expected Outcome | Actual Outcome | Participants | Link | Status |
|---|---|---|---|---|---|---|---|---|---|---|
| 1 | {e.g., Discovery Call} | {e.g., Prospect} | {date} | | {Validate opp} | {Champion identified} | | {CTO / AM, SA} | {Call Plan + PMR} | Planned / Done |
| 2 | {e.g., Technical Workshop} | | | | | | | | | Planned |
| 3 | {e.g., POC Review} | | | | | | | | | Planned |
| 4 | {e.g., Business Case} | | | | | | | | | Planned |
| 5 | {e.g., Contract Negotiation} | | | | | | | | | Planned |

---

## 6. Risk Register

> *💡 Agent identifies risks from PMR findings and sales input. Sales reviews and confirms.*

| Risk | Likelihood | Impact | Mitigation | Owner | Status |
|---|---|---|---|---|---|
| {e.g., Budget freeze in Q4} | High / Med / Low | High / Med / Low | {e.g., Accelerate POC to lock commitment} | {name} | Open / Mitigated / Closed |
| {e.g., Champion leaves} | | | {Build relationships with multiple stakeholders} | | Open |

---

*Version: 2.0 | Last updated: 2026-04-17 | Part of the Customer Engagement Closed-Loop Flow*
