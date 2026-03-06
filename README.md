# Finding First Customer
### A Positive Deviance Approach

A Claude skill for zero-to-one product discovery. Gets you to a paying user faster than any framework that starts with ideation.

**The thesis:** Users who are already solving a problem badly — with spreadsheets, DMs, copy-paste, or hired help — are proof that the problem is urgent. Find them. Do the thing manually. Charge them. Then build.

---

## What It Does

Installs a structured product discovery workflow into Claude that:

- Identifies observable workarounds (not stated preferences)
- Classifies workaround type by willingness-to-pay signal
- Tests for independent parallel invention (pattern vs. anecdote)
- Forces a concierge transaction before any code is written
- Outputs an exact DM script to send to your first customer today

**Verdict system:**

| Verdict | Meaning |
|---|---|
| `CHARGE NOW (MANUALLY)` | Paid workaround found — send the DM, charge before building |
| `INTERVIEW AND CHARGE` | Workaround found — talk to 3 deviants this week, attempt charge |
| `WATCH AND WAIT` | Pattern emerging, not enough cases yet |
| `DISCARD` | No observable workaround — move on |

---

## Install

1. Download `finding-first-customer.skill`
2. Drop it into your Claude skills directory:
   - Claude Code: `~/.claude/skills/`
   - Claude.ai: Settings → Skills → Upload
3. Restart Claude

---

## Usage

Once installed, trigger it by asking Claude anything like:

- *"Help me find my first customer for [idea]"*
- *"Is this worth building?"*
- *"What should I build in [market]?"*
- *"Validate this idea: [description]"*
- *"How do I get my first paying user?"*

Claude will run the full positive deviance workflow and output a deviance table, first customer profile, workaround cost calculation, and a verdict with an exact next action.

---

## What It Won't Do

- TAM estimates
- Competitive landscape analysis
- Roadmap planning
- GTM beyond first 10 customers

This skill terminates at first paying user. Use a different framework for scale.

---

## Methodology

Built on positive deviance theory applied to product discovery:

- Workarounds are behavioral proof of urgency — stronger than any survey
- Paid workarounds are direct evidence of willingness-to-pay
- Independent parallel invention separates markets from feature requests
- The concierge transaction (manual delivery, real charge) is the fastest validation possible

Inspired by: Zappos (sold shoes manually before building the store), Airbnb (photographed apartments themselves), Superhuman (onboarded users 1:1 before scaling).

---

## Contributing

PRs welcome. Especially interested in:
- Additional worked examples across different domains
- Edge cases where the framework breaks
- Refinements to the concierge gate logic

---

## License

MIT
