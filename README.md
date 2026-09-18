# AI Marketing Knowledge System Starter

Created by Amber Li.

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

Describe the task, its practical scope, and the outcome you want. The agent should create a provisional task context and then run [`workflows/knowledge-sprint.md`](workflows/knowledge-sprint.md).

It should not require you to complete every field before work begins. Missing information should be classified as researchable, safely provisional, dependent on user judgment, or unnecessary for the first action.

The working context may include:

- the outcome and its checkable success definition;
- the audience, channel, campaign, or unit affected;
- the knowledge and evidence required;
- what the agent may research, draft, recommend, prepare, or change;
- the decisions that still require human approval.

Do not fill every knowledge domain before starting. Add only what the first task needs, and expect the agent to research or propose what it can.

### 3. Use it with an agent

Open the cloned folder with an agent that can read local Markdown files, such as Codex or Claude Code. Start with:

```text
Start here.
```

Repository instructions cannot make an agent speak before the first user turn. This short message activates the guided onboarding. If the agent does not automatically load repository instructions, use:

```text
Read AGENTS.md, START-HERE.md, and README.md completely. Then guide me
through setting up my first marketing task. Ask one question at a time and
do not assume missing business facts.
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
├── CONTRIBUTING.md
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
│   ├── task-run.md
│   ├── url-ingest-review.md
│   └── task-context.md
├── workflows/
│   ├── knowledge-handoff.md
│   ├── knowledge-sprint.md
│   ├── task-learning-loop.md
│   └── url-ingest.md
├── tasks/
│   └── README.md
└── examples/
    └── campaign-diagnosis/
        ├── README.md
        ├── task-context.md
        ├── task-run-01.md
        └── proposed-learning.md
```

## How to Use It

1. Define the recurring task and its checkable outcome.
2. Fill only the relevant knowledge domains.
3. Record sources, dates, scope, confidence, and status for consequential claims.
4. Tell the agent what it may do and where human approval is required.
5. Let the agent maintain a lightweight run record while doing the task.
6. Compare later runs using setup burden, correction burden, useful knowledge reuse, and time to useful output.
7. Expect the agent to proactively show a knowledge handoff and propose meaningful candidates for retention.
8. Approve, narrow, test longer, or reject each durable-knowledge proposal.
9. Promote a candidate into active guidance only after a human validates it.

## How the System Gets Better

For recurring work, use [`workflows/task-learning-loop.md`](workflows/task-learning-loop.md). Each run gets a small agent-maintained record under `tasks/<task-slug>/runs/`.

The comparison keeps two kinds of evidence separate:

- **Work performance:** how quickly useful work appeared, how much setup and correction it required, and which prior knowledge was reused.
- **Business performance:** the task-specific result, such as impressions, clicks, qualified leads, or revenue.

A later run is not better merely because it produced a higher business metric, and a larger knowledge base is not proof of learning. Improvement should be visible in comparable work: fewer repeated explanations, fewer material corrections, faster useful output, or more accurate reuse of approved knowledge.

The first run establishes a baseline. Later comparable runs may be classified as `improved`, `mixed`, `unchanged`, `regressed`, or `insufficient evidence`. Candidate patterns remain proposed until a human approves them.

At every meaningful handoff, the agent should make knowledge changes visible: what was recorded for the task, what it recommends retaining more durably, what remains provisional, and which exact files would change. See [`workflows/knowledge-handoff.md`](workflows/knowledge-handoff.md). The user should not have to ask whether the knowledge base changed.

## What This Starter Does Not Do

- It does not automatically make uploaded files accurate or current.
- It does not turn an AI inference into approved company knowledge.
- It does not give an agent authority to publish, spend, send, or change live systems.
- It does not replace task-specific data permissions, privacy review, or evaluation.
- It does not require every team to use all seven domains for every task.

## Tool Compatibility

The files are plain Markdown. They can be used as a normal folder, an Obsidian vault, or a version-controlled repository with an AI coding or knowledge agent that can read local files.

## Feedback and Contributions

Feedback from real marketing tasks is welcome—especially confusing behavior, failure cases, material corrections, and examples of knowledge that did or did not help a later run.

Please use the GitHub Issue templates and remove private or identifying information before posting. Changes to the core framework are reviewed selectively while the model is evolving; substantial pull requests should begin with an Issue. See [`CONTRIBUTING.md`](CONTRIBUTING.md) for the current contribution policy.

## Status

Version: v0.5.3

Publication: public

License: [CC BY 4.0](LICENSE.md)

## Attribution

Created by Amber Li. If you reuse or adapt this starter, please use the attribution provided in [`LICENSE.md`](LICENSE.md).
