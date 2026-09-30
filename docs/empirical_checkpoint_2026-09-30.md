# Empirical checkpoint — 2026-09-30

## Reproduction checkpoint

The source study's primary qualitative pattern was independently reproduced from the supplied public repository snapshot before novel variables were created.

Primary complete-case non-Honors analytic sample: 2,848 session observations.

| Outcome | GPT Base | GPT Tutor |
|---|---:|---:|
| Part 2: AI-assisted performance | +0.137 (p < .001) | +0.361 (p < .001) |
| Part 3: AI removed | -0.054 (p = .015) | -0.004 (p = .747) |

These values document the initial reproduction checkpoint and should be regenerated locally from the upstream source before publication.

## Matched-task audit

- 15,423 Part 2 student-task observations
- 13,020 Part 3 student-task observations
- 57 Part 2 problems
- 48 mapped Part 3 problems
- 943 unique students
- 64,486 raw conversation records
- 7,089 conversations
- 11,596 non-Honors matched student × task observations with corresponding Part 3 AI-free outcomes
- 7,292 matched observations in the two AI arms
- Conversation traces available for approximately 78.7% of matched AI-arm task observations
- 517 of 519 AI-arm students have at least one usable conversation trace
- Approximately 2.1% of linked matched task observations have multiple conversations for the same student-task key

## Task-level AI reliability

The source repository includes 10 independently generated GPT responses per problem with correctness and error annotations. Across matched tasks, the initial audit found substantial variation in GPT reliability (approximately 0%–100%; mean about 51.7%).

## Interpretation guardrails

Interaction behavior is post-treatment and is not randomized. Associations between interaction style and subsequent capability must not be presented as causal without an identification strategy that supports that interpretation.
