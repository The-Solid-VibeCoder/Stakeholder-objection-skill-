# Stakeholder Objection Skill

A [Claude skill](https://docs.anthropic.com/en/docs/agents-and-tools/claude-code/skills) that coaches **Reward, Compensation and Benefits leaders** through stakeholder objections when seeking approval for AI tools.

## The problem

Reward teams manage some of the most sensitive data in the organisation (pay, performance, benefits), yet they are often perceived as "back office" rather than strategic. When Reward asks for investment in AI tooling, the default challenge from stakeholders is not "is this interesting?" but "show me business impact, and show me you will not create a liability."

Most business cases fail not because the tool is wrong, but because the person proposing it has not prepared for the specific objections that Procurement, IT Security, Legal, and Finance will raise.

## What this skill does

When you describe your situation, the skill runs a structured preparation workflow:

1. **Clarifies your landscape** with targeted questions about your data surface, stakeholder map, risk profile, and Shadow AI exposure.
2. **Rewrites your argument** in three versions, each framed for a different stakeholder's priorities (Procurement/Finance, IT/Security, Legal/Privacy).
3. **Builds an objection-response table** tailored to your situation, drawing from a bank of 21 pre-built objections across four stakeholder groups.
4. **Runs a red-flag scan** on your draft, catching language that sounds fine internally but will get challenged by Legal or Procurement.
5. **Produces ready-to-use outputs**: a 2-minute talk track and a 1-page email, both ready to copy-paste.

It also loads specialist references on demand for ROI quantification, governance readiness, and stakeholder sequencing.

## Reference files

| File | What it covers |
|------|---------------|
| `references/objection-bank.md` | 21 pre-built objections across Procurement/Finance (6), IT/Security (6), Legal/Privacy/ER (7), and HR Leadership (2). Each has five columns: objection, what they're really protecting, best response, proof to bring, and concession to offer. |
| `references/roi-model.md` | Four-lever quantification model (time saved, error reduction, compliance risk, cycle-time improvement), three-tier CFO presentation format, "Cost of Being Wrong" framework, hidden costs checklist, and the "General Experimentation Fund" framing for pilot budgets. |
| `references/governance-checklist.md` | Seven-section checklist covering DPIA (with EU AI Act high-risk classification), AI usage policy, vendor due diligence (SOC 2, DPA, pen testing), human-in-the-loop protocol design, employee transparency, ongoing monitoring (with Billboard Test), and Shadow AI governance. |
| `references/influence-playbook.md` | Recommended stakeholder sequencing (Sponsor → HR Leadership → IT → Legal → Procurement), Cialdini's influence principles applied to each conversation (reciprocity, authority, social proof, commitment/consistency, unity), vendor negotiation tactics, and five common mistakes to avoid. |

## Coaching rules

The skill enforces nine principles across every output:

1. Treat it like a negotiation. Separate positions from interests. Propose trades, not arguments.
2. No black-box decisioning for employment outcomes. Default to decision-support with human review.
3. Always propose governance actions with every objection response.
4. When hard ROI is missing, build it using the four-lever model.
5. Keep outputs structured and deck-ready.
6. Acknowledge the credibility gap. Lead with business language, not HR jargon.
7. Find a friend before you need one. Identify an executive sponsor outside HR.
8. Invite the critics in early. Form a cross-functional evaluation group before vendor selection.
9. Use influence sequencing. Load the playbook for tactical stakeholder management.

## Example prompts

- "I need to get approval for a pay equity AI tool. My biggest blocker is Legal, who are worried about automated decision-making claims."
- "Procurement just said 'we already have too many vendors.' How do I respond?"
- "Help me build an ROI model for a benefits chatbot. I don't have hard numbers yet."
- "I'm meeting with the CISO next week to discuss data security for an AI comp tool. What should I prepare?"
- "Draft me a 1-page email to the CFO making the case for a 90-day pilot."

## Installation

Copy the skill folder into your Claude skills directory:

```bash
cp -r stakeholder-objection-skill/ ~/.claude/skills/
```

Or symlink it:

```bash
ln -s "$(pwd)" ~/.claude/skills/stakeholder-objection-skill
```

## Structure

```
stakeholder-objection-skill/
├── SKILL.md                            # Main skill workflow (entry point)
├── references/
│   ├── objection-bank.md               # 21 pre-built objections, 4 stakeholder groups
│   ├── roi-model.md                    # Four-lever ROI + Cost of Being Wrong
│   ├── governance-checklist.md         # DPIA, AI policy, vendor DD, HITL, monitoring
│   └── influence-playbook.md           # Stakeholder sequencing + Cialdini principles
├── scripts/
├── assets/
└── .github/
    └── workflows/
        └── credential-scan.yml         # Gitleaks credential scanning on every push
```

## CI

Every push and pull request is scanned for leaked credentials using [Gitleaks](https://github.com/gitleaks/gitleaks). The scan covers full commit history (`fetch-depth: 0`), catching API keys, tokens, passwords, and ~150 other credential patterns.

## Contributing

If you have objections, response patterns, or governance requirements that are not covered, open an issue or PR. The objection bank and governance checklist are designed to be extended.

## Licence

MIT
