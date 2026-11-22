# research-blue-team

English | [中文](README.cn.md) · [Research Skillbox](https://github.com/windyvictor/research-skillbox)

A research blue team. It challenges the claims that decide your work — an idea, an experiment, a proof, a paper, a grant — and calibrates every objection by whether it would change a decision. It finds the strongest counterexample, not the longest list of complaints.

## Try it

> Our method changes both the neighbourhood graph and the solver. The combined model scores higher. Can we attribute the gain to the graph?

The comparison supports a gain for the combined model. To isolate the graph’s contribution, hold the solver, data split and tuning budget fixed and compare the two graphs. If the result depends on the solver, report that dependence.

Ask for a proof check, an experiment review or a grant rehearsal. For rehearsal, the skill asks one question and waits for your answer. For a written review, it gives the strongest supported objection, the evidence and the smallest check that could change the decision.

## Calibrated criticism

| Grade | Meaning | Allowed action |
|---|---|---|
| **A — confirmed, affects the conclusion** | In-material evidence changes a core claim | Narrow the claim, repair the proof, fix the control, withdraw a sentence |
| **B — needs verification** | A concrete doubt the material cannot settle | One low-cost check; never a revision demand |
| **C — optional strengthening** | Does not affect the conclusion | Folded or omitted; never written into paper limitations |

No more than three objections per round. Grades guide the review internally. Ask for explicit grades if needed. Format, numbering, figure fonts, and reference style are C or unreported. Intensity is graded by stake: light for reversible wording, medium (default) for designs and assumptions, heavy for irreversible decisions such as submission, funding, or a large experiment. Heavy mode still obeys the same cap and stop rules.

## Use it for

- Deciding whether a research idea is worth pursuing, and what would kill it early
- Checking whether an experiment can distinguish the hypothesis from its strongest alternative
- Locating the exact step where a paper's conclusion outruns its evidence
- Rehearsing a grant defence around the one dependency that decides funding
- Simulating a review round or a one-question-at-a-time defence practice

Triggers include "act as a blue team", "challenge my idea", "find a counterexample", "rehearse the review", and "does this experiment really show that". Translation, formatting, and language polishing follow the original task instead.

## Contents

- `SKILL.md`: triggers, five-step workflow, calibration rules, delivery format
- `references/calibration.md`: six failure modes, evidence contract, stake levels, stop conditions, known critic biases, eight self-check items, six regression cases
- `references/scenarios.md`: four research scenarios with worked examples
- `references/sources.md`: traceable methodological sources and their boundaries
- `agents/openai.yaml`: Codex entry metadata and default prompt

## Core rule

Only report objections that change a conclusion or a decision, and require evidence for each. Do not pad the count, do not turn a single counterexample into a rejection of the whole route, and do not decide or rewrite on the author's behalf. When the material supports the claim, say so and state what you checked.

## Install

```bash
git clone https://github.com/windyvictor/research-blue-team.git
mkdir -p ~/.agents/skills
ln -s "$PWD/research-blue-team" ~/.agents/skills/research-blue-team
```

Use the equivalent skills directory for your agent host. WorkBuddy reads `SKILL.md` from the skill directory; Codex uses `agents/openai.yaml`.

## Sources and license

MIT. The calibration rules adapt published work on LLM judges and critic models, peer-review guidance, and the premortem and Rapoport frameworks. All findings are restated for research work; external sources and their boundaries are listed in `references/sources.md`. Third-party quotations remain the property of their respective rights holders.
