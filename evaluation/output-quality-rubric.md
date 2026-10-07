# Output Quality Rubric

A lightweight rubric for evaluating LLM outputs used in business workflows.

Score each category from **1 to 5**.

## 1. Grounding

**1:** Material claims are invented or unsupported.  
**3:** Mostly grounded with minor unsupported interpretation.  
**5:** Claims are traceable to the supplied information; uncertainty is explicit.

## 2. Task Completion

**1:** Misses the requested objective.  
**3:** Completes the core task but misses secondary requirements.  
**5:** Fully addresses the stated objective and required components.

## 3. Accuracy

**1:** Material factual or logical errors.  
**3:** Minor issues that do not change the overall conclusion.  
**5:** No material errors identified during review.

## 4. Decision Usefulness

**1:** Generic or difficult to act on.  
**3:** Useful with additional interpretation.  
**5:** Clear, prioritized, and directly supports the intended decision or workflow.

## 5. Clarity

**1:** Disorganized or ambiguous.  
**3:** Generally clear with some unnecessary complexity.  
**5:** Concise, structured, and easy for the target audience to use.

## 6. Constraint Adherence

**1:** Ignores important instructions.  
**3:** Meets most constraints.  
**5:** Consistently follows format, scope, length, and source boundaries.

## Suggested Acceptance Rule

For a low-to-moderate-risk business workflow:
- no category below **3**
- average score of at least **4**
- grounding must score **4 or 5**

Higher-risk workflows should add domain-specific checks and mandatory human review.

## Failure Log

When an output fails, record:
- input type
- prompt version
- failure category
- example of the failure
- likely cause
- proposed change
- whether the change improved later tests

This turns prompt iteration into a repeatable learning process instead of ad hoc rewriting.
