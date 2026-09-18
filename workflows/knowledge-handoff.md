# Workflow — Knowledge Handoff

Use this workflow by default when a task, review, or substantive conversation produces knowledge that may improve future work.

The purpose is to make learning visible without allowing the agent to silently rewrite durable guidance.

## 1. Identify Meaningful Candidates

A candidate is worth surfacing when it is likely to affect a future decision or execution, such as:

- a user-confirmed business fact, audience, preference, or constraint;
- a decision and its rationale;
- a material correction, rejection, override, or exception;
- an evidence-backed observation with continuing relevance;
- a repeated or consequential pattern;
- a task-specific rule that should be retrieved in the next run.

Do not create a candidate for casual remarks, one-off formatting requests, unsupported guesses, duplicated knowledge, or details unlikely to matter again.

## 2. Classify the Destination

Recommend the smallest useful scope:

- **Task context or task history** — useful only for the current recurring job.
- **Proposed reusable knowledge** — may help across tasks but still needs testing, narrowing, or approval.
- **Active durable knowledge** — a user-confirmed fact, decision, example, criterion, exception, or rule the user explicitly approves for future use.

Task-scoped knowledge is still knowledge. Do not imply that only files under `knowledge/` count. At the same time, do not use the task folder to bypass approval for a cross-task rule.

## 3. Present the Proposal

At the end of meaningful work, include a concise `Knowledge handoff`:

```text
Knowledge handoff

Recorded for this task:
- [what was saved and where]

Proposed for durable knowledge:
- Statement:
- Why it matters:
- Scope:
- Evidence/source:
- Recommended status: proposed / active
- Destination:

Still provisional or unknown:
- ...

Decision requested:
Approve / narrow / test longer / reject
```

Show the exact file to be updated. When several candidates express one idea, combine them. Keep the handoff proportional to the work.

## 4. Apply the Human Decision

- **Approve:** write the approved statement to the proposed destination with source, date, scope, and status.
- **Narrow:** revise the statement or scope, confirm the narrowed form when consequential, then save it.
- **Test longer:** preserve it as `proposed` with the evidence needed and a concrete review trigger.
- **Reject:** record the rejection only when its rationale will prevent repeated re-proposal; otherwise leave durable knowledge unchanged.

Update the task run with the decision and files changed. Never represent silence as approval.

## 5. Retrieve It Later

In the next relevant task, retrieve the approved knowledge and note whether it helped. If later evidence conflicts with it, propose a revision or supersession instead of silently overwriting it.
