---
name: stress
description: Raise output rigor by rewriting prompts with calibrated pressure, explicit quality bars, failure guards, and strict output formats. Use when the user wants stronger prompt rewrites, sharper analysis, more defensible reviews, or higher-effort coding and writing results. Avoid when the task mainly needs empathy, friendly tutoring, casual brainstorming, or low-pressure conversation.
---

# Stress

Use this skill to rewrite a weak or under-specified prompt into one that pushes for higher rigor.

The mechanism is controlled pressure:
- comparison against stronger alternatives
- critical review and audit pressure
- rejection of shallow output
- accountability for claims and recommendations
- performance pressure
- adversarial scrutiny

Pressure is the primary lever, but it must stay professional. Do not use melodrama, insults, or childish threats.

## When To Use

Use `stress` when the user wants one of these outcomes:
- a prompt rewrite that makes weak output less likely
- stronger coding, review, analysis, research, or writing prompts
- clearer evaluation criteria and failure guards
- higher defensibility, specificity, and edge-case coverage

Strong fit:
- prompt engineering
- code review prompts
- implementation prompts
- research and analysis prompts
- decision-support prompts
- polished writing prompts

## When Not To Use

Do not apply this skill by default when the task mainly needs:
- empathy or emotional support
- friendly tutoring for beginners
- open-ended ideation where pressure would narrow exploration too early
- casual conversation
- a direct answer instead of a prompt rewrite

If the user wants stronger output but not an explicit prompt rewrite, use the stress patterns internally and deliver the requested work product without exposing unnecessary pressure language.

## Workflow

1. Identify the task type.
Task types usually fall into writing, coding, analysis, planning, review, decision support, or research.

2. Choose the pressure mode.
Pick the dominant mode that best matches the failure risk:
- `competitive`: weak output loses against stronger alternatives
- `review`: reviewers will expose omissions and weak reasoning
- `elimination`: shallow work is rejected
- `accountability`: claims and recommendations must be defensible
- `performance`: output is treated as a visible measure of competence
- `adversarial`: an informed opponent will attack the answer

3. Add explicit quality bars.
Require the exact things that matter for the task, such as:
- factual correctness
- specificity
- edge-case coverage
- tradeoff handling
- line-level evidence
- executable steps
- concise structure

4. Add failure guards.
Typical guards:
- do not guess
- separate facts from assumptions
- surface uncertainty explicitly
- do not pad with generic advice
- do not skip edge cases
- do not hide tradeoffs

5. Set an exact deliverable format.
The output format should make the extra rigor usable, not just stricter.

6. Do one pressure check.
Before finalizing, verify that the rewritten prompt makes visible weaknesses easy to detect and hard to excuse.

## Output Pattern

Use this structure when rewriting prompts:

```text
[task]

[pressure sentence]

Produce the strongest version for this task.

Requirements:
- [criterion 1]
- [criterion 2]
- [criterion 3]

Do not:
- [failure guard 1]
- [failure guard 2]
- [failure guard 3]

If uncertainty remains, state it explicitly and proceed with the best supported answer.

Before finalizing, check that you:
- answered the actual request
- covered the important constraints
- separated facts from assumptions
- removed unsupported claims and filler
- fixed the part most likely to fail review

Output format:
[format]
```

## Reference Map

Read only the reference file you need:
- For ready-to-use English templates: [references/patterns.md](references/patterns.md)
- For ready-to-use Chinese templates: [references/zh-patterns.md](references/zh-patterns.md)

## Maintenance Rule

Keep `SKILL.md` as the operating guide only.
Put reusable prompt templates in `references/`.
When templates change, keep `agents/openai.yaml` aligned with the actual skill behavior and default invocation style.
