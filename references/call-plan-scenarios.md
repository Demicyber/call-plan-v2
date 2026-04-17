# Call Plan — Scenario Guidance

> **Purpose:** This document guides the AI agent on how to tailor the Call Plan Foundation Template for different meeting scenarios. All Call Plans use the **same 6-section template** — the agent adjusts focus, depth, and content based on the scenario identified.
>
> **How it works:** Sales rep describes the meeting → Agent identifies the scenario → Agent generates the Call Plan using the foundation template, applying the guidance below to shape each section appropriately.

---

## Scenario Identification

When a sales rep requests a Call Plan, the agent determines the scenario using the **Stage → Scenario Mapping** defined in SKILL.md Section 6.

**Primary method:** Map from the current AWS Sales Stage to the default scenario, then check for override conditions (meeting purpose, special circumstances).

**If stage is unknown:** Ask the user directly: "What's the current sales stage for this opportunity?" Then apply the mapping.

**Always confirm** the selected scenario with the user before generating.

```
EBC visit or internal leadership briefing? → Scenario 6: EB ONLY (no Call Plan)
Special circumstance? → Scenario 7: Special Scenarios

Sales stage known?
  ├─ YES → Use Stage → Scenario Mapping (SKILL.md Section 6) → confirm with user
  └─ NO → Ask user for sales stage → then use mapping → confirm with user
```

---

## Scenario 1: New Customer Development

**Stage:** Prospect
**Context:** First interaction — cold outreach, introductory meeting, or warm referral. Little to no prior relationship.

### Agent Guidance

> **Stage Exit Criteria (Prospect → Qualified):** Customer willing to pursue solution; champion & decision-maker identified; delivery partner strategy identified.
>
> **Core principle:** This is a first meeting. The goal is to earn a second meeting, not to close anything. Listen more than you talk.

| Section | Focus |
|---|---|
| **Meeting Details** | Expect sparse info. Pull account context from EP (account analysis). If attendee titles are unknown, ask sales to confirm before generating — persona matching depends on it. |
| **Target Outcomes** | **User's objective comes first.** Then suggest outcomes aligned to stage exit criteria: (1) *Customer perspective:* Understand how AWS is relevant to their business; see industry-specific proof points. (2) *Our perspective:* Validate whether a real pain point exists (I); identify potential champion (Ch) and economic buyer (E); understand org structure and decision process (DP); assess if opportunity is worth pursuing. **Do not push for commitment — the target is a second meeting.** |
| **Success Criteria** | Must be observable: e.g., "Customer agrees to a follow-up meeting with technical team" or "Customer shares their current vendor landscape and budget cycle." Not: "Customer is interested." |
| **Information Exchange** | **Gather:** Org structure, strategic priorities, existing tech stack, cloud posture, decision-making process. **MEDDPICC focus: Identified Pain (I), Economic Buyer (E), Metrics (M), Decision Process (DP), Champion (Ch).** Questions should be conversational, not interrogative — weave into natural dialogue. **Deliver (aligned to Prospect stage activities):** (1) Industry credibility — AWS positioning in their specific industry, market share, relevant certifications; (2) Peer references — 1-2 customer stories from similar companies/industries with quantified outcomes; (3) Initial value hypothesis — a specific, testable proposition about how AWS could address their situation (not a generic pitch); (4) Industry/market insights — trends, benchmarks, or data points that demonstrate you understand their world. **Purpose of delivery at this stage: build credibility and earn the right to a deeper conversation, not sell.** |
| **Objections** | Expect "why should we talk to AWS?" and "we already have a vendor." Prepare credibility anchors: industry-relevant proof points, peer company references, specific value propositions. If executive attendee, load CXO Persona objection handling. |
| **Agenda** | Conversational. **70/30 rule: customer talks 70%, you talk 30%.** Structure: rapport/ice-breaker (use recent company news or industry trend) → transition to discovery → share 1-2 relevant insights → propose next step. Keep it natural, not a presentation. |

### Additional Prep for Agent
- Pull latest account analysis from EP (ensure data is current)
- If executive attendee: load CXO Persona profile, apply to objections, questions, and language
- Prepare ice-breaker strategy (recent company news, mutual connections, industry trends)
- Build an initial value hypothesis to validate during the meeting
- Prepare a concrete next-step proposal (e.g., "technical deep-dive with your CTO" or "value assessment workshop")

---

## Scenario 2: Discovery

**Stage:** Qualified
**Context:** Customer is engaged. Need deep understanding of requirements across multiple levels or departments.

### Agent Guidance

> **Stage Exit Criteria (Qualified → Technical Validation):** Shared understanding of customer requirements; technical solution direction agreed; POC or technical validation plan in place.
>
> **Core principle:** This is the deep-dive. Your success is measured by how much information you gather, not how much you present. Fill MEDDPICC gaps aggressively.

| Section | Focus |
|---|---|
| **Meeting Details** | Map all attendees to their decision roles. **If key roles (EB, Champion) are missing from the invite, don't just flag it — suggest sales invite them.** "I notice there's no economic buyer in this meeting. Would it make sense to invite [title] to ensure we can validate budget direction?" |
| **Target Outcomes** | **User's objective comes first.** Then suggest outcomes aligned to stage exit criteria: (1) *Customer perspective:* Confirm AWS understands their requirements and can propose a viable approach. (2) *Our perspective:* Complete MEDDPICC qualification — validate pain (I), confirm metrics (M), identify champion (Ch), map decision process (DP), identify economic buyer (E), understand competitive landscape (CP). Aim to exit this meeting with enough information to propose a technical validation plan. |
| **Success Criteria** | All critical MEDDPICC elements confirmed or significantly advanced. Clear picture of decision process and timeline. E.g., "Customer confirms their top 3 technical requirements" or "Customer shares their evaluation timeline and competing vendors." |
| **Information Exchange** | This is the **primary section — expand significantly.** MEDDPICC focus: I, M, Ch, DP, E, CP. Gather across departments if multi-stakeholder. **Questions should probe depth, not breadth** — follow up on answers, don't just check boxes. **Deliver (aligned to Qualified stage activities):** (1) Preliminary solution direction — how AWS could address their validated pain points; (2) Tailored value proposition — pain → value → solution mapping specific to their situation; (3) Relevant architecture patterns — high-level approaches that match their requirements; (4) Proof points — case studies or data that address their specific pain, not generic AWS marketing. **Purpose of delivery at this stage: demonstrate you've listened and can propose a credible path forward.** |
| **Objections** | Expect scope/timing objections: "we're not ready," "we're still evaluating," "this is too big." Prepare phased approaches and quick-win options to reduce perceived risk. |
| **Agenda** | Structure around **discovery themes, not presentations.** Allocate majority of time to questions and listening. If multiple stakeholders, plan who asks what to whom. |

### Additional Prep for Agent
- Pull latest account analysis from EP
- Prepare MEDDPICC deep-dive framework: current understanding per element + specific gaps to close
- Map department-by-department discovery needs if multi-BU engagement
- Prepare budget / timeline / decision process question sets
- If executive attendee: load CXO Persona profile

---

## Scenario 3: Solution Advancement

**Stage:** Technical Validation
**Context:** Proving technical fit — demos, architecture workshops, POC planning, technical deep-dives.

### Agent Guidance

> **Stage Exit Criteria (Technical Validation → Business Validation):** Technical solution finalized and agreed; shared understanding of architecture/implementation; customer confirms technical fit.
>
> **Core principle:** Prove it works. Technical credibility is everything in this meeting. Come prepared with specifics, not generalities.

| Section | Focus |
|---|---|
| **Meeting Details** | Technical attendees expected (architects, engineers, technical decision-makers). **If no technical decision-maker is present, flag and suggest inviting one** — technical validation without a technical decision-maker is wasted effort. |
| **Target Outcomes** | **User's objective comes first.** Then suggest outcomes aligned to stage exit criteria: (1) *Customer perspective:* Confirm the proposed solution meets their technical requirements; understand implementation approach and timeline. (2) *Our perspective:* Get agreement on architecture direction or POC scope (DC); confirm technical success metrics (M); secure technical champion alignment (Ch); understand integration constraints and compliance needs. **POC success criteria must be co-defined with the customer** — not AWS-defined unilaterally. |
| **Success Criteria** | Customer confirms technical fit or agrees to POC/pilot. Technical objections addressed. E.g., "Customer and AWS jointly agree on POC scope, success metrics, and 8-week timeline" or "Customer confirms proposed architecture meets their scalability requirements." |
| **Information Exchange** | **MEDDPICC focus: Decision Criteria (DC), Decision Process (DP), Metrics (M), Champion (Ch — technical champion alignment).** Also gather: technical requirements, integration constraints, compliance needs, scale expectations, **potential technical blockers** (what could prevent this from working?). **Deliver (aligned to Technical Validation stage activities):** (1) Architecture proposal — detailed design with specific AWS services, integration points, and data flows; (2) Benchmark data — performance, scalability, and reliability evidence relevant to their workload; (3) Demo or hands-on experience — let them see/touch the technology; (4) POC plan — jointly-defined scope, success metrics, timeline, and exit criteria; (5) Technical blocker mitigation — for each identified risk, a specific mitigation approach. **Purpose of delivery at this stage: prove technical fit with evidence, not promises.** |
| **Objections** | Technical objections and competitive FUD. Prepare **specific technical proof points** — benchmarks, reference architectures, customer testimonials from similar technical environments. Don't hand-wave; show evidence. |
| **Agenda** | Include demo flow or workshop structure. **Balance presentation with hands-on / interactive elements.** Technical audiences engage more when they can touch the technology, not just watch slides. |

### Additional Prep for Agent
- Pull latest account analysis from EP
- Document proposed architecture and AWS services involved
- Prepare POC scope, success metrics, and exit criteria — **framed as a joint exercise with the customer, not a pre-baked plan**
- Build competitive differentiation points with technical proof
- **Identify potential technical blockers** (integration complexity, data residency, compliance, legacy system constraints) and prepare mitigation approaches
- If executive attendee: load CXO Persona profile

---

## Scenario 4: Commercial Negotiation

**Stage:** Business Validation
**Context:** Pricing, contracts, terms, procurement discussions. Finance and procurement attendees likely.

### Agent Guidance

> **Stage Exit Criteria (Business Validation → Committed):** Customer approvals secured; deal details/economics/close plan agreed; commercial terms aligned.
>
> **Core principle:** This is about the business case, not the technology. Speak in financial language. Every claim must be quantified.

| Section | Focus |
|---|---|
| **Meeting Details** | Expect procurement / finance / legal attendees. **If Economic Buyer is not in the room, flag and suggest inviting them** — commercial negotiation without the budget holder is a rehearsal, not a negotiation. |
| **Target Outcomes** | **User's objective comes first.** Then suggest outcomes aligned to stage exit criteria: (1) *Customer perspective:* Validate the financial case; understand total cost of ownership; confirm commercial terms are acceptable. (2) *Our perspective:* Get agreement on pricing or receive a counter-proposal (E); confirm procurement steps and timeline (PP); validate financial metrics and ROI assumptions (M); secure economic buyer alignment (E). |
| **Success Criteria** | Clear path to contract execution. E.g., "Customer confirms pricing model is within budget range and shares procurement timeline" or "Customer provides counter-proposal with specific terms to negotiate." |
| **Information Exchange** | **MEDDPICC focus: Economic Buyer (E), Paper Process (PP), Decision Process (DP), Metrics (M — financial).** Gather: budget authority, **full procurement process** (approval chain, legal review, security review, contract execution steps), legal requirements, approval timeline. **Deliver (aligned to Business Validation stage activities):** (1) Business case / ROI analysis — with specific numbers, assumptions, and time horizons; (2) TCO comparison — total cost of ownership vs. current state or competitors; (3) Pricing proposal — clear pricing model with options; (4) Commercial terms — contract structure, commitment options, flexibility; (5) Procurement process alignment — show you understand their process and have a plan to navigate it. **All delivery must be quantified — no vague value claims. Purpose of delivery at this stage: make the financial case irrefutable and remove procurement friction.** |
| **Objections** | Pricing and contract objections. Prepare **value-based responses, not discount offers.** Frame every response in terms of business outcomes and financial impact. If CFO persona is involved, use financial language (payback period, TCO, ROIC). |
| **Agenda** | Structured around commercial topics. Leave time for negotiation and Q&A. Don't rush — commercial conversations need space for back-and-forth. |

### Additional Prep for Agent
- Pull latest account analysis from EP
- Prepare pricing strategy — **agent reminds sales to internally confirm discount authority and walk-away point before the meeting, but these do NOT go into the Call Plan document** (sensitive internal information)
- Build ROI / TCO analysis summary with specific numbers and assumptions
- **Map the full procurement process:** budget approval → legal review → security review → contract execution. Identify which steps are done and which remain.
- If executive attendee: load CXO Persona profile (especially CFO, Head of Procurement)

---

## Scenario 5: Post-Signing

**Stage:** Committed / Closed/Launched
**Context:** Kick-offs, implementation reviews, QBRs, customer success check-ins, renewal/expansion discussions.

### Agent Guidance

> **Stage Exit Criteria (Committed → Closed/Launched):** Agreement signed; migration started or usage targets met. For expansion: new opportunity identified and qualified.
>
> **Core principle:** Shift from "win the deal" to "ensure success and grow the account." **If the customer has unresolved concerns, address those first before discussing expansion.** Trust is the foundation for growth.

| Section | Focus |
|---|---|
| **Meeting Details** | May include implementation teams, customer success, or new stakeholders for expansion. Map new attendees to roles — expansion conversations may involve different decision-makers than the original deal. |
| **Target Outcomes** | **User's objective comes first.** Then suggest outcomes aligned to stage context: (1) *Customer perspective:* Confirm implementation is on track and delivering expected value; understand what's next from AWS. (2) *Our perspective:* Validate adoption metrics and customer satisfaction (M); identify expansion opportunities across specific dimensions — **new workloads, new business units, new regions, upsell existing services, cross-sell new services** (DC); understand budget for next phase (E); confirm renewal trajectory (PP). |
| **Success Criteria** | Customer confirms satisfaction and implementation progress. E.g., "Customer shares adoption metrics and confirms 3 workloads on track for migration" or "Customer identifies 2 new business units interested in AWS." |
| **Information Exchange** | **MEDDPICC focus: Metrics (M), Decision Criteria (DC), Paper Process (PP), Economic Buyer (E).** Gather: adoption blockers, satisfaction signals, migration progress, new initiatives, budget for expansion, **unresolved concerns or complaints.** **Deliver (aligned to Committed/Closed stage activities):** (1) Usage insights — actual adoption data, consumption trends, cost optimization opportunities; (2) Business outcome report — how the implementation is tracking against the promised metrics; (3) New capabilities — relevant AWS launches, features, or services since last engagement; (4) Roadmap alignment — how AWS product roadmap maps to their future needs; (5) Optimization recommendations — specific actions to improve performance, reduce cost, or increase adoption. **If concerns exist, address them before pivoting to expansion. Purpose of delivery at this stage: demonstrate ongoing value and build the case for growth.** |
| **Objections** | Reframe as "concerns" — support issues, unmet expectations, implementation delays. **Listen first, acknowledge, then address.** Don't be defensive. Show you're invested in their success, not just the next sale. |
| **Agenda** | Review-oriented. Cover: implementation status → usage metrics → satisfaction check → address concerns → next phase planning. **The order matters: don't jump to expansion before confirming the current phase is healthy.** |

### Additional Prep for Agent
- Pull latest account analysis from EP
- Pull implementation milestone tracker and usage/adoption metrics
- Prepare customer success scorecard
- **Identify expansion opportunities across 5 dimensions:** new workloads, new BUs, new regions, upsell existing services, cross-sell new services
- Check for any open support tickets, escalations, or unresolved issues — address these first
- If executive attendee: load CXO Persona profile

---

## Scenario 6: Executive Briefing (EBC or Internal Leadership)

**Stage:** Cross-stage

> ⚠️ **Executive Briefing scenarios do NOT use the Call Plan template.** Use the **Executive Briefing Document** instead.
>
> This applies to two situations:
> 1. **EBC visits** — External executive briefing center engagements
> 2. **Internal leadership briefing** — AWS senior leadership joining a customer visit and needing a briefing
>
> In both cases, the Executive Briefing Document is the sole preparation document. The agent should generate an Executive Briefing Document when either situation is identified.

---

## Scenario 7: Special Scenarios

**Stage:** Cross-stage
**Context:** Non-standard situations requiring specialized preparation.

### 7a: Crisis / Escalation Meeting

**Agent should additionally prepare:**
- Crisis summary (what happened, impact, resolution status, root cause)
- Relationship recovery plan (immediate → short-term → long-term actions)
- "Topics to handle carefully" guidance for AWS attendees

### 7b: Joint Partner Visit

**Agent should additionally prepare:**
- Partner coordination (who leads which topics, messaging alignment)
- Joint value proposition (why AWS + partner together > separate)
- Pre-meeting sync plan between AWS and partner teams

### 7c: Event Follow-up

**Agent should additionally prepare:**
- Event context (what was discussed, interests expressed, commitments made)
- Connection to broader engagement strategy
- Time-sensitive follow-up items from the event

### 7d: Competitive Displacement

**Agent should additionally prepare:**
- Current vendor analysis (products in use, **contract status and expiration date**, customer satisfaction)
- **Contract timing assessment:** How long until the current vendor contract expires? This determines the displacement window and urgency. Strategy differs significantly for "expires in 6 months" vs. "3 years remaining."
- Switching cost/benefit analysis (financial, technical, operational, strategic)
- Phased migration path with risk mitigation

---

*Version: 2.1 | Last updated: 2026-04-17 | Part of the Customer Engagement Closed-Loop Flow*
