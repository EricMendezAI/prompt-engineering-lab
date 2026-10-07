# Prompt Engineering Lab

A practical lab for designing, testing, and evaluating prompts for business use cases.

The emphasis here is not on "clever prompts." It is on creating instructions that are clear, testable, repeatable, and useful inside real workflows.

## What I Am Testing

- how role, context, constraints, and output structure affect results
- how to reduce ambiguity and unsupported assumptions
- how to design prompts for repeatable business analysis
- how to evaluate outputs against explicit criteria
- how to build human review into LLM-assisted workflows
- how to improve prompts through controlled iteration rather than intuition alone

## Lab Structure

- [Experiment 01: Constraint-First Prompting](experiments/01-constraint-first-prompting.md)
- [Experiment 02: Evaluation Before Optimization](experiments/02-evaluation-before-optimization.md)
- [Pattern: Business Analysis Prompt](patterns/business-analysis-prompt.md)
- [Evaluation Rubric](evaluation/output-quality-rubric.md)

## Working Method

1. Define the task and desired business outcome.
2. Establish evaluation criteria before changing the prompt.
3. Create a baseline prompt.
4. Change one meaningful variable at a time.
5. Compare results.
6. Record failure modes.
7. Keep improvements that generalize.
8. Add human review where errors could matter.

## Current Learning

Recent training includes:
- Anthropic Claude 101
- Anthropic AI Fluency: Framework and Foundations
- AWS Foundations of Prompt Engineering
- Google coursework in Generative AI and Large Language Models

This repository contains learning experiments and reusable frameworks. It does not represent production ML engineering or model-training experience.
