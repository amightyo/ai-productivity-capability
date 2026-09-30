# Milestone 02 — Conversation Discovery

## Purpose
Develop the first cognitive-engagement taxonomy from observed AI interactions before applying NLP or LLM labeling.

## Linkage audit
Each conversation ID in the source logs maps to exactly one problem ID. System prompts are excluded from behavioral coding. The working linkage connects AI-arm Part 2 task performance, conversation traces, mapped Part 3 AI-free performance, and task-level GPT reliability.

## Stratified discovery sample
24 conversations were selected across AI arm, task reliability, and subsequent matched-task performance. This was a discovery sample, not an inferential sample.

## Main methodological finding
A single “delegation” category is empirically inadequate. Observed interactions distinguish at least direct-answer solicitation, generic help without an attempt, learner-generated answer verification, targeted conceptual requests, scaffold uptake, repeated dependence after scaffolding, and answer-persistence behavior.

The same broad behaviors appear among both later-success and later-failure cases. Therefore, the project will preserve **ordered interaction sequences** and model them jointly with task reliability rather than assign simplistic beneficial/harmful labels to isolated messages.

## Decision
Freeze Codebook v0.1 as a discovery artifact. Do not train an automated classifier until a blinded human-validation sample has been independently coded.
