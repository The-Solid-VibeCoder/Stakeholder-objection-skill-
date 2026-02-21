# Influence Playbook: Sequencing Stakeholder Conversations

This reference covers the tactical side of stakeholder management: not what to say (that is in the objection bank), but how to sequence conversations, build momentum, and use behavioural principles to shift entrenched positions.

---

## The Sequencing Problem

Most Reward professionals make the same mistake: they build a business case in isolation, then present it to all stakeholders simultaneously and hope for the best. This fails because each stakeholder has different concerns, different decision criteria, and different levels of influence over the outcome. A rejection from one can poison the others.

The better approach is sequential momentum-building: win small agreements from easier stakeholders first, then use those agreements as leverage with harder ones.

---

## Recommended Sequence

The exact order depends on your organisation, but this sequence works in most cases:

### 1. Executive Sponsor (outside HR)

**Why first:** You need someone with budget authority and cross-functional credibility to champion the case alongside you. Without a sponsor, Reward is asking for something on its own, which reinforces the "back office" perception.

**Who to approach:** Look for a senior leader (Operations, Finance, Commercial) who is experiencing a pain the AI tool addresses, such as a COO struggling with labour shortages caused by slow recruitment, a CFO spending heavily on external consultants for pay benchmarking, or a business unit leader frustrated by how long the annual salary review takes.

**What to ask for:** Not budget approval yet. Just agreement that the problem is real and worth investigating. "If I could show you a way to cut the salary review cycle by 3 weeks, would that be worth exploring?" A "yes" here is all you need.

### 2. HR Leadership / CHRO

**Why second:** You need your own leadership aligned before approaching other functions. Presenting externally without internal alignment is politically dangerous.

**What to show them:** The sponsor's interest, the connection to an existing strategic priority, and a clear proposal that does not require additional headcount or major change management.

### 3. IT / Security

**Why third:** IT buy-in (or at least non-opposition) is essential before Legal and Procurement, because both will ask "has IT reviewed this?" If you can answer yes, you clear their most common deferral tactic.

**What to offer them:** Reciprocity. Before asking for anything, offer something valuable. For example, share the vendor's SOC 2 report and DPA in advance, or offer to co-own the security assessment. If you can demonstrate the tool solves a problem IT also cares about (e.g., replacing unsanctioned Shadow AI with a governed platform), even better.

### 4. Legal / Privacy

**Why fourth:** Legal will want to see that IT has reviewed the security posture and that you have a governance framework. Coming to Legal without these is asking them to do your homework.

**What to bring:** A draft DPIA, a proposed human-in-the-loop protocol, and the governance checklist (see `references/governance-checklist.md`). Ask for their review, not their permission. "We have drafted this. We would like your input before we finalise." This positions Legal as a collaborator, not a gatekeeper.

### 5. Procurement / Finance

**Why last:** By this point, you have: an executive sponsor, HR leadership alignment, IT's security assessment, and Legal's compliance framework. Procurement's remaining concern is cost and value. Present the full business case with all objections already addressed.

---

## Behavioural Principles for Each Conversation

These are adapted from Cialdini's influence research, applied to the specific context of internal HR stakeholder management.

### Reciprocity: Give Before You Ask

People are wired to return favours. Before requesting anything from a stakeholder, offer them something valuable that costs you relatively little.

**In practice:**
- Build IT a quick data dashboard or automated report that solves one of their problems, using the tool you are proposing
- Give Legal a first draft of the AI policy they have been meaning to write but have not had time for
- Give Procurement a clean vendor comparison that saves them evaluation work

The value does not need to be large. The principle works because the act of giving creates a psychological obligation that makes the recipient more amenable to your subsequent request.

### Authority: Speak Their Language

Stakeholders defer to people they perceive as credible experts. When HR talks to IT about "efficiency gains," IT hears HR jargon. When HR talks about "data flow architecture, encryption at rest, and RBAC," IT hears a peer.

**In practice:**
- Learn enough of each stakeholder's technical vocabulary to demonstrate competence (you do not need to be an expert, just credible)
- Lead with radical transparency about risks before stakeholders point them out. Paradoxically, admitting limitations enhances perceived authority
- "Borrow" authority by bringing in external validation: an independent analyst, a legal opinion, a case study from a peer organisation

### Social Proof: Show Who Else Has Done This

When people face uncertainty, they look at what others are doing. This is especially powerful with senior executives who fear being left behind.

**In practice:**
- Research 2-3 direct competitors or peer organisations who have deployed similar AI tools in their Reward function. Be specific about outcomes, not vague about "industry trends."
- If you cannot find direct competitors, use adjacent examples (e.g., Finance teams deploying the same tool for financial analysis)
- Frame it as: "Three of our direct competitors have already done this. The question is not whether, but when."

### Commitment and Consistency: Start Small

People want to be consistent with their previous commitments. If someone publicly agrees to a small step, they are psychologically primed to agree to the larger step that follows.

**In practice:**
- Do not ask the CFO for enterprise budget on day one. Ask for a 90-day pilot budget (£5k-15k)
- Do not ask Legal for full sign-off. Ask them to review your draft DPIA
- Do not ask IT for full integration. Ask for a sandboxed environment with non-production data
- Once each stakeholder has said "yes" to the small ask and the pilot succeeds, the larger ask becomes an extension of their existing commitment, not a new decision

### Unity: Make Them Co-Architects

People support what they help create. Invite the most vocal critics into the process before vendor selection, not after.

**In practice:**
- Form a lightweight cross-functional evaluation group (Legal, IT, Procurement, HR) before writing the RFP
- Give each stakeholder a specific role: IT owns the security assessment, Legal owns the DPIA, Procurement owns the commercial evaluation
- When the recommendation comes from the group, not from HR alone, it carries fundamentally different weight

---

## Vendor Negotiation Tactics

When negotiating externally with AI vendors, keep these principles in mind:

**Evaluate Total Cost of Ownership, not licence fees.** AI vendors often structure pricing to capture value through implementation fees, API usage limits, token pricing tiers, and premium support. Model how costs scale as adoption grows over 3-5 years.

**Anchor high.** Enter discussions requesting premium features, unlimited API access, dedicated implementation support, and customised encryption. Vendors expect negotiation. Starting high gives you room to concede on non-essentials while holding firm on pricing and security guarantees.

**Use timing.** Aligning negotiations with the vendor's fiscal quarter or year end increases your leverage significantly, because sales teams face pressure to close deals.

**Be transparent about competition.** Telling a vendor you are actively evaluating a specific competitor forces them to abandon standard pricing and offer their best terms. You do not need to bluff; genuinely evaluate at least two vendors and let each know.

---

## Common Mistakes to Avoid

1. **Presenting to all stakeholders simultaneously.** This ensures the most risk-averse stakeholder sets the pace for everyone.
2. **Asking for permission instead of input.** "May we do this?" invites "no." "We have drafted this; could you review it?" invites collaboration.
3. **Arguing instead of trading.** When a stakeholder objects, the instinct is to counter-argue. The better move is to offer a concession that addresses their underlying interest while preserving your core objective.
4. **Ignoring Shadow AI.** If your colleagues are already using consumer AI tools, that fact is your single most powerful argument. It shifts the conversation from "should we adopt AI?" to "should we govern the AI we are already using?"
5. **Waiting for perfect data.** The pilot exists to generate data. You do not need perfect ROI projections to justify a small, time-boxed experiment.
