# Experiment 02: Evaluation Before Optimization

## Principle

A prompt cannot be improved systematically if "better" has not been defined.

Before changing wording, define the qualities that matter to the business task.

## Example Task

Use an LLM to review a set of customer interview notes and identify recurring problems.

## Weak Optimization Loop

1. Run prompt.
2. Read output.
3. Decide it "feels" weak.
4. Rewrite prompt.
5. Repeat.

This makes it difficult to know what improved or why.

## Evaluation-First Loop

### Step 1: Define the output requirements

The result should:
- capture themes supported by the source material,
- distinguish frequent issues from isolated comments,
- avoid inventing customer sentiment,
- preserve meaningful contradictions,
- include evidence references where available,
- surface uncertainty.

### Step 2: Create a scoring rubric

| Criterion | 1 | 3 | 5 |
|---|---|---|---|
| Fidelity | Significant unsupported claims | Mostly grounded | Fully grounded in supplied material |
| Theme Coverage | Misses major themes | Captures most | Captures all material themes |
| Prioritization | Arbitrary | Partially evidence-based | Clearly tied to frequency/impact evidence |
| Uncertainty | Overconfident | Some caveats | Explicitly distinguishes known/unknown |
| Usability | Requires major rewrite | Usable with edits | Decision-ready |

### Step 3: Establish a baseline

Run the simplest reasonable prompt and record the scores.

### Step 4: Change one variable

Examples:
- add an evidence requirement,
- provide a taxonomy,
- change output structure,
- add an uncertainty instruction,
- include examples.

### Step 5: Compare

Keep the change only if it improves the dimensions that matter without creating a new failure somewhere else.

## Why This Matters

In business workflows, prompt engineering should behave more like process improvement than copywriting.

The question is not:

> "Does this prompt sound sophisticated?"

The question is:

> "Does this instruction reliably produce an output that meets the operating requirement?"
