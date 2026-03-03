# Incident Postmortem

**Incident ID:** [INC-XXXX]
**Incident title:** [Short description of what broke]
**Date of incident:** [YYYY-MM-DD]
**Date of this review:** [YYYY-MM-DD]
**Severity:** [Critical / High / Medium / Low]
**Postmortem facilitator:** [Name]
**Document owner:** [Name]

---

## Incident summary

[2–4 sentences. What broke, when, how long, and what was the user impact? Write this for someone who wasn't on call.]

## Timeline

All times in [timezone, e.g. UTC].

| Time | Event |
|---|---|
| [HH:MM] | Incident first detected |
| [HH:MM] | Alert triggered / on-call notified |
| [HH:MM] | Incident acknowledged |
| [HH:MM] | [Key diagnostic or mitigation step] |
| [HH:MM] | Service restored |
| [HH:MM] | Incident closed |

**Total duration:** [X hours Y minutes]
**Time to detect:** [X minutes]
**Time to resolve (from detection):** [X hours Y minutes]

## Impact

- **Users affected:** [number or percentage]
- **Services affected:** [list]
- **Data loss:** [Yes / No — if yes, describe]
- **SLA breached:** [Yes / No — if yes, which SLA and by how much]

## Root cause

[What actually caused the incident? Go past symptoms to the underlying reason. Use "5 Whys" if helpful.]

**Contributing factors:**
- [Factor 1]
- [Factor 2]

## What went well

- [Thing that worked — detection, communication, tooling, etc.]
- [Thing that worked]

## What went poorly

- [Thing that slowed resolution or made it worse]
- [Thing that slowed resolution or made it worse]

## Action items

| # | Action | Owner | Due date | Status |
|---|---|---|---|---|
| 1 | [Specific action to prevent recurrence] | [Name] | [YYYY-MM-DD] | Open |
| 2 | [Specific action to improve detection] | [Name] | [YYYY-MM-DD] | Open |
| 3 | [Specific action to improve response] | [Name] | [YYYY-MM-DD] | Open |

## Communication log

| Time | Audience | Channel | Message summary |
|---|---|---|---|
| [HH:MM] | [Internal team / customers / leadership] | [Slack / email / status page] | [Brief summary] |

## Sign-off

| Name | Role | Date |
|---|---|---|
| [Name] | Incident manager | [YYYY-MM-DD] |
| [Name] | Service owner | [YYYY-MM-DD] |
