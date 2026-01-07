# [[TITLE]]

## Executive summary
- Outcome: [[e.g., 40s → 3s (p95), -X% timeouts, -Y% DB CPU]]
- Why it mattered: [[user/business impact]]
- Scope: [[service/API endpoint + database + related components]]
- Timeframe: [[e.g., 2 days / 1 week]]
- Keywords: [[SQL, indexing, caching, AWS, Django, Stripe, etc.]]

---

## Context
System overview
- Workload: [[high traffic endpoint | batch job | internal tool]]
- Data: [[approx rows, growth, key entities (sanitized)]]
- Constraints: [[SLOs | no downtime | limited infra changes | release cadence]]

What “good” looks like
- Targets: [[p95 latency | error rate | cost | throughput]]

---

## Problem
- Symptom: [[what was observed in production]]
- Impact: [[who was affected and how]]
- Signals: [[p95 latency | error rate | timeouts | slow query log | alarms]]

---

## Investigation
What I checked
- [[slow query log | EXPLAIN | index coverage | join order | cardinality | locks | N+1 | caching]]
- [[application instrumentation | traces | logs]]

Root cause
- [[root cause bullet 1]]
- [[root cause bullet 2]]
- [[root cause bullet 3 (optional)]]

---

## Options considered
Option A: [[name]]
- Pros: [[...]]
- Cons: [[...]]
- Why not chosen: [[...]]

Option B: [[name]]
- Pros: [[...]]
- Cons: [[...]]
- Why chosen: [[...]]

---

## Decision
What changed (high level)
- [[query redesign | pivot/aggregation | reduce joins | new/adjusted indexes | denormalization | caching strategy]]
- [[schema change (if any)]]

Tradeoffs
- [[write amplification | storage cost | eventual consistency | complexity | operational risk]]

---

## Implementation notes (sanitized)
- [[2–6 bullets explaining “how”, without real identifiers]]
- Optional pseudo-SQL (only if safe): [[...]]
- Optional simplified diagram: [[link or description]]

---

## Verification
How I measured
- Before: [[baseline method]]
- After: [[same conditions, same dataset shape]]
- Guardrails: [[tests | regression checks | sampling | monitoring]]

Results
| Metric | Before | After | Delta |
|---|---:|---:|---:|
| [[p95 latency]] | [[...]] | [[...]] | [[...]] |
| [[error rate]] | [[...]] | [[...]] | [[...]] |
| [[DB CPU / load]] | [[...]] | [[...]] | [[...]] |

---

## Rollout and risk management
- Deployment approach: [[feature flag | gradual rollout | canary | scheduled window]]
- Monitoring: [[dashboards/alerts watched]]
- Rollback plan: [[what would trigger rollback + steps at high level]]

---

## Follow-ups
- [[next improvement 1]]
- [[next improvement 2]]
- Accepted debt: [[what you intentionally didn’t do]]

---

## Redactions
To protect confidentiality, I intentionally redacted:
- [[company/product names]]
- [[table/entity names and identifiers]]
- [[infra details: hosts, credentials, internal links]]
- [[customer data or business-sensitive metrics]]
