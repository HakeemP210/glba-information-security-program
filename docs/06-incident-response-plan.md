# Incident Response Plan — 16 CFR §314.4(h)

[← Back to README](../README.md)

## Requirement

§314.4(h) requires a written incident response plan covering seven specific elements: goals, an internal response process, defined roles/responsibilities/decision-making authority, an internal and external communications plan, remediation of identified weaknesses, documentation and reporting, and post-incident evaluation and revision of the plan itself.

## Approach

### Five-phase internal response process

```
1. Detect & Report → 2. Assess & Contain → 3. Eradicate → 4. Recover → 5. Post-Incident Review
```

Every phase has a named owner and a plain description of what actually happens in it. Staff are trained (see [Security Awareness Training](08-security-awareness-training.md)) to report anything suspicious immediately rather than attempt to resolve it themselves. The Qualified Individual leads assessment, containment, and eradication with standing authority to take immediate technical action (disabling accounts, isolating devices) without needing prior sign-off when it's needed to limit harm.

### Roles & decision authority

| Role | Responsibility |
|---|---|
| All staff | Report any suspected event immediately. They are not expected to resolve anything on their own |
| Qualified Individual | Leads response: assesses severity, directs containment/eradication, has standing authority for immediate technical action |
| Ownership/Director | Notified of any confirmed event; makes decisions requiring executive authority including: external communications, legal counsel, law enforcement, material financial/operational decisions |

### Communications

Internal: the QI notifies ownership as soon as a suspected event is confirmed as an incident, with status updates through resolution.

External notification obligations are genuinely layered for a Title IV institution and worth documenting explicitly rather than leaving implicit:

- **State breach notification law** — triggered if sensitive personal information is compromised, with a "without unreasonable delay" standard and a hard deadline (and Attorney General notification) once the number of affected state residents crosses a statutory threshold
- **U.S. Department of Education** — Title IV participants are required to report cybersecurity incidents affecting Title IV data through Federal Student Aid's incident reporting channel
- **Affected service providers** — if the incident involves systems or data they hold on the institution's behalf
- **Law enforcement** — if criminal activity is suspected

![Five-phase incident response process table](../images/incident-response/five-phase-diagram.png)

### Remediation, documentation, and revision

Every control weakness identified during or after an incident gets logged into the same [risk register](03-risk-assessment-methodology.md) used everywhere else in the program, with an owner, target date, and status. A blank incident log template is attached to the plan so any staff member reporting an event fills in the same structured fields every time.

The plan itself gets reviewed within 15 business days of any incident's resolution, and at least annually independent of whether an incident occurred.

![Blank incident log template](../images/incident-response/incident-log-template.png)

### It's been tested once, for real

This isn't hypothetical. A third-party servicer deployed a new report-export feature that, due to a defect on their end, briefly let staff at other institutions download reports containing a small number of our students' financial aid data (name, ID number, SSN, award year, disbursement amount) before the servicer caught and fixed it on their own side.

The incident was reported to the U.S. Department of Education's Federal Student Aid Cybersecurity Team at `FSASchoolCyberSafety@ed.gov`. It was logged using the same incident log template referenced above.

![Completed incident log for this event, with identifying fields redacted](../images/incident-response/completed-incident-log.png)

## Why this matters

A plan that only exists on paper fails the first time it's actually needed. Naming who has authority to act *before* an incident (not during one), pre-confirming the actual reporting channels and deadlines, and routing every finding back into the same risk register the rest of the program uses is what makes an incident response plan operational instead of decorative.

## Related

- [Risk Assessment Methodology](03-risk-assessment-methodology.md)
- [Security Awareness Training](08-security-awareness-training.md)
- [Program Review & Adjustment](09-program-review-adjustment.md)
