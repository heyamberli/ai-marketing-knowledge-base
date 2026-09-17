# Source and Evidence Policy

## Evidence States

| State | Meaning | Use |
| --- | --- | --- |
| Direct experience | A named owner personally did, saw, or decided it | State with appropriate scope and date |
| Verified fact | Supported by a current authoritative source or observable behavior | Retain the source and observation date |
| Company or founder claim | Supplied by the organization but not independently verified | Attribute explicitly |
| Interpretation | A plausible explanation of evidence | Label as judgment, not fact |
| Recommendation | A proposed action based on evidence | Include criteria and limitations |
| Unknown | Missing, inaccessible, or not checked | Keep unknown; do not replace with zero or inference |

## Confidence

- **High:** current direct evidence supports the statement and material contradiction is unlikely.
- **Medium:** credible evidence exists, but scope, recency, or corroboration is limited.
- **Low:** early signal, small sample, indirect source, or meaningful uncertainty.

Confidence does not turn an interpretation into a fact.

## Freshness

Recheck prices, features, product availability, leadership, policies, campaign state, and performance data when their age could change the decision.

## Minimum Source Record

```yaml
claim_or_input:
evidence_state:
source_title:
source_url_or_path:
source_owner:
published_or_observed_date:
accessed_date:
scope_or_limitations:
confidence:
```

