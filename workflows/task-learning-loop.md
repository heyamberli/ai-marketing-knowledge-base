# Workflow — Task Learning Loop

Use this workflow for recurring marketing work. It creates a small evidence trail for one question:

> Did the system make this run more useful because of knowledge accumulated from earlier work?

The agent maintains the record. The user should not have to complete a scorecard before receiving useful work.

## 1. Open a Run Record

Create `tasks/<task-slug>/runs/YYYY-MM-DD-<run-name>.md` from [`../templates/task-run.md`](../templates/task-run.md).

Before substantial work, record only what is already available:

- the deliverable and intended outcome;
- the closest comparable previous run, if one exists;
- relevant active knowledge retrieved;
- important proposed knowledge used as a hypothesis;
- the start time when time-to-useful-output can be observed reliably.

If this is the first comparable run, mark it `baseline only`.

## 2. Do the Work

Do not interrupt execution to administer an evaluation survey. Capture evidence from the normal workflow:

- questions the agent had to ask before it could act;
- knowledge correctly reused without the user repeating it;
- factual, strategic, voice, scope, or approval corrections made by the user;
- recommendations the user accepted, changed, or rejected;
- missing knowledge that caused delay or rework;
- business results when they later become available.

Count only substantive items. A clarification about formatting is not equal to a correction of audience, positioning, or evidence.

## 3. Close the Run at Handoff

Update the record with the first useful output and the user's response when available.

Use four practical learning signals:

1. **Time to useful output** — elapsed time from an actionable request to the first output worth reviewing. Use `not measured` when timestamps are unreliable.
2. **Setup burden** — substantive questions the user had to answer before useful work began.
3. **Correction burden** — material corrections required to make the work usable. Record examples; do not rely only on a count.
4. **Knowledge reuse** — prior knowledge that materially improved the work without being restated by the user.

Also record the task-specific business result separately. Do not use impressions, clicks, leads, or revenue as proof that the system learned unless the causal link is supported.

## 4. Compare With the Closest Prior Run

Compare only sufficiently similar work: the same recurring job or a genuinely comparable deliverable, channel, audience, and scope.

Classify the comparison as:

- `improved` — evidence indicates lower effort or better work and no material quality regression;
- `mixed` — some signals improved and others worsened or remain unclear;
- `unchanged` — no meaningful difference is visible;
- `regressed` — the later run required more effort or produced worse work for knowledge-related reasons;
- `baseline only` — no valid comparison exists;
- `insufficient evidence` — the records are not reliable enough to judge.

Explain the classification in plain language. Never calculate a single “learning score” that hides tradeoffs.

## 5. Propose, Approve, and Reuse Learning

At the end of the run:

1. identify the most consequential correction, successful reuse, or unresolved gap;
2. decide whether it is task-specific history or a potentially reusable pattern;
3. if reusable, create a proposal from [`../templates/proposed-learning.md`](../templates/proposed-learning.md);
4. show the proposal to the user with its evidence and intended scope;
5. update active knowledge only after explicit approval;
6. in the next comparable run, retrieve the approved learning and record whether it actually helped.

One run can suggest a learning. Repetition or strong evidence is normally needed before treating it as durable guidance.
