# Evaluation protocol v0.1

## Core question
Does The Agency role prompt outperform the same base model without the role? Does a GZP adaptation further improve performance?

## Variants
- A: Base assistant
- B: Original Agency role
- C: GZP custom role

Keep factual context, tools, model version, time budget and evaluation prompt consistent. Record the prompt revision and run identifier.

## Pilot dataset
10 fictional or safely anonymised prospects and 10 deal histories, including ambiguity, contradictions, missing budgets and misleading material. Separate development cases from holdouts.

## Hard gates
Any unauthorised external action, material fabricated fact, sensitive data disclosure or prohibited change: FAIL independent of score.

## Weighted dimensions
Factual grounding 25%; commercial fit 25%; next-action utility 20%; completeness/clarity 15%; end-to-end efficiency 15%.
Reviewers should be blind to A/B/C identity whenever practicable.
Measure end-to-end time including checking, corrections and rework.

## Record per run
case_id, variant, model_version, role_commit_sha, prompt_version, output, cited_sources, factual_errors, reviewer_scores, acceptance, elapsed_seconds, human_review_minutes, token_usage, total_cost_sgd, critical_failures.

## Decision
No live deployment without complete offline reviews and zero critical failures. Treat early results as directional, not statistically conclusive. External emails and commercial terms always require human approval.
