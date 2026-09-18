# Welcome to the AIMKT Marketing Knowledge Base Starter

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

1. define the task and desired outcome;
2. make success or the decision criterion checkable;
3. identify the minimum knowledge required;
4. distinguish evidence, assumptions, unknowns, and proposed learning;
5. set privacy and approval boundaries;
6. create `tasks/<task-slug>/task-context.md` for your review.

## What the Agent Will Ask About

The conversation will normally cover:

- What recurring marketing task or decision are you trying to improve?
- What would a useful outcome look like?
- Which audience, campaign, channel, market, or business unit is in scope?
- What evidence and authoritative sources already exist?
- What is still unknown or unreliable?
- What may the agent do, and which actions require your approval?

It should ask only the questions needed for your task, one at a time.

## What Happens Next

After you approve the task context, the agent will propose a minimum knowledge plan across the relevant domains:

1. Business and offer
2. Customer and market
3. Brand and communication
4. Product and domain
5. Operating knowledge
6. Evidence and performance
7. Decisions and learning

Not every task needs all seven domains.

The objective is not to complete a knowledge base. It is to make the smallest useful set of knowledge available for a real marketing decision—and improve it as the work produces better evidence.

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
