# Workflow — First Knowledge Sprint

Run this workflow as soon as the task, scope, and intended outcome are clear enough to act. Do not wait for every onboarding question to be answered.

The goal is to replace abstract questioning with visible work the user can react to.

## 1. Create a Provisional Task Context

Create `tasks/<task-slug>/task-context.md` from the template.

Fill what is known. Label the rest:

- `provisional` when a reasonable working assumption is available;
- `unknown — researchable` when the agent can investigate it;
- `unknown — user judgment` only when it depends on private context or personal preference;
- `not required yet` when it does not block the first useful action.

Do not keep interviewing merely to eliminate blank fields.

## 2. Build the Minimum Knowledge Map

Select only the domains that materially affect the task. For each selected domain, show:

| Domain | What the task needs | Current state | Best available source | Next action |
| --- | --- | --- | --- | --- |
| Example | Specific decision-relevant knowledge | known / inferred / missing | URL, file, data, or human judgment | inspect / ingest / propose / ask |

The map is a working proposal, not homework for the user.

## 3. Do One Useful Piece of Work

Before asking another setup question, complete at least one available action, such as:

- inspect the supplied website or public page;
- review representative existing content;
- propose a starter source stack for a monitoring or research need;
- identify candidate performance inputs and what each can answer;
- draft a taxonomy, checklist, or workflow from available evidence;
- compare existing repository material with the task requirements.

If access to a private source is unavailable, specify what the source would contribute and continue with public evidence or a provisional structure.

## 4. Separate Results by State

Label the output clearly:

- **Observed:** directly supported by an inspected source.
- **Proposed:** a useful recommendation or structure awaiting user review.
- **Unknown:** information that remains unavailable.
- **Needs user judgment:** a consequential choice that cannot be researched externally.

Do not turn proposed material into active knowledge.

## 5. Hand Back Work, Not a Questionnaire

Return:

1. the provisional task context created;
2. the minimum knowledge map;
3. the useful work already completed;
4. the most important uncertainty;
5. one recommended next action;
6. a concise knowledge handoff following [`knowledge-handoff.md`](knowledge-handoff.md): what was recorded for the task, what may deserve durable retention, what remains provisional, and the exact approval requested.

Ask the user to react to the proposal. If a question is necessary, make it concrete and attach it to the artifact—for example, “I proposed these five sources for trend discovery; which would you remove?” rather than “Where do you find trends?”

## 6. Start the Learning Baseline

If this is recurring work, create the first run record from [`../templates/task-run.md`](../templates/task-run.md) and follow [`task-learning-loop.md`](task-learning-loop.md). Maintain it from the work already performed; do not ask the user to reconstruct the session or score the agent.
