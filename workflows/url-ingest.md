# Workflow — Ingest a URL Into Candidate Marketing Knowledge

Use this workflow when a user supplies a webpage, article, product page, report, or other URL and wants to make its relevant content usable in the knowledge base.

The purpose is not to summarize everything on the page. The purpose is to extract the smallest useful set of task-relevant, source-aware candidate knowledge.

## 1. Connect the Source to a Task

Confirm:

- the current task or decision the source should support;
- the question the user hopes the source will help answer;
- whether the user wants research context, product intelligence, evidence, an external framework, or another output;
- whether this single page is the full scope.

If the intended use is unclear, ask one focused question before processing the page.

## 2. Capture Source Metadata

Record:

- URL;
- page title;
- author or publisher, if available;
- source type;
- publication or last-updated date, if available;
- access date;
- whether the page is a primary source, secondary source, company claim, practitioner opinion, research report, documentation, or another evidence type.

## 3. Extract in Separate Layers

Keep these layers distinct:

### Source claims

What the author, company, or founder says is true.

### Observable facts

What can be directly confirmed from the page without accepting its interpretation.

### Cited evidence

The data, examples, methods, or external sources offered in support. Record whether the underlying evidence was inspected.

### Interpretation

What the material may mean for the current marketing task. Clearly label this as agent or human interpretation.

### Unknowns and limitations

What the page does not establish, what may be stale, and what needs independent verification.

## 4. Map to Relevant Knowledge Domains

Use only the domains that affect the current task:

1. Business and offer
2. Customer and market
3. Brand and communication
4. Product and domain
5. Operating knowledge
6. Evidence and performance
7. Decisions and learning

Explain why each selected domain is relevant. Do not create entries in all seven domains by default.

## 5. Check Before Saving

Compare the extraction with existing knowledge when available:

- Does it confirm, qualify, or contradict an active statement?
- Is it newer or more authoritative than the current source?
- Is the claim scoped to a particular market, audience, channel, product version, or time period?
- Is the source describing observed behavior or desired positioning?
- Could the source create a privacy, copyright, disclosure, or commercial conflict?

## 6. Present a Review Preview

Before writing files, show:

1. a short source summary;
2. the task relevance;
3. proposed domain mapping;
4. candidate knowledge objects;
5. conflicts, gaps, and verification needs;
6. the proposed save location and status.

Ask the user to approve, edit, reject, or request deeper verification.

## 7. Save the Approved Record

Use [`../templates/url-ingest-review.md`](../templates/url-ingest-review.md) and save to:

```text
tasks/<task-slug>/sources/YYYY-MM-DD-<source-slug>.md
```

Default status:

- source record: `raw`;
- inferred pattern or recommendation: `proposed`;
- independently unverified company or author claim: label by source type and keep out of active guidance.

## Suggested User Prompt

```text
Ingest this URL for my current task:
[URL]

Extract only knowledge relevant to the task. Separate source claims,
observable facts, cited evidence, interpretation, and unknowns. Show me the
proposed knowledge objects and save location before writing anything.
```

