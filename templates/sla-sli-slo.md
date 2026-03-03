# SLA / SLI / SLO One-Pager

**Service name:** [Name of the service or product]
**Service owner:** [Team or individual responsible]
**Customers / users:** [Who depends on this service]
**Document version:** 1.0
**Last reviewed:** [YYYY-MM-DD]

---

## Definitions

| Term | Meaning |
|---|---|
| **SLI** (Service Level Indicator) | A metric that measures actual service behaviour |
| **SLO** (Service Level Objective) | The target value or range you set for an SLI |
| **SLA** (Service Level Agreement) | A formal commitment (usually contractual) based on SLOs, with consequences for missing it |

---

## Service Level Indicators and Objectives

| SLI | What it measures | SLO target | Measurement window | Data source |
|---|---|---|---|---|
| Availability | % of time the service responds successfully | ≥ [99.9]% | Rolling 30 days | [Monitoring tool] |
| Latency (p95) | 95th percentile response time | ≤ [300] ms | Rolling 7 days | [APM tool] |
| Error rate | % of requests that return an error | ≤ [0.5]% | Rolling 7 days | [Log aggregator] |
| [Custom SLI] | [What it measures] | [Target] | [Window] | [Source] |

---

## Error budget

An error budget is how much failure you're allowed before you breach your SLO.

| SLO | Allowed downtime per month | Allowed downtime per week |
|---|---|---|
| 99.9% availability | ~43 minutes | ~10 minutes |
| 99.5% availability | ~3.6 hours | ~50 minutes |
| [Your SLO] | [Calculate: (1 − SLO%) × period] | |

**Error budget policy:**
- If > 50% of the monthly error budget is consumed, [action — e.g. pause non-critical releases]
- If 100% of the monthly error budget is consumed, [action — e.g. freeze releases, incident review required]

---

## Service Level Agreement

| Term | Detail |
|---|---|
| Parties | [Provider] and [Customer / team] |
| Effective date | [YYYY-MM-DD] |
| Review date | [YYYY-MM-DD] |
| Reporting frequency | [Monthly / quarterly] |
| Consequence of breach | [Credit / escalation / formal review] |
| Exclusions | Planned maintenance windows; force majeure events |

---

## Reporting and review

- **Dashboard:** [Link to monitoring dashboard]
- **Reports sent to:** [Names or distribution list]
- **Report frequency:** [Monthly]
- **Review meeting:** [Quarterly SLA review with stakeholders]

---

## Escalation

| Situation | Action | Contact |
|---|---|---|
| SLO breached for > [X] minutes | Page on-call | [PagerDuty / phone / Slack handle] |
| SLA breach confirmed | Notify service owner and customer | [Name / email] |
| Repeated breaches (3+ in a quarter) | Service review meeting | [Name / role] |
