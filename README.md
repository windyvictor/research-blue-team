# research-blue-team

English | [中文](README.cn.md) · [Research Skillbox](https://github.com/windyvictor/research-skillbox)

A research blue team. It challenges the claims that decide the work — an idea, an experiment, a proof, a paper, a grant — and calibrates every objection by whether it would change a decision. The aim is the strongest supported counterexample, not the longest list of complaints.

This repository is instructions for an agent. It has no checker script, test runner, or score. An objection is not a decision to abandon the route.

## Why this skill

A review goes wrong in two directions: it spends itself on wording, numbering, and figure fonts, or it treats one gap as a reason to reject the whole line of work. [SKILL.md](SKILL.md) keeps the review on the claim that would change the current decision. When the material supports that claim, the skill says so and states what it checked.

## What you get

The delivery depends on the decision, as specified in [SKILL.md](SKILL.md):

| The decision | First delivery |
|---|---|
| Whether a research idea is worth pursuing | The nearest known result or candidate baseline, what is actually new, and one early test that could decide whether to continue |
| Whether an experiment can test the core hypothesis | The control under which the original explanation and the strongest alternative predict different results, and how those results limit the claim |
| Whether a paper's conclusion holds, and how far it may be stated | A location in a sentence, theorem, proof step, table, or figure; a rebuttal, a repair, or a replacement sentence the evidence supports |
| Whether a proposal can carry a funding case | The scientific question that decides the case, the critical dependency in the route, prior evidence of feasibility, and a fallback that still answers part of the question |

For a written review, the reply states the judgment, the evidence, and the smallest next step that could change the judgment. For rehearsal, say so: the skill asks one question and waits. It does not enter a question-and-answer loop when you asked for a one-pass review or cannot reply between turns.

## When to use it, and when not to

Use it when you ask for a blue team, a counterexample, a review rehearsal, or a check that an experiment really shows the claim. The same applies to a group-meeting question, a reviewer follow-up, or a grant defence. Trigger phrases recorded in [SKILL.md](SKILL.md) include “act as a blue team”, “challenge my idea”, “find a counterexample”, “rehearse the review”, and “does this experiment really show that”.

Do not use it for these jobs:

- Translation, formatting, or language polishing. Those stay with the original task. For prose that keeps facts, uncertainty, citations, and the author's voice, use [academic-deai-writing](https://github.com/windyvictor/academic-deai-writing).
- Numbering, figure fonts, and reference style. [references/calibration.md](references/calibration.md) treats these as optional or unreported.
- Choosing the project for the author, rewriting the whole manuscript, or filing every possible reviewer question under limitations.
- Judging a full paper from the abstract alone. The judgment stays inside the abstract.
- Scoring a proposal, inferring a funder's hidden preference, or estimating a funding probability. With only the call title, the judgment stays at topic level.

If the material needed for the decision is missing, the skill asks for the smallest fragment and waits. It does not fill the gap with a guess.

## Positioning and boundaries

The stance in [SKILL.md](SKILL.md) is specific. A blue team is not an opposing camp and not a mutiny: it shares the scientific problem, may challenge the current route, and does not change the research goal. It first asks what evidence would move both sides.

These limits are rules, not tone:

- Report only objections that change a conclusion or a decision, and give evidence for each one.
- Do not pad the count. One round carries at most three independent objections.
- A counterexample must satisfy every premise and violate the conclusion. If it does, it answers that claim. It does not by itself close nearby claims or the whole route.
- A broken proof step means that proof needs repair. It does not, by itself, mean the theorem is false.
- If two factors change together, write both explanations before asking for a control that separates them.
- If the author's strongest reply holds, withdraw the objection. Do not reopen it from another angle to keep the list full.
- Do not treat “simple”, “obvious”, or “A+B” as a lack of novelty. Compare assumptions and conclusions item by item.
- A search hit on a nearby paper is not a finding that the claim has already been done, until the older result is shown to cover this claim.
- “Possible” and “not reported here” are not “refuted” or “the author did not do it”.

The design notes and their limits are in [references/sources.md](references/sources.md). They are reasons for the brakes above. They are not evidence that a stricter objection is automatically correct.

## One review round

[SKILL.md](SKILL.md) fixes five steps:

1. State the decision in one sentence. Keep the object, quantifiers, premises, and comparison. If only an abstract is available, say so.
2. Pick the objection most likely to change the decision and check what the material already lets you check.
3. Look in the text, appendix, or the author's reply for the strongest answer. Withdraw the objection if that answer holds. If it holds only in part, name the remainder.
4. Give the judgment, the evidence, and the next step. A settled point gets only the local change the evidence supports. Two live possibilities get one check, with what each result would change.
5. When new material arrives, name which step of the previous judgment it changes. Stop when the question is settled or there is no new evidence to inspect. Re-open the judgment when new evidence arrives, even after quiet rounds.

Stop without adding another item when any condition in [references/calibration.md](references/calibration.md) holds: the strongest reply succeeded, the decision can now be made, two rounds brought no new evidence or feasible check, the objections are repeating or flipping, or the round has hit its cap. The stop note states the conclusion, what was checked, and what was not. An unsettled disagreement stays one “needs verification” item.

## How strong an objection may be

Grades are an internal priority. The default reply is prose. Ask if you want the letters shown.

| Grade | Meaning | Allowed action |
|---|---|---|
| **A — confirmed, affects the conclusion** | Evidence in the material changes a core claim or what a reader understands by it | Narrow the claim, repair the proof, fix the control, or withdraw one sentence. Touch only that place. |
| **B — needs verification** | A concrete doubt the material cannot settle | One low-cost check, with what each result would support. Not a revision demand. |
| **C — optional strengthening** | Does not affect the conclusion | Fold into a clause, or omit. Do not write it into the limitations. |

`PASS_NO_CHANGE` is a valid outcome. If there is no A or B item, say that this round found no substantive problem, and list what was checked and what was not. Do not close with “one more comment”.

Six patterns in [references/calibration.md](references/calibration.md) are dropped or downgraded on sight: a side issue standing in for the claim, a template complaint that would fit a sound paper, padding or changing the subject, treating simplicity as a lack of novelty, writing a guess as a defect, and deciding or rewriting on the author's behalf. The same file has the evidence fields used before a comment is kept, eight pre-writing checks, and six regression cases for a person editing the skill. This repository does not ship a script that runs those cases.

## What to give it, and what it returns

Give the smallest packet that makes the decision checkable:

- The decision you are about to make.
- The claim, including its object, quantifiers, premises, and comparison.
- The material you actually have: abstract, selected section, proof step, experiment description, table, or proposal passage. Say if the rest is absent.
- Whether you want a written review or one question at a time.
- The stake, when it is not the default: reversible wording, a design choice, or an irreversible step such as submission, funding, or a large experiment.
- Any confidentiality or offline constraint.
- If you want a rewrite, say that the meaning and notation stay.

Do not paste unpublished theorem statements, project titles, review comments, data, or identifiable excerpts into a web search yourself if the skill is allowed to check public sources. The skill's own rule is to search with public titles, standard terms, and already public information.

A written reply has this shape:

| Part | What it contains |
|---|---|
| Decision and claim | One sentence. Abstract-only work stays inside the abstract. |
| Judgment | Supported, narrowed, needs a check, or no substantive problem this round. |
| Evidence | A locatable sentence, equation, table, calculation, or public source. |
| Next step | Grade A: one local change. Grade B: one check and what each result would mean. No substantive objection: the scope that was checked. |
| Count | At most three independent objections. Grade C usually does not appear. |

The internal check behind that prose is location, evidence, which conclusion moves, the smallest action, and confidence. Missing a locatable basis is a reason to drop the comment.

## Prompts you can paste

These are prompts, not recorded model answers. In Codex CLI or the IDE extension, the `$research-blue-team` prefix is an explicit mention. In the ChatGPT desktop app, [Build skills](https://learn.chatgpt.com/docs/build-skills) says to select a skill with `@`. The task text is the same either way.

The concrete cases below are the worked examples already written in [references/scenarios.md](references/scenarios.md). They are there to show which check is relevant. They are not measured results from this repository.

### Idea

```text
$research-blue-team
I want to use a new neighbourhood graph to recognise sparse clusters. Treat this as a blue-team review of the idea. Rewrite it as a claim a peer could refute. Name the nearest known result or candidate baseline, what would actually be new, and one early test that could decide whether to continue. If I have no results yet, do not decide go or no-go. A nearby paper counts against novelty only if you show that its result covers this claim.
```

[references/scenarios.md](references/scenarios.md) uses this case to separate a new edge weight from merely dropping cross-cluster edges: on synthetic data with controlled density and cluster separation, compare with a conventional graph matched on edge count, keep the downstream clustering method fixed, and record the cross-cluster edge ratio and the clustering error.

### Experiment

```text
$research-blue-team
The method changes both the neighbourhood graph and the solver, and the combined model scores higher. Check whether we can attribute the gain to the graph. State the original explanation and the strongest alternative. Give one comparison that can separate them, with the solver, data split, and tuning budget held fixed where they are compatible. Do not rewrite the combined gain as “the new graph improves accuracy” without that comparison.
```

The same reference says a broader graph explanation needs the new graph to improve under both solvers. A gain under only the new solver is a reason to inspect the interaction first. If one combination cannot run, name the effect that cannot be identified and narrow the claim.

### Proof

```text
$research-blue-team
I claim that a continuous, strictly decreasing objective that is bounded below must attain its minimum on the real line. Check this step. A counterexample has to satisfy every premise and violate the conclusion. If the counterexample only refutes “attains its minimum”, say how far the claim should be narrowed. If later steps need a minimiser, do not write the missing condition as something I have already proved.
```

The worked example in [references/scenarios.md](references/scenarios.md) is `exp(-x)`: the three premises hold, the infimum is zero, and the function stays positive. That rejects “attains its minimum”. It does not reject a claim that only needs the infimum to exist.

### Paper

```text
$research-blue-team
Here are the title, abstract, introduction sentences, and result paragraphs. Find the step where the conclusion outruns the evidence, and point to the sentence, theorem, table, or figure. If I only tested prespecified perturbations, a supported sentence is limited to the perturbations that were tested. Do not report formatting, numbering, figure fonts, or reference style. If I ask for a rewrite, keep the meaning and notation and change only the sentence the evidence supports.
```

### Grant

```text
$research-blue-team
This proposal extends a convergence result proved under strong convexity to a more general model. Rehearse the defence one question at a time, and wait for my answer. Start from the scientific question that carries the funding case. Ask where the original proof first uses strong convexity in an essential way, and whether the proposed condition restores the property that step was providing. Do not invent a score, a reviewer's preference, or a funding probability.
```

[references/scenarios.md](references/scenarios.md) says to leave a global linear rate as an open target when the preliminary result only supports convergence to a solution set, and to state which part of the original question a weaker fallback would still answer.

## Light, medium, and heavy stakes

The stake changes how deep the check goes. It does not raise the cap of three objections. All three levels still use the grades above. Heavy mode is not a licence to keep objecting without a stopping rule.

| Level | Use it for | What to inspect |
|---|---|---|
| Light | A reversible choice, such as one sentence in an abstract or the wording for a group meeting | The decisive facts, quantifiers, and scope |
| Medium, the default | Whether to add an experiment, or which technical route to take | The key assumption, the competing explanation, the strongest baseline, and the evidence chain |
| Heavy | An irreversible or high-consequence step: submission, a grant, a proposal defence, or a large experiment | Everything in the medium level, plus a failure rehearsal, pressure on the strongest argument, and a backup route |

In the heavy level, write down what evidence would stop the challenge before starting, and attack one point that could change the decision. [references/calibration.md](references/calibration.md) warns against assigned contrarianism: sustained denial without a deciding piece of evidence makes both sides more sure of the original judgment.

## Files

```text
research-blue-team/
├── SKILL.md                      # triggers, five-step review, delivery rules
├── README.md
├── README.cn.md
├── LICENSE
├── agents/
│   └── openai.yaml               # Codex display name, short description, default prompt
└── references/
    ├── calibration.md            # failure modes, grades, stakes, stops, biases, checks
    ├── scenarios.md              # four worked research situations
    └── sources.md                # methodological sources and their limits
```

There is no `scripts/`, `evals/`, or `tests/` directory. Nothing in this repository executes the review.

## Alongside other skills

These repositories are separate. This skill does not call them. Use another skill for the job it actually describes, then use this one for the decision-relevant challenge.

| Job | Use | What this skill still does |
|---|---|---|
| Read a paper and mark what was actually read | [paper-deep-reading](https://github.com/windyvictor/paper-deep-reading) | Challenge a claim only inside that source boundary |
| Build a proof, design, algorithm, or experiment | [research-copilot](https://github.com/windyvictor/research-copilot) | Challenge the claim that would change the decision. It does not replace the derivation or the experiment plan |
| Draft or revise a paper from traceable evidence | [writing-research-papers](https://github.com/windyvictor/writing-research-papers) | Locate where the conclusion outruns the evidence. A rewrite stays local and keeps the supported claim |
| Draft a grant argument against the current call | [grant-proposal-ai](https://github.com/windyvictor/grant-proposal-ai) | Challenge the dependency that decides the funding case. Compliance still follows that skill's current-call check |
| Remove template-like prose without changing the science | [academic-deai-writing](https://github.com/windyvictor/academic-deai-writing) | Leave wording, tone, and disclosure practice there |

A blue-team pass does not certify the other skill's output, and a polite or severe tone does not change the grade.

## Privacy and limits

[SKILL.md](SKILL.md) keeps the confidentiality requirement you set for unpublished papers, proposals, and data. It handles material only inside the current authorisation. Public checks use public titles, standard terms, and already public information. Offline means the supplied material only, with the missing external comparison stated as missing.

The limits in [references/sources.md](references/sources.md) and [references/calibration.md](references/calibration.md) are part of the result:

- The cited empirical work comes from LLM judging, code critique, and meta-science. Those tasks are not the same distribution as mathematics, optimisation, or machine-learning papers. The citations justify brakes, not a claim that a class of objection is always right or always wrong.
- The premortem and Rapoport's rules are thinking frames. This skill uses their checkable tests and stop rules. It does not claim that the posture itself makes criticism more effective.
- The reported link between demanding review and later citation is observational, and the sample is accepted papers. It is not a reason to expect a stricter review to raise the impact of a particular manuscript.
- For a real submission, the target venue's current reviewer guide remains the authority.

## Sources

The short descriptions below follow [references/sources.md](references/sources.md). That file states the boundary of each source. Third-party wording remains the property of its rights holders.

| Source | Role in this skill |
|---|---|
| 快刀青衣, reprinted as [同名转载](https://www.53ai.com/news/neirongchuangzuo/2025011019563.html) | Same goal, challenge the route rather than the research aim |
| 快刀青衣, [同名文章](https://www.53ai.com/news/neirongchuangzuo/2025060691523.html) | Rehearse before the meeting; leave room for the author to answer |
| Gary Klein, [Performing a Project Premortem](https://hbr.org/2007/09/performing-a-project-premortem), HBR, 2007 | Imagine failure in order to find a dependency worth testing. Do not write the imagined failure as a fact |
| Daniel Dennett, *Intuition Pumps and Other Tools for Thinking* (2013), Rapoport's rules | Restate the strongest reply before pressing the objection. Nitpicking is named as a failure |
| Jiang, Li, Wang, Fan, and Zeng, [arXiv:2604.14047](https://arxiv.org/abs/2604.14047) (2026); Nature, [d41586-026-01615-4](https://www.nature.com/articles/d41586-026-01615-4) | Put the weight on the core claim. Observational; accepted papers only |
| Zheng et al., [arXiv:2306.05685](https://arxiv.org/abs/2306.05685) | Position, verbosity, and self-enhancement biases. An LLM judge is not treated as neutral |
| McAleese et al., [arXiv:2407.00215](https://arxiv.org/abs/2407.00215); [OpenAI note](https://openai.com/index/finding-gpt4s-mistakes-with-gpt-4/) | Separate nitpicks and hallucinated bugs from objections that survive a check |
| Huang et al., [arXiv:2310.01798](https://arxiv.org/abs/2310.01798) | Do not withdraw or rewrite a correct step by thinking again with no new material |
| Michael J. Black, [Novelty in Science](https://perceiving-systems.blog/en/news/novelty-in-science) | Complexity is not novelty, and “A+B” is not by itself a rejection |
| [NeurIPS Paper Checklist](https://neurips.cc/public/guides/PaperChecklist) | A prompt to match claims, scope, assumptions, proofs, and experiment details. The target venue's current guide wins |
| [国家自然科学基金项目评审专家行为规范](https://www.nsfc.gov.cn/p1/2871/2874/2884/69612.html) | Used for a proposer's own check and defence rehearsal. The current call for that program is the authority |

## Install and invoke

The clone-and-symlink block is the install used by the other standalone skills, including [research-copilot](https://github.com/windyvictor/research-copilot), [writing-research-papers](https://github.com/windyvictor/writing-research-papers), and [paper-deep-reading](https://github.com/windyvictor/paper-deep-reading). The destination is the user skill location in the current Codex skill document, [Build skills](https://learn.chatgpt.com/docs/build-skills): `$HOME/.agents/skills`. That page also says Codex follows a symlink to the skill directory.

```bash
git clone https://github.com/windyvictor/research-blue-team.git
mkdir -p ~/.agents/skills
ln -s "$PWD/research-blue-team" ~/.agents/skills/research-blue-team
```

`mkdir` is only there so the documented directory exists before the link is created. For one repository, put this directory at `.agents/skills/research-blue-team` instead. Codex scans `.agents/skills` from the directory where you launch it up through the repository root. The same page says it does not merge two skills that share a `name`; both can appear.

The `name` in [SKILL.md](SKILL.md) is `research-blue-team`. [agents/openai.yaml](agents/openai.yaml) sets the Codex display name to “科研 AI 蓝军” and stores this default prompt:

```text
请用 $research-blue-team 检查这份研究材料最关键的主张，提出最强异议，说明依据和影响，给出能改变判断的最小验证；没有实质问题就直接说明。
```

From the same Codex document:

- In Codex CLI or the IDE extension, run `/skills` or type `$research-blue-team`.
- In the ChatGPT desktop app, type `@` and select the skill.
- This `agents/openai.yaml` does not set `policy.allow_implicit_invocation`. The documented default is `true`, so a prompt that matches the `description` in `SKILL.md` may select the skill without `$`. Explicit `$research-blue-team` still works. Setting the policy to `false` would turn implicit selection off; this repository does not set that.
- Codex detects a skill change on its own. If an install or an edit does not appear, restart Codex.
- To disable a skill without deleting it, that page shows a `[[skills.config]]` entry in `~/.codex/config.toml` with the `SKILL.md` path and `enabled = false`.

This install follows `$HOME/.agents/skills` as documented there. It does not install into the older `~/.codex/skills` directory. Another agent host should use its own skills directory. WorkBuddy reads `SKILL.md` from the skill directory.

## License

MIT. The copyright line is in [LICENSE](LICENSE). Third-party quotations remain the property of their rights holders.
