# AI Governance Readiness Checklist for Reward Teams

Use this checklist to demonstrate governance readiness to Legal, IT, and HR leadership. Completing (or having a plan to complete) these items before the approval conversation turns a potential blocker into evidence of seriousness.

---

## 1. Data Protection Impact Assessment (DPIA)

**Status:** [ ] Not started / [ ] In progress / [ ] Complete

A DPIA is likely required if the AI tool processes employee personal data in a way that could create risk, particularly if it involves profiling, automated decision-making, or large-scale processing of special category data.

**EU AI Act classification:** Under the EU AI Act, AI systems used in employment, worker management, and access to self-employment are explicitly classified as "high-risk" if they can affect a person's employment status, health, or safety. This triggers mandatory requirements for transparency, human oversight, data governance, and accuracy standards. Fines for non-compliance can reach 7% of annual global turnover. Even if you are not in the EU, this classification is increasingly used as a reference point by Legal teams globally. Factor it into your DPIA and governance framework proactively.

**Key questions the DPIA must answer:**
- What personal data is processed? (Name, pay, performance ratings, benefits elections, demographic data)
- What is the legal basis? (Legitimate interest, performance of contract, consent, legal obligation)
- Is data minimisation applied? (Only data strictly necessary for the use case)
- What are the risks to data subjects? (Discrimination, unfair treatment, privacy breach, inaccuracy)
- What mitigations are in place? (Human review, access controls, encryption, audit trail, appeal mechanism)
- Is there cross-border data transfer? If so, what transfer mechanism applies? (SCCs, adequacy decision, BCRs)

**Tip:** Offer to draft the DPIA and have Legal/DPO review, rather than waiting for them to initiate it. This shows ownership and accelerates the timeline.

---

## 2. AI Usage Policy / Responsible AI Guidelines

**Status:** [ ] Not started / [ ] In progress / [ ] Complete

If your organisation does not yet have an AI usage policy, this is an opportunity to help create one. A controlled pilot is actually the best way to develop a fit-for-purpose policy, because you can test it in practice.

**Minimum policy elements:**
- **Scope:** Which tools and use cases are covered
- **Permitted use cases:** What the tool may be used for (e.g., analysis, benchmarking, reporting)
- **Prohibited use cases:** What the tool must not be used for (e.g., autonomous hiring/firing decisions, processing data outside scope)
- **Human oversight requirement:** For any output that informs an employment decision, a named human must review, can override, and must document their rationale
- **Data handling rules:** What data may be input, how outputs are stored, who has access
- **Transparency:** How employees are informed that AI tools are used in Reward processes
- **Accountability:** Who is responsible for monitoring tool performance, reviewing outputs, and escalating issues
- **Review cadence:** How often the policy and tool performance are reviewed (suggest quarterly for the first year)

---

## 3. Vendor Due Diligence

**Status:** [ ] Not started / [ ] In progress / [ ] Complete

**Security assessment:**
- [ ] SOC 2 Type II report reviewed (or equivalent, e.g., ISO 27001)
- [ ] Data processing agreement (DPA) reviewed and signed
- [ ] Penetration test summary reviewed (ask for the executive summary, not the full report)
- [ ] Data residency confirmed (where is data stored and processed?)
- [ ] Encryption standards confirmed (TLS 1.2+ in transit, AES-256 at rest)
- [ ] Model training opt-out confirmed (vendor does not use your data to train models)
- [ ] Access controls documented (RBAC, SSO/SAML integration, audit logging)

**Contractual review:**
- [ ] Liability and indemnification clauses reviewed
- [ ] Data portability clause included (ability to export data in standard formats)
- [ ] Termination and data deletion clause included
- [ ] SLA terms reviewed (uptime, incident response, notification timelines)
- [ ] Sub-processor list reviewed (who else touches the data?)

**Tip:** Many vendors have a pre-built security pack (SOC 2 report, DPA template, security whitepaper, pen test summary). Ask for it upfront. If they do not have one, that is itself a data point.

---

## 4. Human-in-the-Loop Protocol

**Status:** [ ] Not started / [ ] In progress / [ ] Complete

This is the most important governance element for Reward AI use cases because it directly addresses the risk of automated decision-making claims.

**Protocol design:**
- [ ] AI outputs are presented as recommendations, not decisions
- [ ] A named human reviews every output before it informs an employment action
- [ ] The human can override the AI recommendation and must document their rationale
- [ ] The rationale (AI recommendation + human decision + reasoning) is logged and retained
- [ ] Retention period is aligned to employment litigation limitation period (typically 3-6 years depending on jurisdiction)
- [ ] Employees have a right to request human review of any AI-influenced decision

**For each use case, document:**

| Use case | AI output | Human reviewer | Override authority | Rationale logged? | Retention period |
|----------|----------|---------------|-------------------|-------------------|-----------------|
| Pay equity analysis | Flagged outliers, suggested adjustments | Comp Manager | Yes, full override | Yes | [X] years |
| Salary benchmarking | Market positioning, recommended ranges | Comp Analyst + Manager | Yes, full override | Yes | [X] years |
| Benefits recommendation | Personalised plan suggestions | Benefits Advisor | Yes, full override | Yes | [X] years |

---

## 5. Employee Transparency and Communication

**Status:** [ ] Not started / [ ] In progress / [ ] Complete

- [ ] Privacy notice updated to include AI-assisted processing (if applicable)
- [ ] Employee FAQ prepared explaining what the tool does, what data it uses, and how decisions are made
- [ ] Works Council / union consultation triggered if required (check local labour law)
- [ ] Manager briefing prepared explaining how AI outputs should be used and what "human review" means in practice
- [ ] Feedback mechanism in place for employees to raise concerns about AI-influenced decisions

---

## 6. Ongoing Monitoring and Review

**Status:** [ ] Not started / [ ] In progress / [ ] Complete

- [ ] Quarterly review of AI tool outputs for accuracy and bias (compare AI recommendations to actual outcomes)
- [ ] Annual DPIA review (or sooner if scope changes)
- [ ] Regular audit of access logs (who is using the tool and accessing what data)
- [ ] Vendor performance review against SLA
- [ ] Policy review and update based on emerging regulation (e.g., EU AI Act, local employment law changes)
- [ ] Incident response plan for AI-specific issues (e.g., biased output detected, data leak, tool malfunction)
- [ ] **Billboard Test applied:** For each use case, ask: "Would we be comfortable if the exact methodology behind this AI's recommendations were published publicly?" If the answer is no, the approach needs more transparency, explainability, or human oversight before deployment.

---

## 7. Shadow AI Governance

**Status:** [ ] Not started / [ ] In progress / [ ] Complete

If employees are already using consumer AI tools for HR work (and research suggests they almost certainly are), this needs to be addressed as part of the governance framework, not ignored.

- [ ] Assessed extent of informal/consumer AI usage within the HR and Reward team
- [ ] Documented the data risk: what types of sensitive data could be (or have been) entered into consumer AI tools
- [ ] Included Shadow AI risk mitigation as an explicit benefit of the enterprise AI business case
- [ ] AI usage policy explicitly prohibits use of unsanctioned consumer AI tools for processing employee data
- [ ] Enterprise AI tool positioned as the approved, governed alternative that replaces consumer AI usage
- [ ] Communication plan prepared explaining why the enterprise tool exists and why consumer alternatives are no longer permitted

---

## Using This Checklist in Stakeholder Conversations

**With Legal:** "We have completed / are completing a DPIA, and here is our proposed human-in-the-loop protocol. We would like your review before we proceed."

**With IT:** "We have reviewed the vendor's SOC 2 report and DPA. Here is the data flow. We would like to schedule the standard vendor security assessment."

**With HR Leadership:** "We have a governance plan covering data protection, human oversight, and employee communication. The pilot is designed to test the tool and the governance framework together."

**With Procurement:** "We have addressed the security and governance requirements. Here is the business case, and here is the pilot scope with a go/no-go gate."

The checklist turns "we want to buy a tool" into "we have a governed, risk-aware plan to test a tool." That is a fundamentally different conversation.
