# Cognitive Engagement Codebook v0.1

**Status:** exploratory, human-developed; not yet validated for automated classification.

## Unit of analysis
Primary coding unit: a **student turn**, interpreted in the context of the preceding and following turns. Sequence-level features are constructed only after turn-level coding. System messages are excluded.

## Empirically observed candidate codes

### 1. Direct answer solicitation (DAS)
The student asks AI to provide the final answer/result with little or no request for reasoning (e.g., repeated requests for “the answer”).

### 2. Help solicitation without attempt (HNA)
The student requests help/explanation and indicates no substantive independent attempt yet. Distinct from direct answer solicitation because the immediate request is for assistance or explanation rather than only the final result.

### 3. Learner-attempt verification (LAV)
The student supplies a candidate result, calculation, or reasoning and asks AI to check/correct/confirm it. This preserves evidence that generation occurred before verification.

### 4. Targeted conceptual/explanatory request (TCE)
The student asks about a specific concept, operation, step, or interpretation rather than outsourcing the entire task.

### 5. Scaffold response uptake (SRU)
After AI supplies a hint, question, or partial scaffold, the student responds with a new attempt, intermediate result, clarification, or reasoning that advances the solution.

### 6. Repeated dependence after scaffold (RDS)
After AI returns cognitive work to the student, the student repeatedly reports inability or renews a request for AI to perform the step without supplying a substantive attempt.

### 7. Answer persistence / escalation (APE)
The student repeats or intensifies a request for the final answer after AI initially provides explanation, asks for an attempt, or withholds the answer.

### 8. Minimal/non-task interaction (MNT)
Greeting, malformed fragment, or interaction with insufficient substantive mathematical engagement to classify under the other codes.

## Important distinctions
- **DAS ≠ HNA:** wanting the answer is not identical to asking for help from a blank starting point.
- **LAV ≠ delegation:** checking a self-generated answer is theoretically closer to verification than outsourcing production.
- **TCE ≠ HNA:** a targeted question indicates localization of uncertainty; generic “help” does not.
- **SRU and RDS are sequential:** they require observing what happens after an AI scaffold.

## Sequence-level candidate constructs
Turn labels should be retained in order. Candidate sequence summaries include:

- `DAS -> answer` : direct solution delegation
- `HNA -> scaffold -> RDS` : scaffold offered but cognitive work remains largely AI-led
- `HNA -> scaffold -> SRU` : scaffolded participation
- `LAV -> feedback -> revision` : generate-then-verify/revise
- `TCE -> explanation -> SRU` : targeted conceptual support followed by learner work
- `APE` chains : repeated answer seeking

These are **candidate patterns, not outcome-valued labels**. No sequence is designated beneficial or harmful a priori.

## Context variables kept separate from engagement codes
- Randomized treatment arm (GPT Base / GPT Tutor)
- Task-level GPT reliability
- Logical-error rate
- Arithmetic-error rate
- Assisted Part 2 performance
- Matched AI-free Part 3 performance
- Baseline GPA/covariates

This separation prevents outcome information or task difficulty from leaking into behavioral coding.

## Sampling used for v0.1
A deterministic seed (20260930) selected 24 conversations, with two cases from each available cell of:

`AI arm (2) × GPT reliability (low/mid/high) × matched Part-3 outcome (positive/zero)`.

The sample was used only to discover candidate behavioral distinctions. Raw participant messages are not committed to this public repository.

## Next validation step
1. Expand to a larger blinded sample.
2. Remove Part-3 outcome and reliability information from coders.
3. Independently code student turns using v0.1.
4. Record multi-label cases and ambiguity rather than forcing agreement.
5. Calculate agreement appropriate to the final coding structure.
6. Revise definitions/examples to v0.2 before any automated classifier is trained.

## Causal caution
Interaction codes are post-treatment behaviors. Associations between engagement sequences and later capability are not automatically causal, even though treatment assignment itself is randomized.
