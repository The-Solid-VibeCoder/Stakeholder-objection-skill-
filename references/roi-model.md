# ROI Quantification Model for Reward AI Tools

When the user lacks hard ROI data, use this model to build defensible numbers from observable inputs. The goal is not false precision but a credible range that shifts the conversation from "prove it" to "let's test it."

---

## The Four Levers

Every Reward AI business case can be quantified through some combination of these four levers. You do not need all four, but the more you can populate, the stronger the case.

### 1. Time Saved (Hours × Rate)

**What to measure:** Hours currently spent on tasks the AI tool would handle or accelerate.

**How to estimate:**
- Ask the user: "How many hours per week/month does your team spend on [specific task]?"
- Multiply by fully loaded hourly rate (salary + benefits + overhead, typically 1.3-1.5× base salary ÷ annual working hours)
- Apply a conservative automation/acceleration factor (start at 30-50% time reduction for realistic credibility; do not claim 80%+ unless the user has evidence)

**Example calculation:**
```
Task: Manual salary benchmarking for annual review
Team hours per cycle: 320 hours (4 analysts × 2 weeks)
Fully loaded rate: £55/hour
Current cost per cycle: £17,600
Estimated time reduction with AI: 40%
Annual saving: £17,600 × 0.40 × [cycles per year] = £7,040 per cycle
```

**Common Reward tasks to quantify:**
- Salary benchmarking and market pricing
- Pay equity analysis and reporting
- Benefits enrolment and query handling
- Compensation modelling for annual review
- Job evaluation and grading
- Ad-hoc data requests from HRBPs and managers
- Regulatory reporting (gender pay gap, pay transparency)

### 2. Error / Rework Reduction

**What to measure:** Cost of errors in current manual processes.

**How to estimate:**
- Ask: "When was the last time a comp error had to be corrected? How long did it take to fix?"
- Common error types: incorrect benchmarking, wrong pay band assignment, missed eligibility, formula errors in modelling, data entry mistakes
- Cost of an error = time to detect + time to correct + time to communicate + any financial impact (overpay, underpay, clawback)

**Example calculation:**
```
Error rate in manual salary review: 3% of recommendations need rework
Volume: 2,000 employees reviewed
Errors: 60 cases
Average rework time per error: 2 hours (analyst) + 1 hour (manager/HRBP communication)
Cost per error: 3 hours × £55 = £165
Total annual rework cost: 60 × £165 = £9,900
Estimated error reduction with AI: 50%
Annual saving: £4,950
```

### 3. Compliance Risk Reduction (Probability × Impact)

**What to measure:** Reduced exposure to regulatory penalties, litigation, or reputational damage.

**How to estimate:**
- Identify the compliance obligation (e.g., gender pay gap reporting, pay transparency directive, equal pay audit)
- Estimate probability of a compliance gap under current process (qualitative: low/medium/high, or % if available)
- Estimate financial impact of non-compliance (regulatory fine, litigation cost, reputational damage)
- Show how the AI tool reduces the probability (earlier detection, automated audit, continuous monitoring)

**Example calculation:**
```
Risk: Pay equity claim (employment tribunal)
Current probability (without systematic analysis): 10% per year (estimated)
Average cost per claim: £30,000 (legal fees + settlement + management time)
Expected annual cost: 0.10 × £30,000 = £3,000
With AI-powered pay equity monitoring: probability reduced to 3%
Expected annual cost with AI: 0.03 × £30,000 = £900
Risk reduction value: £2,100 per year
```

**Note:** Compliance risk numbers are inherently uncertain. Present them as a range, not a point estimate, and label the assumptions clearly. The point is not to pretend you know the exact risk, but to show you have thought about it.

### 4. Cycle-Time Improvement

**What to measure:** Speed of key Reward processes, and the business value of doing them faster.

**How to estimate:**
- Ask: "How long does [process] take end-to-end today?"
- Identify the bottleneck the AI tool addresses
- Estimate the reduced cycle time
- Quantify the value of faster delivery (earlier implementation of pay changes, faster response to market shifts, reduced time-to-offer)

**Example calculation:**
```
Process: Annual salary review (from data collection to manager communication)
Current cycle time: 12 weeks
Bottleneck: Manual data gathering and modelling (4 weeks)
Estimated reduction with AI: 4 weeks → 1.5 weeks
New cycle time: 9.5 weeks
Business value: Pay changes implemented 2.5 weeks earlier, reducing attrition risk during review period
```

**Cycle-time improvements are often the most compelling argument for HR leadership** because they are visible and felt across the organisation, even if they are harder to assign a precise financial value.

---

## Assembling the Business Case

### Quick-and-Dirty Version (for a meeting or email)

Pick the two strongest levers and present them as a range:

```
Conservative estimate: £[X] per year in time savings alone
Adding error reduction and compliance risk: £[X] - £[Y] per year
Payback period on a £[tool cost] investment: [N] months
```

### Full Version (for a deck or formal business case)

| Lever | Annual Value (Conservative) | Annual Value (Optimistic) | Assumptions |
|-------|---------------------------|--------------------------|-------------|
| Time saved | £X | £Y | [list key assumptions] |
| Error/rework reduction | £X | £Y | [list key assumptions] |
| Compliance risk reduction | £X | £Y | [list key assumptions] |
| Cycle-time improvement | Qualitative | Qualitative | [describe benefit] |
| **Total** | **£X** | **£Y** | |
| Tool cost (annual) | £Z | £Z | |
| **Net value** | **£X-Z** | **£Y-Z** | |
| Payback period | [N months] | [N months] | |

### Three-Tier Presentation (for CFOs and Finance)

CFOs increasingly expect AI business cases to be structured in tiers that separate operational efficiency from strategic impact. Use this structure when presenting to Finance:

| Tier | What it measures | Input variables | How to quantify |
|------|-----------------|-----------------|-----------------|
| **Tier 1: Efficiency gains** | Direct time and cost savings | Hours saved per task, fully loaded rate, adoption rate | Use Lever 1 (Time Saved) above |
| **Tier 2: Quality improvements** | Reduction in costly errors, compliance gaps, rework | Error rate, cost per error, compliance risk exposure | Use Levers 2 and 3 above |
| **Tier 3: Strategic impact** | Revenue protection, talent retention, speed-to-market | Turnover cost, time-to-hire impact, revenue-per-employee | Harder to quantify precisely; link to business outcomes qualitatively and propose measuring during pilot |

Tier 1 is the easiest to defend. Tier 3 is the most compelling but hardest to prove upfront. Lead with Tier 1, add Tier 2 for credibility, and reference Tier 3 as the strategic upside the pilot is designed to validate.

---

## The "Cost of Being Wrong" Framework

CFOs are trained to think about downside risk, not just upside. Use this framework to show you have thought about what happens if the AI tool fails, not just what happens if it succeeds. This directly addresses the scepticism documented in BCG research showing median AI ROI of only 10% against 20% targets.

**The calculation:** Risk exposure = Probability of AI error × Financial/reputational impact of that error

**Apply it to each proposed use case:**

| Use case | If the AI gets it wrong | Cost of being wrong | Risk classification | Recommended approach |
|----------|------------------------|--------------------|--------------------|---------------------|
| Benefits FAQ chatbot | Employee gets incorrect plan information, calls HR to correct | Low (operational annoyance, minor rework) | Low risk | Automate confidently, monitor accuracy |
| Salary benchmarking | Market data misinterpreted, pay bands set incorrectly | Medium (competitive disadvantage, retention risk) | Medium risk | AI recommends, analyst validates, manager approves |
| Pay equity analysis | Statistical model misses a genuine pay gap or flags a false positive | High (regulatory fine, litigation, reputational damage) | High risk | AI assists analysis, specialist reviews methodology, Legal signs off on conclusions |
| Executive compensation modelling | Hallucinated market data, miscalculated equity vesting | Very high (board-level exposure, fiduciary breach) | Very high risk | AI handles data preparation only, all modelling reviewed line-by-line |

**How to use this in the conversation:** "We have categorised our proposed use cases by the cost of being wrong. Our pilot starts exclusively with low and medium-risk use cases. High-risk use cases will only proceed after the pilot has validated the tool's accuracy and our governance framework."

This gives the CFO a risk-adjusted view and shows you are not asking them to bet the farm on day one.

---

## Hidden Costs to Include Proactively

Business cases that only account for software licence fees and projected time savings look naive to experienced Finance and Procurement stakeholders. Pre-empt their objections by including these costs upfront:

| Hidden cost category | What it covers | How to estimate |
|---------------------|---------------|-----------------|
| **Data preparation** | Cleaning, normalising, and cataloguing historical HR data so the AI can process it | Estimate analyst hours × rate. For a first-time data cleanup, budget 40-80 hours depending on data quality. |
| **Systems integration** | Connecting the AI tool to HRIS, payroll, benefits platforms via API | Get a scoping estimate from IT or the vendor. Budget for IT involvement (typically 20-40 hours for a pilot). |
| **Change management** | Training the team, updating processes, communicating to stakeholders | Budget for 2-3 training sessions, process documentation updates, and a manager briefing. |
| **Ongoing monitoring** | Reviewing AI outputs for accuracy and bias, quarterly governance reviews | Budget 4-8 hours per quarter for the first year. |
| **Contingency** | Unexpected rework, scope creep, vendor issues | Add 15-20% contingency to total estimated costs. |

Including these costs does not weaken the case. It strengthens it, because the CFO will add them mentally anyway. If you include them and the ROI still holds, the case is far more credible.

---

## The "General Experimentation Fund" Framing

When the full business case for enterprise rollout is too large or uncertain to approve in one step, propose a ring-fenced experimentation budget. This is particularly effective because it reframes the ask from "commit to this tool" to "buy information about whether this tool works."

**Structure:** £5k-15k for a 90-day proof of concept, with a defined success metric and a go/no-go gate before any further investment.

**Why this works:** It leverages the commitment/consistency principle. Once the CFO has publicly approved a small pilot and the pilot succeeds, they are psychologically primed to approve the larger investment, because rejecting it would contradict their earlier endorsement.

---

### Tips for Credibility

1. **Use ranges, not point estimates.** A single number invites challenge. A range shows you have thought about uncertainty.
2. **Label every assumption.** If Procurement can see the assumptions, they can argue with the inputs, not dismiss the model.
3. **Start conservative.** It is better to over-deliver on a conservative estimate than under-deliver on an aggressive one.
4. **Compare to the cost of doing nothing.** The baseline is not zero. Manual processes have costs, risks, and opportunity costs. Frame this explicitly: "If we do nothing, we continue spending £X on manual processes, we remain exposed to £Y in compliance risk, and our team continues to use unsanctioned consumer AI tools without governance."
5. **Include the pilot cost separately.** A £5k-15k pilot is a much easier ask than a £100k enterprise contract. Frame the pilot as buying information, not committing to the tool.
6. **Pre-empt the "AI hype" objection.** CFOs are aware that many departments relabel standard software as "AI" to bypass scrutiny. Be specific about what the tool actually does and how it differs from existing capabilities. Vague claims about "AI-powered insights" will be dismissed.
