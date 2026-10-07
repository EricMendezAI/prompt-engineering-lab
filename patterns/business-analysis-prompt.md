# Pattern: Business Analysis Prompt

A reusable structure for LLM-assisted business analysis.

## Template

```text
ROLE
Act as a [relevant business role or analytical perspective].

OBJECTIVE
Analyze the supplied information to [specific business outcome].

CONTEXT
[Explain the situation, audience, decision, and relevant operating context.]

SOURCE BOUNDARY
Use only the information provided.
Do not invent facts, metrics, causes, or stakeholder views.
When information is insufficient, state what is unknown.

ANALYSIS
Evaluate:
1. [dimension]
2. [dimension]
3. [dimension]

Separate:
- observed facts
- reasonable inferences
- unresolved questions
- recommendations

PRIORITIZATION
Rank issues/opportunities using:
- business impact
- urgency
- evidence strength
- implementation difficulty

OUTPUT
Return:
1. Executive summary
2. Key findings
3. Root-cause hypotheses
4. Recommended actions
5. Risks/unknowns
6. Metrics to monitor

QUALITY CHECK
Before finalizing, verify that:
- every material claim is supported by the supplied information,
- recommendations are clearly labeled,
- no missing information was silently assumed,
- the output follows the requested structure.
```

## Why This Pattern Works

It gives the model a clear job while preventing several common business-use failure modes:
- hidden assumptions
- recommendations presented as facts
- vague prioritization
- overconfident conclusions
- inconsistent output structure

## When to Modify It

Use fewer sections for low-risk, high-volume workflows. Add more explicit validation or human review for decisions involving customers, money, compliance, employment, or other meaningful consequences.
