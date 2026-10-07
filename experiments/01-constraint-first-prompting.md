# Experiment 01: Constraint-First Prompting

## Question

Does explicitly defining constraints produce a more useful business output than simply asking for a "better" answer?

## Business Scenario

A manager needs an executive summary of a long operational update. The summary must be short enough for leadership, preserve material risks, and distinguish facts from recommendations.

## Baseline Prompt

> Summarize this operational update for leadership.

### Likely Failure Modes

- inconsistent length
- too much background
- loss of important risks
- recommendations mixed with facts
- unclear ownership or next steps

## Constraint-First Version

> Summarize the operational update for a senior leadership audience.
>
> Requirements:
> - Maximum 200 words.
> - Preserve all material risks, deadlines, and unresolved decisions.
> - Separate confirmed facts from recommendations.
> - Do not invent missing context.
> - Identify the three items that most need leadership attention.
> - Use this structure:
>   1. Current state
>   2. Key risks
>   3. Decisions/actions needed

## Evaluation Criteria

Score each output from 1–5 on:
- factual fidelity
- completeness of material risks
- concision
- decision usefulness
- clarity of facts vs. recommendations
- adherence to requested format

## Hypothesis

The constraint-first prompt should outperform the baseline because "good summary" is subjective, while the revised prompt defines what usefulness means for this specific audience.

## What This Demonstrates

Prompt quality is often less about adding more words and more about removing ambiguity.

For repeatable business use, the prompt should tell the model:
- who the output is for,
- what must be preserved,
- what must not happen,
- how success will be judged,
- and what structure the workflow expects.

## Next Test

Run both versions against several different operational updates and compare rubric scores. A useful improvement should generalize across inputs rather than work only on one example.
