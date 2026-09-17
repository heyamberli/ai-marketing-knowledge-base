# AI Marketing Knowledge Base Starter

A practical Markdown structure for turning marketing context, evidence, decisions, and human judgment into knowledge that people and AI agents can use.

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

## Start With One Task

Do not document everything first.

Choose one recurring marketing task, such as diagnosing campaign quality, briefing a content draft, evaluating a tool, or reviewing a landing page. Complete [`templates/task-context.md`](templates/task-context.md), then add only the knowledge required for that task.

Use the example in [`examples/campaign-diagnosis/`](examples/campaign-diagnosis/) to see how the pieces work together.

## Structure

```text
ai-marketing-knowledge-base/
├── AGENTS.md
├── LICENSE.md
├── README.md
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
│   └── task-context.md
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

Version: v0.1  
Publication: prepared for public release  
License: [CC BY 4.0](LICENSE.md)

## Attribution

Created by Amber Li Yang. If you reuse or adapt this starter, please use the attribution provided in [`LICENSE.md`](LICENSE.md).
