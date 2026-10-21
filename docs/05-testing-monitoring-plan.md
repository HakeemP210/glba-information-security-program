# Testing & Monitoring Plan — 16 CFR §314.4(d)

[← Back to README](../README.md)

## Requirement

§314.4(d) requires the institution to regularly monitor and test the effectiveness of its safeguards. The rule gives two paths: continuous monitoring, or annual penetration testing plus vulnerability assessments at least every six months. Whichever path is chosen has to be documented, not just practiced informally.

## Approach

Without continuous monitoring infrastructure in place yet (tracked as its own entry in the risk register), the institution documented the following path as its current approach:

- **Annual penetration testing**
- **Vulnerability assessments** at least every six months

As the institution's logging and monitoring capabilities mature, the goal is to transition toward continuous monitoring to improve visibility into security events and identify potential threats more quickly.

### Scope

Testing scope is split by who actually controls the system:

- **In-scope for direct testing** — infrastructure the institution owns and controls outright (network devices, staff workstations). These get scanned and tested directly.
- **Out of scope for direct testing** — vendor-hosted, federally hosted, or state/accreditor-hosted systems. The institution has no authorization to scan or pen-test systems it doesn't own. Their security is instead evidenced through vendor assurance documentation, contractual safeguards clauses, or the hosting platform's own mandated security requirements, and tracked in the [asset inventory](02-asset-data-inventory.md) and [service provider oversight](07-service-provider-oversight.md) documentation instead.

### Cadence & responsibilities

![Testing cadence and responsibilities table](../images/testing-monitoring/testing-cadence-table.png)

All findings from the internal testing above feed back into the [risk register](03-risk-assessment-methodology.md) with an owner, target date, and status, the same as every other finding across the program.

## Why this matters

"We ran a scan once" isn't a testing program. A defined cadence with named responsibility is what turns testing from a one-time event into an ongoing control. Documenting the scope boundary (what's tested directly vs. relied on vendor/federal assurance for) also heads off the most common audit finding in this area: institutions either not testing anything, or testing systems they never had authorization to touch.

## Related

- [Safeguards Gap Analysis](04-safeguards-gap-analysis.md)
- [Service Provider Oversight](07-service-provider-oversight.md)
