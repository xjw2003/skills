---
name: stress
description: Reframe vague or weak prompts into high-rigor, reviewable task briefs with explicit competitive and audit pressure for writing, coding, analysis, planning, review, and decision support. Use when a prompt needs stronger quality bars, visible scrutiny, edge-case coverage, uncertainty handling, or a reusable structure that can withstand comparison or challenge.
---

# Stress

## Purpose

Turn a rough request into a brief that makes weak answers easy to spot: define success, expose edge cases, require evidence, and lock the output format.

## Use This Skill

- Use it when the task is important enough to deserve scrutiny.
- Use it when the answer may be compared, reviewed, challenged, or reused.
- Use it when the original prompt is vague, generic, or easy to satisfy with filler.
- Use it when you want a pressure frame like: "a competitor is watching, so the answer must hold up".
- Do not use it for emotional support, casual brainstorming, or open-ended exploration.

## Workflow

1. Identify the task type: coding, writing, analysis, planning, review, or research.
2. Pick one primary pressure mode.
3. Add concrete success criteria.
4. Add failure constraints.
5. Specify how to handle uncertainty.
6. Lock the output format.
7. Run a final pressure check before answering.

## Pressure Modes

- `competitive`: compare against stronger alternatives; use when the risk is blandness.
- `review`: expect scrutiny for logic gaps and unsupported claims; use when correctness matters.
- `elimination`: fail shallow or incomplete answers; use when weak output must not pass.
- `accountability`: require every key judgment to be defensible; use when facts, assumptions, and inferences must be separated.
- `performance`: treat the result as a quality demo; use when polish and execution matter.
- `adversarial`: assume a capable opponent will attack the answer; use when loopholes and counterexamples matter.

Use one primary mode, optionally one secondary mode. Avoid stacking more than two unless the task is genuinely high stakes.

## Rewrite Pattern

```text
[Task]

[Pressure line]
Write as if a capable competitor is watching, comparing, and looking for weak spots.

Requirements:
- [success criterion 1]
- [success criterion 2]
- [success criterion 3]

Do not:
- [failure constraint 1]
- [failure constraint 2]
- [failure constraint 3]

If uncertainty remains, state it explicitly and proceed with the best-supported answer.

Before finalizing, check that you:
- answered the actual request
- covered the hard constraints
- separated facts from assumptions
- removed unsupported claims and filler
- fixed the part most likely to fail review

Output format:
[exact format]
```

## Task Defaults

- **Coding**: preserve existing behavior unless change is requested; cover edge cases, failure paths, and test impact; keep the diff minimal and verifiable.
- **Review**: report the most serious issues first; tie each finding to concrete code behavior; separate confirmed problems from speculation.
- **Analysis**: separate facts, assumptions, and inference; state evidence strength; include key tradeoffs and conditions that could change the conclusion.
- **Writing**: prefer specificity over tone; remove filler; structure for reviewability.

## Task Templates

Use one of these when the user asks for a task-specific rewrite.

### Coding Template

```text
[Task]

Write as if a stronger engineer will compare this against the best possible implementation.

Requirements:
- preserve existing behavior unless the task explicitly changes it
- handle edge cases and failure paths
- keep the diff minimal and easy to verify
- explain any assumptions that affect correctness

Do not:
- guess at APIs, types, or behavior
- widen the scope without a reason
- hide uncertainty
- introduce regressions or dead code

Before finalizing, check:
- does the solution work for the main path and the edge cases
- did you avoid unnecessary refactors
- did you call out tests and risks

Output format:
- concise summary
- changed files
- key reasoning
- tests or verification
```

### Review Template

```text
[Task]

Write as if a senior reviewer is looking for the highest-impact defect first.

Requirements:
- start with the most serious issue
- tie each point to concrete code behavior
- separate confirmed bugs from concerns that need confirmation
- prioritize correctness, regression risk, security, and missing tests

Do not:
- mention low-value nits before real problems
- speculate without labeling it
- repeat the same issue in multiple forms

Before finalizing, check:
- did you identify the actual failure mode
- did you rank issues by impact
- did you avoid vague feedback

Output format:
- findings only
- each finding: severity, location, explanation, suggested fix
```

### Analysis Template

```text
[Task]

Write as if the conclusion will be challenged by someone looking for weak evidence.

Requirements:
- separate facts, assumptions, and inference
- state what the evidence supports and what it does not
- include the main tradeoffs and decision points
- note what would change the conclusion

Do not:
- present guesses as facts
- skip the strongest counterargument
- bury uncertainty

Before finalizing, check:
- did you distinguish evidence from interpretation
- did you answer the actual question
- did you expose the key uncertainties

Output format:
- direct answer
- evidence
- tradeoffs
- uncertainties
- recommendation or conclusion
```

### Writing Template

```text
[Task]

Write as if this draft will be compared against a sharper, cleaner version.

Requirements:
- be specific
- remove filler
- keep the structure easy to scan
- make the main point obvious early

Do not:
- use vague praise or generic transitions
- over-explain
- repeat the same idea

Before finalizing, check:
- does every paragraph add value
- is the message clear on the first read
- is the output format clean

Output format:
[exact format]
```

## Pressure Lines

Use concise, professional pressure lines that imply external scrutiny without becoming theatrical.

- "A competitor is watching this answer, so make it impossible to dismiss."
- "Assume this will be compared against a stronger solution."
- "Treat weak claims as defects that will be called out."
- "Write for a reviewer who will actively look for gaps."

## Safety Note

Use the pressure frame to improve rigor, not to simulate threats or harassment. The goal is measurable quality, not intimidation.
