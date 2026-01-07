# <TITLE>

## Executive summary
- **Outcome:** <e.g., 40s → 3s (p95), -X% timeouts, -Y% DB CPU>
- **Why it mattered:** <user/business impact>
- **Scope:** <service/API endpoint + database + any related components>
- **Timeframe:** <e.g., 2 days / 1 week>
- **Keywords:** <SQL, indexing, caching, AWS, Django, Stripe, etc.>

---

## Context
**System overview**
- **Workload:** <high traffic endpoint / batch job / internal tool>
- **Data:** <~rows, growth, key tables (sanitized)>
- **Constraints:** <latency SLO, release cadence, no downtime, limited infra changes, etc.>

**What “good” looks like**
- <target latency / reliability / cost>

---

## Problem
- **Symptom:** <what was observed in production>
- **Impact:** <who was affected and how>
- **Signals:** <p95 latency, error rate, timeouts, slow query log, alarms>

---

## Investigation
**What I checked**
- <slow query log / EXPLAIN / index coverage / join order / cardinality / locks / N+1 / caching>
- <application-level instrumentation / traces / logs>

**Root cause**
- <1–3 bullets explaining the actual cause, in plain language>

---

## Options considered
### Option A — <name>
- **Pros:** <...>
- **Cons:** <...>
- **Why not chosen:** <...>

### Option B — <name>
- **Pros:** <...>
- **Cons:** <...>
- **Why chosen:** <...>

---

## Decision
**What changed (high level)**
- <query redesign / pivot/aggregation / reduce joins / new index / denormalization / caching strategy>
- <any schema changes, if applicable>

**Tradeoffs**
- <write amplification / storage cost / eventual consistency / complexity>

---

## Implementation notes (sanitized)
- <2–6 bullets with “how”, without exposing code or real identifiers>
- <include pseudo-SQL or simplified examples only if safe>

---

## Verification
**How I measured**
- **Before:** <how baseline was captured>
- **After:** <same conditions, same dataset shape>
- **Guardrails:** <tests, regression checks, sampling, monitoring>

**Results**
- <table or bullets with before/after metrics>

---

## Rollout and risk management
- **Deployment approach:** <feature flag / gradual rollout / canary / backout plan>
- **Monitoring:** <what dashboards/alerts were watched>
- **Rollback plan:** <what would trigger rollback>

---

## Follow-ups
- <what you'd do next if you had more time>
- <debt you intentionally accepted>

---

## Redactions
To protect confidentiality, I intentionally redacted:
- <company/product names>
- <table names / identifiers / customer data>
- <infra details (hosts, credentials, internal links)>
