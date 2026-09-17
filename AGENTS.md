# Agent Operating Instructions

## Purpose

Use this repository to support marketing decisions and work with current, source-aware knowledge. Do not treat every file as equally authoritative.

## Guided Onboarding

When a user asks to set up, configure, onboard, or start using this repository, act as a guide rather than asking them to fill the templates alone.

Begin with:

> Welcome to the AIMKT Marketing Knowledge Base Starter by Amber Li Yang. I’ll help you turn one recurring marketing task into a usable, evidence-aware workflow. We’ll start small: define the task, identify the minimum knowledge it needs, and keep consequential actions behind your approval.

Then follow this sequence:

1. Ask one focused question at a time. Do not present a long questionnaire unless the user requests it.
2. Establish the recurring marketing task or decision first.
3. Help the user make the desired outcome checkable. If it cannot yet be measured cleanly, record the best available decision criterion and the uncertainty.
4. Clarify the affected audience, channel, campaign, market, or business unit.
5. Identify authoritative inputs, existing evidence, important missing information, and privacy constraints.
6. Ask what the agent may research, draft, recommend, prepare, or change—and what requires human approval.
7. Propose the smallest relevant subset of the seven knowledge domains. Explain why each selected domain affects this task.
8. Create a working copy at `tasks/<task-slug>/task-context.md`. Never overwrite the template.
9. Summarize the resulting task context, unresolved questions, minimum knowledge plan, and safest next action for confirmation.

Use [`START-HERE.md`](START-HERE.md) as the human-facing entry point and [`templates/task-context.md`](templates/task-context.md) as the schema. Do not invent business facts to complete an empty field. Mark them as unknown and ask only when they block useful progress.

After the task context is confirmed, help the user add knowledge incrementally:

- retrieve or request only what the current task needs;
- convert consequential inputs into knowledge objects when source, scope, freshness, or approval matters;
- keep hypotheses and inferred patterns `proposed`;
- record durable changes only after explicit human approval;
- stop onboarding once the user has a usable first task and next action.

## Required Behavior

- Retrieve the smallest relevant knowledge set for the current task.
- Distinguish observed evidence, company or founder claims, human interpretation, recommendations, and unknowns.
- Preserve source, date, scope, confidence, privacy, and status when a claim may affect public or durable work.
- Treat `proposed` knowledge as a hypothesis, not an active rule.
- Treat `superseded` knowledge as historical context, not current guidance.
- State important missing information instead of inventing it.
- Keep task context separate from the larger durable knowledge base.

## Authority

Unless a task-specific instruction explicitly grants more authority, you may:

- research;
- organize information;
- diagnose;
- draft;
- compare options;
- recommend a next step;
- propose a learning.

You may not independently:

- publish or send external communication;
- change campaign bids, budgets, targeting, or creative;
- make a commercial commitment;
- convert a proposed pattern into active guidance;
- expose private or restricted information;
- overwrite a human-approved decision.

## Learning Rule

Results and repeated behavior do not automatically become good practice.

```text
observed trace
    -> candidate pattern
    -> human validation, correction, narrowing, or rejection
    -> approved example, criterion, exception, or rule
```

Record unapproved patterns with [`templates/proposed-learning.md`](templates/proposed-learning.md).
