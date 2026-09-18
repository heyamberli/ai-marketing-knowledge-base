# Welcome to the AI Marketing Knowledge System Starter

Created by Amber Li.

This starter helps you turn scattered marketing context, evidence, decisions, and experience into knowledge that both people and AI agents can use.

You do not need to understand the full framework or complete every file before starting.

Start with one recurring marketing task.

## Start With an Agent

Open this repository in Codex, Claude Code, or another agent that can read and edit local Markdown files.

A repository cannot send the first chat message by itself, so type this short activation message:

```text
Start here.
```

The agent should read the repository instructions automatically and welcome you into the guided conversation. If your agent does not automatically load repository instructions, use the longer prompt in the README.

The agent should help you:

1. understand the task, scope, and intended outcome;
2. create a provisional `tasks/<task-slug>/task-context.md` without waiting for every field;
3. identify the minimum knowledge required;
4. research or propose what it can before asking you for more information;
5. distinguish observed, proposed, unknown, and judgment-dependent knowledge;
6. complete one useful piece of work so you have something concrete to review.
7. for recurring work, quietly maintain a run record so later work can be compared with the first baseline;
8. proactively show what knowledge was recorded and propose any meaningful candidate for your approval before it becomes durable guidance.

## What the Agent May Need to Clarify

The agent may clarify:

- What recurring marketing task or decision are you trying to improve?
- What would a useful outcome look like?
- Which audience, campaign, channel, market, or business unit is in scope?
- Which private sources it cannot inspect;
- Which consequential choices depend on your judgment;
- What actions require your approval.

It should research and propose answers wherever possible. It should not ask you to build source lists, taxonomies, or workflows from scratch before it begins helping.

## What Happens Next

Once the basic task is clear, the agent should create a provisional context and immediately run a first knowledge sprint across the relevant domains:

1. Business and offer
2. Customer and market
3. Brand and communication
4. Product and domain
5. Operating knowledge
6. Evidence and performance
7. Decisions and learning

Not every task needs all seven domains.

The objective is not to complete a knowledge base. It is to make the smallest useful set of knowledge available for a real marketing decision—and improve it as the work produces better evidence.

For a recurring task, the agent should also follow [`workflows/task-learning-loop.md`](workflows/task-learning-loop.md). You should not be asked to fill in an evaluation form. The agent records useful knowledge reuse and material corrections from the work itself, then brings any reusable learning to you for approval.

You should not have to ask whether the knowledge base changed. After meaningful work, the agent should provide a short knowledge handoff following [`workflows/knowledge-handoff.md`](workflows/knowledge-handoff.md), including the exact proposed destination and a clear choice to approve, narrow, test longer, or reject.

## Add Knowledge From a URL

You can give the agent an article, product page, report, or public website while describing the task. It should first use the page for orientation, then return to the onboarding conversation with better questions.

Once the task is sufficiently clear, you can request a structured ingest:

```text
Ingest this URL for my current task:
[URL]

Extract only knowledge relevant to the task. Separate source claims,
observable facts, cited evidence, interpretation, and unknowns. Show me the
proposed knowledge objects and save location before writing anything.
```

The agent should follow [`workflows/url-ingest.md`](workflows/url-ingest.md). A URL does not become trusted knowledge merely because it has been ingested.

## Prefer to Explore First?

- Read [`README.md`](README.md) for the complete model.
- Open [`examples/campaign-diagnosis/`](examples/campaign-diagnosis/) for a fictional end-to-end example.
- Review [`governance/`](governance/) for evidence, status, and approval rules.
