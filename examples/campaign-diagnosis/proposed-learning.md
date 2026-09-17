# Proposed Learning — Verifiable Success Should Gate Agent Authority

```yaml
proposed_date: YYYY-MM-DD
source_owner: campaign team
source_url_or_path: examples/campaign-diagnosis/task-context.md
scope: agents diagnosing or recommending changes to paid campaigns
confidence: medium
status: proposed
approved_by:
decision_date:
next_review: after two comparable campaign workflows
```

## Observed Traces

- The campaign's form-completion count increased while qualified-lead quality remained unclear.
- Without a written qualification definition, the agent initially treated all form completions as equivalent conversions.
- After the definition was supplied, the diagnosis shifted from volume optimization to segment and message quality.

## Candidate Pattern

If an agent cannot evaluate success against a checkable conversion definition, its permission level should remain limited to research, analysis, and drafting.

## Alternative Explanations

- The qualification definition itself may be wrong or incomplete.
- CRM delays or source-mapping errors may create an apparent quality problem.
- Different campaign objectives may require a graded score rather than a binary definition.

## Exceptions and Failure Cases

- Brand or exploratory work may not have an immediate conversion definition.
- A checkable metric can still incentivize the wrong behavior.
- Greater authority also requires evidence quality, privacy, budget, and brand checks.

## Proposed Application

Require the task context to contain a checkable success definition before an agent prepares campaign changes. If the definition is absent or cannot be applied to the relevant unit, restrict the output to questions, analysis, and drafts.

## Human Decision

- [ ] Approve as active guidance
- [ ] Narrow and approve
- [x] Test longer
- [ ] Reject

