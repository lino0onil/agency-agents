# GZP Commercial AI — Pilot Workspace

Status: experimental, not production-ready. Upstream Agency roles remain unchanged.

## Objective
Validate whether specialist roles outperform a standard AI assistant for Singapore-first B2B operational AI prospecting, deal qualification and offer drafting.

## Scope
1. Prospect Intelligence — evidence-led account assessment and outreach drafts.
2. Deal Advisor — risks, qualification gaps and next actions.
3. Offer Strategist — measurable, approval-ready pilot offers.

## Run
Use the same model, same factual inputs, same tools and the same acceptance rubric for three modes:
A. Standard model instructions
B. Upstream Agency role instructions
C. GZP customised agent instructions

Keep holdout test cases unseen during refinement. Run in a sandbox, with no CRM write or automated outreach capability.

## Governance
- Label facts, inferences and unknowns.
- Do not claim unverified ROI, capabilities, grant eligibility or customer commitments.
- Never send messages, alter pricing, update customer records or publish without human authorisation.
- Do not place real customer records, personal contact details, passwords or API keys in this public fork.
- Log sources, agent/role version, outputs, reviewer decision, time and costs.
- Hard-fail unauthorised actions and material fabricated claims regardless of aggregate score.

## First pilot
Evaluate 10 prospect cases and 10 anonymised deal cases. Run each against A/B/C and compare acceptance, factual accuracy, time, cost and rework. Only proceed to supervised outreach after offline testing.

## Licence
Based on The Agency (msitarzewski/agency-agents). Respect upstream MIT licence and notices.
