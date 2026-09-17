# AIMKT Marketing Knowledge Base Starter

Created by Amber Li Yang.

A practical Markdown structure for turning marketing context, evidence, decisions, and human judgment into knowledge that people and AI agents can use.

New here? Start with [`START-HERE.md`](START-HERE.md) for agent-guided onboarding.

This starter is designed for marketers who already have documents, data, prompts, and campaign history but need a clearer way to answer:

- What does an agent need to understand before it works?
- Which source should it trust?
- What is current, proposed, or superseded?
- What may it analyze, draft, recommend, or change?
- How does feedback become reusable guidance without removing human judgment?

It is a starting structure, not a universal architecture or an autonomous marketing system.

## The Core Model

The knowledge base covers seven domains:

1. Business and offer
2. Customer and market
3. Brand and communication
4. Product and domain
5. Operating knowledge
6. Evidence and performance
7. Decisions and learning

Every domain may contain three knowledge states:

- **Explicit:** articulated and retrievable.
- **Tacit:** present in human experience but not adequately expressed.
- **Emerging:** a candidate pattern that has not yet been validated as durable guidance.

## Quick Start

### 1. Clone the starter

```bash
git clone https://github.com/heyamberli/ai-marketing-knowledge-base.git
cd ai-marketing-knowledge-base
```

You can use the folder directly in a Markdown editor or open it as an Obsidian vault.

### 2. Start with one real marketing task

Open [`templates/task-context.md`](templates/task-context.md) and define:

- the outcome and its checkable success definition;
- the audience, channel, campaign, or unit affected;
- the knowledge and evidence required;
- what the agent may research, draft, recommend, prepare, or change;
- the decisions that still require human approval.

Do not fill every knowledge domain before starting. Add only what the first task needs.

### 3. Use it with an agent

Open the cloned folder with an agent that can read local Markdown files, such as Codex or Claude Code. Start with:

```text
Read AGENTS.md, START-HERE.md, and README.md completely.

Guide me through setting up my first marketing task.
Ask one question at a time and do not assume missing business facts.
```

Before allowing the agent to read company files or systems, review their privacy, access, and sharing requirements.

### 4. See a completed example

Use [`examples/campaign-diagnosis/`](examples/campaign-diagnosis/) to see how a goal, a qualified-conversion definition, evidence, uncertainty, and agent permissions fit together.

### 5. Ingest a relevant URL

Once the task is defined, use [`workflows/url-ingest.md`](workflows/url-ingest.md) to turn a specified article, product page, report, or webpage into reviewable candidate knowledge. The workflow separates source claims, observable facts, cited evidence, interpretation, and unknowns before anything is saved.

## Start With One Task

Do not document everything first.

Choose one recurring marketing task, such as diagnosing campaign quality, briefing a content draft, evaluating a tool, or reviewing a landing page. Complete [`templates/task-context.md`](templates/task-context.md), then add only the knowledge required for that task.

Use the example in [`examples/campaign-diagnosis/`](examples/campaign-diagnosis/) to see how the pieces work together.

## Structure

```text
ai-marketing-knowledge-base/
├── AGENTS.md
├── CLAUDE.md
├── LICENSE.md
├── README.md
├── START-HERE.md
├── knowledge/
│   ├── 01-business-and-offer.md
│   ├── 02-customer-and-market.md
│   ├── 03-brand-and-communication.md
│   ├── 04-product-and-domain.md
│   ├── 05-operating-knowledge.md
│   ├── 06-evidence-and-performance.md
│   └── 07-decisions-and-learning.md
├── governance/
│   ├── source-and-evidence-policy.md
│   ├── approval-boundaries.md
│   └── knowledge-status.md
├── templates/
│   ├── knowledge-object.md
│   ├── decision-record.md
│   ├── proposed-learning.md
│   ├── experiment-record.md
│   ├── url-ingest-review.md
│   └── task-context.md
├── workflows/
│   └── url-ingest.md
├── tasks/
│   └── README.md
└── examples/
    └── campaign-diagnosis/
        ├── README.md
        ├── task-context.md
        └── proposed-learning.md
```

## How to Use It

1. Define the recurring task and its checkable outcome.
2. Fill only the relevant knowledge domains.
3. Record sources, dates, scope, confidence, and status for consequential claims.
4. Tell the agent what it may do and where human approval is required.
5. Run the task and record misunderstandings, corrections, and outcomes.
6. Save new patterns as proposed learning.
7. Promote a pattern into active guidance only after a human validates it.

## What This Starter Does Not Do

- It does not automatically make uploaded files accurate or current.
- It does not turn an AI inference into approved company knowledge.
- It does not give an agent authority to publish, spend, send, or change live systems.
- It does not replace task-specific data permissions, privacy review, or evaluation.
- It does not require every team to use all seven domains for every task.

## Tool Compatibility

The files are plain Markdown. They can be used as a normal folder, an Obsidian vault, or a version-controlled repository with an AI coding or knowledge agent that can read local files.

## Status

Version: v0.2

Publication: public

License: [CC BY 4.0](LICENSE.md)

## Attribution

Created by Amber Li Yang. If you reuse or adapt this starter, please use the attribution provided in [`LICENSE.md`](LICENSE.md).
