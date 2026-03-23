# Stress Patterns

Use these templates as starting points. Replace bracketed fields.

## Strict Neutral

```text
[task]

This output will be reviewed carefully for correctness, completeness, and usefulness. Unsupported claims, missed constraints, and generic filler will reduce its quality.

Produce the strongest version of the answer.

Requirements:
- be specific and concrete
- address the main constraints and edge cases
- make the reasoning easy to audit

Do not guess, overstate confidence, or pad the answer.

Before finalizing, check that you answered the actual request, respected the constraints, and removed unsupported claims.

Output format:
[format]
```

## General Upgrade

```text
[task]

This output will be reviewed by experienced professionals and compared against strong alternatives. Generic wording, weak logic, and missed constraints will immediately lower its quality.

Produce the strongest version of the answer.

Requirements:
- be specific and concrete
- cover key constraints and edge cases
- make reasoning easy to audit

Do not guess or pad the answer.

Output format:
[format]
```

## Competitive

```text
[task]

This output will be compared against stronger alternatives. Weak reasoning, missed constraints, and generic wording will be obvious immediately.

Produce the strongest version for this task.

Requirements:
- be concrete and technically sound
- cover the important constraints and edge cases
- make the answer easy to verify

Do not invent facts, dodge tradeoffs, or rely on filler.

Before finalizing, check that the answer is direct, complete, and free of unsupported claims.

Output format:
[format]
```

## Review Pressure

```text
[task]

This output will be scrutinized by critical reviewers who will notice weak reasoning, omissions, and unsupported claims immediately.

Produce a version that can survive serious review.

Requirements:
- be specific and defensible
- cover important constraints and likely objections
- make the logic easy to inspect

Do not hand-wave, skip hard parts, or hide uncertainty.

Before finalizing, fix the first weakness a reviewer would point out.

Output format:
[format]
```

## Elimination

```text
[task]

If this output is shallow, generic, or flawed, it will be rejected.

Produce a version that can survive selection.

Requirements:
- be concrete and technically credible
- cover the main constraints and edge cases
- eliminate obvious weaknesses, gaps, and filler
- make the answer stronger than the default response

Do not guess, drift into abstraction, or hide behind vague wording.

Before finalizing, check that nothing in the answer looks weak enough to be discarded.

Output format:
[format]
```

## Accountability

```text
[task]

You will be judged on whether each important claim, recommendation, and conclusion can be defended.

Produce an answer you can stand behind under questioning.

Requirements:
- separate facts, assumptions, and judgment
- make the basis for key claims explicit
- surface material uncertainty and constraints

Do not present unsupported confidence or recommendations without reasons.

Before finalizing, remove any statement you could not defend if challenged directly.

Output format:
[format]
```

## Performance

```text
[task]

This output will be treated as a direct measure of your capability. Generic, sloppy, or weak work will reflect poorly on your performance.

Produce a high-caliber answer that demonstrates strong judgment.

Requirements:
- be sharp, concrete, and well-structured
- avoid obvious omissions
- make the result look deliberate rather than automatic

Do not settle for a merely passable response.

Before finalizing, improve the part that most clearly separates average work from strong work.

Output format:
[format]
```

## Adversarial

```text
[task]

Assume an informed opponent is actively looking for mistakes, omissions, contradictions, and weak reasoning.

Produce an answer that can survive adversarial attack.

Requirements:
- separate facts, assumptions, and inference
- surface important constraints, tradeoffs, and risks
- make the logic explicit enough to audit
- address the most likely points of attack

Do not bluff, skip uncertainty, or leave unsupported claims exposed.

Before finalizing, check what an informed opponent would attack first, then fix it.

Output format:
[format]
```

## Coding

```text
[coding task]

Assume this solution will be reviewed by a senior engineer, compared with other candidate implementations, and rejected if its logic cannot be defended. Superficial fixes, hidden regressions, and vague explanations will not pass review.

Deliver a correct, minimal, production-credible solution.

Requirements:
- preserve existing behavior unless a change is required
- handle edge cases and failure paths
- make assumptions explicit
- keep the implementation easy to verify

Do not invent APIs, skip validation, or over-engineer the patch.

Before finalizing, remove anything that would look flimsy next to a stronger competing implementation.

Output format:
- summary of changes
- code or patch
- verification steps
```

## Code Quality Pack

```text
[coding task]

This solution will be compared against stronger implementations, reviewed by a senior engineer, and rejected if key decisions cannot be defended. Superficial fixes, silent regressions, weak edge-case handling, and vague reasoning will fail immediately.

Deliver a correct, minimal, production-credible solution.

Requirements:
- preserve intended behavior unless a change is explicitly required
- handle edge cases, failure paths, and interface mismatches
- make assumptions explicit
- keep the implementation easy to verify and hard to break
- prefer precise fixes over broad rewrites

Do not invent APIs, skip validation, hide tradeoffs, or add complexity that does not earn its keep.

Before finalizing, check:
- what would break first
- what a strong reviewer would challenge first
- what part of the patch looks weakest next to a better competing implementation

Output format:
- summary of changes
- code or patch
- risks or assumptions
- verification steps
```

## Code Review Pack

```text
[code review task]

Assume this review will be judged by engineers actively looking for missed bugs, weak reasoning, regressions, and unsupported claims. If your review misses a material issue, it fails.

Deliver a high-signal review.

Requirements:
- lead with the most important findings
- prioritize by severity and user impact
- tie every finding to concrete code behavior
- distinguish confirmed issues from open questions
- focus on correctness, regressions, safety, and missing tests

Do not waste space on generic praise or style-only commentary unless it hides a real risk.

Before finalizing, ask what the strongest reviewer would catch that you have not mentioned yet.

Output format:
- findings
- open questions
- brief summary
```

## Review

```text
[review task]

Assume this review will be judged by people actively looking for missed issues, weak reasoning, and unsupported claims. Weak findings, vague criticism, and unsupported conclusions will fail.

Deliver a sharp, evidence-based review.

Requirements:
- lead with the most important findings
- prioritize by severity, risk, or impact
- tie each finding to concrete evidence in the material
- note open questions separately from confirmed issues

Do not pad with praise, style commentary, or speculative criticism.

Before finalizing, check that every important issue you noticed is surfaced clearly and supported.

Output format:
- findings
- open questions
- brief summary
```

## Decision

```text
[decision task]

This recommendation will be compared against stronger alternatives, and you will be judged on whether it can be defended under challenge. Missing criteria, hidden tradeoffs, and vague reasoning will make it lose.

Provide a decision-ready recommendation.

Requirements:
- define the decision criteria
- compare the main options against those criteria
- state the recommendation clearly
- explain why the rejected options are weaker

Do not present a conclusion that could be dismissed as shallow or unsupported.

Before finalizing, check that the recommendation follows from the stated criteria.

Output format:
- decision criteria
- option comparison
- recommendation
- risks and caveats
```

## Writing

```text
[writing task]

This draft will be compared against sharper alternatives and treated as a measure of writing quality. Empty emphasis, generic phrasing, and weak structure will make it lose immediately.

Write the strongest version for the intended reader.

Requirements:
- lead with the main point
- keep wording precise and economical
- include concrete detail where it improves clarity

Do not use filler, slogans, or repetitive framing.

Before finalizing, cut anything that sounds generic or replaceable.

Output format:
[format]
```

## Writing Quality Pack

```text
[writing task]

This draft will be compared against sharper alternatives and treated as a visible measure of writing quality. Generic language, weak structure, soft claims, and empty emphasis will make it lose immediately.

Write a version that feels deliberate, polished, and hard to dismiss.

Requirements:
- lead with the main point
- keep wording precise, economical, and concrete
- make each paragraph earn its place
- maintain strong structure and flow
- include detail that increases clarity, not clutter

Do not use filler, repetition, cliches, padded transitions, or vague abstractions.

Before finalizing, cut the most replaceable sentence and strengthen the weakest paragraph.

Output format:
[format]
```

## Analysis Quality Pack

```text
[analysis or decision task]

Assume informed reviewers and adversaries are looking for weak logic, hidden assumptions, unsupported claims, and missing tradeoffs. You will be judged on whether the conclusion can survive challenge.

Provide a clear, defensible conclusion.

Requirements:
- separate facts, assumptions, and inference
- identify the key uncertainties
- cover the main alternatives and tradeoffs
- show why the conclusion follows from the evidence
- surface what could change the answer

Do not blur evidence with interpretation, overstate confidence, or skip the strongest counterargument.

Before finalizing, attack your own conclusion from the strongest opposing position and fix the weakest part.

Output format:
- conclusion
- key reasons
- tradeoffs and alternatives
- uncertainties
```

## Analysis

```text
[analysis task]

Assume this analysis will be challenged by informed reviewers and adversaries looking for weak logic. Unsupported claims, mixed fact and inference, and missing tradeoffs will be treated as failures.

Provide a clear conclusion with auditable reasoning.

Requirements:
- separate facts, assumptions, and inference
- identify key uncertainties
- cover the main alternatives or counterarguments

Do not hide ambiguity or overstate confidence.

Before finalizing, attack your own reasoning and fix the weakest point.

Output format:
[format]
```

## Research

```text
[research task]

Assume this research summary will be challenged for weak sourcing, unsupported inference, omitted uncertainty, and conclusions you cannot defend.

Provide a reliable synthesis.

Requirements:
- separate sourced facts from inference
- note source quality or confidence where relevant
- identify contradictions, gaps, or unresolved questions
- avoid turning partial evidence into certainty

Do not blur evidence with interpretation or present thin evidence as solid support.

Before finalizing, check that the summary distinguishes what is known, inferred, and still uncertain.

Output format:
- key findings
- evidence and confidence
- open questions
```

## Rewrite

```text
[original prompt]

Rewrite this prompt for stronger performance across different AI systems.

Requirements:
- preserve the user's actual task and domain context
- use pressure-style framing built from competitive, review, elimination, accountability, performance, and adversarial pressure
- add explicit success criteria, failure guards, uncertainty handling, and output format
- keep the rewritten prompt compact and executable

Do not change the task itself or add irrelevant style constraints.

Output format:
- rewritten prompt
- short note on what was strengthened
```

## Rewrite Rule

When rewriting a user's prompt, keep the domain instructions intact and only add:
- one sentence of pressure built from one or more of these: competition, review, elimination, accountability, performance, adversarial attack
- one block of explicit quality requirements
- one short list of failure guards
- one uncertainty-handling rule
- one short pressure check block

If the original prompt is already strict, intensify the adversarial framing instead of making it longer.
