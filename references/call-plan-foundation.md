# Call Plan — Foundation Template

> **Purpose:** Prepares AWS sales team members before external customer meetings. AI agent generates the Call Plan based on sales input, Engagement Plan context, and scenario guidance.
>
> ✅ *After generating, agent always asks sales to review and revise as needed.*

---

## 1. Meeting Details

> *💡 **Minimum required from sales:** Customer name, attendee names + titles, meeting objective (per SKILL.md Section 4). Agent infers or researches the rest. Date/time/location may not be confirmed yet — mark as `[待确认]` if unknown. Decision roles may be unknown for first meetings — mark as `[待确认]` and add a discovery question in Section 4 to clarify. Agent pulls opportunity context from Engagement Plan if one exists.*

| Field | Value |
|---|---|
| **Date & Time** | `{date}` `{time}` `{timezone}` |
| **Duration** | `{duration}` |
| **Format** | `{In-person / Virtual / Hybrid}` |
| **Location / Link** | `{location or meeting link}` |
| **Opportunity Name** | `{auto from Engagement Plan}` |
| **Current Sales Stage** | `{auto from Engagement Plan}` |

### Customer Attendees

| Name | Title | Role in Decision |
|---|---|---|
| `{name}` | `{title}` | `{EB / Champion / Decision Maker / Influencer / Evaluator / End User}` |
| `{name}` | `{title}` | |
| `{name}` | `{title}` | |

### AWS Attendees

| Name | Title | Role in Meeting |
|---|---|---|
| `{name}` | `{title}` | `{Lead / Support / SME / Executive Sponsor}` |

---

## 2. Target Meeting Outcomes

> *💡 Agent drafts based on scenario guidance, current sales stage, and Engagement Plan roadmap. Sales reviews and adjusts.*
>
> *The user's stated meeting objective takes priority. Agent then cross-references the current stage's **exit criteria** (from meddpicc-stage-mapping.md) and suggests additional outcomes that align with advancing to the next stage. If the user's objectives miss a critical exit criteria dimension, agent should flag it as a suggestion.*

| # | Customer Perspective | Our Perspective |
|---|---|---|
| 1 | `{what the customer hopes to achieve}` | `{what we need to achieve}` |
| 2 | `{outcome}` | `{outcome}` |

**Example (Scenario 1 — Prospect stage):**

| # | Customer Perspective | Our Perspective |
|---|---|---|
| 1 | Understand how AI can address their finance team's capacity constraints | Validate whether the CFO's interest in AI is tied to a real, funded initiative or exploratory curiosity |
| 2 | See relevant proof points from similar manufacturing companies | Identify a potential champion and understand the decision process for technology investments |

**Target Stage Progression:** ( `{current stage}` ) → ( `{target stage}` )

---

## 3. Success Criteria

> *💡 Agent drafts dual-perspective criteria. These will be auto-pulled into the PMR Outcome Assessment after the meeting.*
>
> *Criteria must be **observable and assessable** — something you can clearly judge as achieved or not after the meeting. Avoid vague or subjective criteria.*
>
> *If sales provides criteria that are too vague, offer a concrete example to guide them:*
> - ❌ Too vague: "Customer is interested"
> - ✅ Assessable: "Customer agrees to schedule a follow-up technical deep-dive within 2 weeks"
> - ❌ Too vague: "Good conversation"
> - ✅ Assessable: "Customer shares their current vendor contract timeline and budget cycle"

| # | Customer Would Consider It Successful If… | We Would Consider It Successful If… |
|---|---|---|
| 1 | `{criterion}` | `{criterion}` |
| 2 | `{criterion}` | `{criterion}` |
| 3 | `{criterion}` | `{criterion}` |

---

## 4. Information Exchange

> *💡 Agent auto-selects MEDDPICC elements based on current sales stage (see Scenario Guidance), plus other deal-specific needs from Engagement Plan gaps. Questions and delivery items must be tailored to the specific meeting objectives defined in Section 2 — not generic. Agent should proactively suggest questions and talking points that directly serve the target outcomes.*
>
> *For every Call Plan, agent must prepare **industry-relevant use cases** and **customer references** matched to the customer's industry and meeting context. The purpose varies by stage (see Scenario Guidance), but the principle is universal: concrete examples from peers build confidence at every stage. If no exact industry match exists, use the closest adjacent industry and note the gap.*

### Information to Gather

| # | Question | Category | Target Attendee | Purpose |
|---|---|---|---|---|
| 1 | `{question}` | `{MEDDPICC element / Technical / Org / Budget / Timeline / Other}` | `{name/role}` | `{How this serves the meeting objectives}` |
| 2 | `{question}` | | `{name/role}` | `{purpose}` |
| 3 | `{question}` | | `{name/role}` | `{purpose}` |

**Example (Scenario 1 — meeting with CFO):**

| # | Question | Category | Target Attendee | Purpose |
|---|---|---|---|---|
| 1 | "Revenue grew 7.5% last year but profit contracted — where is the margin pressure coming from?" | Identified Pain (I) | CFO | Validate pain point with data; show we've done homework |
| 2 | "How does Weichai typically evaluate and adopt new technology? Who else would be involved?" | Decision Process (DP) | CFO | Map buying process; identify if CFO can move alone or needs CIO/CEO |
| 3 | "What sparked your interest in AI for finance — is there a specific use case you're hoping to solve?" | Champion (Ch) | CFO | Understand motivation: top-down mandate, personal curiosity, or board pressure |

### Information to Deliver

| # | What to Share | Format | Purpose |
|---|---|---|---|
| 1 | `{e.g., Industry insight on cloud adoption trends}` | `{Data point / Slide / Case study}` | `{e.g., Build credibility and establish relevance}` |
| 2 | `{e.g., Similar customer success story}` | `{Case study / Reference call}` | `{e.g., Address specific objection about migration risk}` |
| 3 | `{e.g., Preliminary architecture overview}` | `{Whiteboard / Diagram}` | `{e.g., Validate technical hypothesis from Section 2 objectives}` |

**Example (Scenario 1 — meeting with manufacturing CFO):**

| # | What to Share | Format | Purpose |
|---|---|---|---|
| 1 | AI in Finance: 3 use cases with measurable ROI (intelligent forecasting, automated close, anomaly detection) | Talking points + 2-3 data points | Build credibility — show we understand finance function challenges |
| 2 | Similar manufacturer reduced close cycle from 12 days to 4 days using AWS | Verbal case study | Social proof from a peer — CFOs trust peer results over vendor claims |
| 3 | "Revenue up, profit down" — how AI-powered cost visibility helps identify margin leakage at product/customer/BU level | Data point / whiteboard | Directly relevant to their 2025 results; shows we understand their specific challenge |

---

## 5. Potential Objections & Responses

> *💡 Agent drafts based on CXO Persona profiles (for executive-level attendees), competitive context from EP, and scenario guidance. Sales reviews and adds.*

| # | Anticipated Objection | Our Response |
|---|---|---|
| 1 | `{objection}` | `{response}` |
| 2 | `{objection}` | `{response}` |
| 3 | `{objection}` | `{response}` |

---

## 6. Meeting Agenda

> *💡 Agent drafts agenda to achieve the Target Outcomes and Success Criteria. Sales reviews and adjusts.*
>
> *If the user provided specific start/end times, use actual clock times (e.g., 14:00–14:05). If no specific times were given, use duration instead (e.g., 5 min, 10 min).*

| Time / Duration | Topic | Owner | Purpose |
|---|---|---|---|
| `{00:00–00:05 or 5 min}` | Welcome & introductions | `{name}` | Set the tone |
| `{00:05–00:15 or 10 min}` | `{topic}` | `{name}` | `{purpose}` |
| `{00:15–00:35 or 20 min}` | `{topic}` | `{name}` | `{purpose}` |
| `{00:35–00:50 or 15 min}` | `{topic}` | `{name}` | `{purpose}` |
| `{00:50–00:55 or 5 min}` | Recap & alignment on next steps | `{name}` | Confirm outcomes |
| `{00:55–01:00 or 5 min}` | Close | `{name}` | — |

---

*Managed by AI Agent · Part of the Customer Engagement Closed-Loop Flow*
