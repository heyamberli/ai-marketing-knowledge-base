# Working Tasks

This folder holds task-specific working context. It is intentionally separate from durable knowledge and governance.

For each recurring task, create:

```text
tasks/<task-slug>/task-context.md
tasks/<task-slug>/sources/
tasks/<task-slug>/runs/
```

Copy [`../templates/task-context.md`](../templates/task-context.md) rather than editing the template itself.

Add supporting notes only when they are required for the task. Do not treat task-specific assumptions or agent inferences as active organizational knowledge.

If the work reveals a reusable pattern, record it with [`../templates/proposed-learning.md`](../templates/proposed-learning.md) and keep it `proposed` until a human approves it.

For each meaningful execution of a recurring task, let the agent maintain a lightweight run record from [`../templates/task-run.md`](../templates/task-run.md). The record captures setup burden, material corrections, knowledge reuse, and results without asking the user to complete another form. Follow [`../workflows/task-learning-loop.md`](../workflows/task-learning-loop.md) when comparing runs.

When a URL supports the task, follow [`../workflows/url-ingest.md`](../workflows/url-ingest.md) and store the approved review under the task's `sources/` folder. Ingested material remains a source record or proposed knowledge until human review changes its status.
