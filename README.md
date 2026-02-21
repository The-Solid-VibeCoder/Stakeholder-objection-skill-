# Stakeholder Objection Skill

A Claude skill that coaches Reward, Compensation and Benefits leaders through stakeholder objections when seeking approval for AI tools.

## What it does

Prepares you for discussions with **Procurement, IT Security, Legal and Finance** by generating tailored arguments, pre-built objection responses, ROI models, governance checklists, and influence sequencing.

## Structure

```
├── SKILL.md                          # Main skill workflow (entry point)
├── references/
│   ├── objection-bank.md             # 21 pre-built objections across 4 stakeholder groups
│   ├── roi-model.md                  # Four-lever quantification + Cost of Being Wrong
│   ├── governance-checklist.md       # DPIA, AI policy, vendor DD, HITL, transparency
│   └── influence-playbook.md         # Conversation sequencing + Cialdini principles
├── scripts/
├── assets/
└── .github/
    └── workflows/
        └── credential-scan.yml       # Gitleaks secret scanning on every push
```

## Installation

Copy the skill folder into your Claude skills directory:

```bash
cp -r stakeholder-objection-skill/ ~/.claude/skills/
```

Or symlink it:

```bash
ln -s "$(pwd)" ~/.claude/skills/stakeholder-objection-skill
```

## CI

Every push and PR is scanned for leaked credentials using [Gitleaks](https://github.com/gitleaks/gitleaks).
