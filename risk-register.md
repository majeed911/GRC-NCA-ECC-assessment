# Risk Register — TechNova Solutions

Risks derived from the [Gap Assessment](./gap-assessment.md), scored using a Likelihood × Impact matrix.

## Scoring Matrix

| | Low Impact | Medium Impact | High Impact |
|---|---|---|---|
| **High Likelihood** | Medium | High | **Critical** |
| **Medium Likelihood** | Low | Medium | High |
| **Low Likelihood** | Low | Low | Medium |

---

## Risk Register

| Risk ID | Risk Description | Related Control | Likelihood | Impact | Risk Level |
|---|---|---|---|---|---|
| R-01 | Account compromise due to absence of Multi-Factor Authentication (MFA) | 2-2-3-2 | High — no additional verification exists across any account | High — direct exposure of sensitive customer PII | **Critical** |
| R-02 | System compromise via direct remote access without VPN | 2-2-3-2 | High — all remote connections currently lack this control | Medium — most critical systems are otherwise confined to the internal network | **High** |
| R-03 | Failure to detect/contain security incidents due to absence of formal risk management | 1-5 | High — confirmed by an actual PII breach with no prior process in place | High — direct exposure of customer data and PDPL non-compliance risk | **Critical** |
| R-04 | Unauthorized access to unrelated systems due to weak Least Privilege enforcement | 2-2-3-3 | Medium — one confirmed case; not evidenced as a company-wide pattern | Medium — exposure of sensitive but non-customer-facing data | **Medium** |
| R-05 | Lack of accountability during security incidents due to undocumented roles/responsibilities | 1-4 | High — zero documentation means confusion is expected in nearly any incident | High — delayed response and blame-shifting during real incidents | **Critical** |
| R-06 | Weakened security oversight due to no dedicated, full-time cybersecurity manager | 1-2 | Medium — a person performs the role, but with divided attention | Medium — potential for delayed or flawed security decisions | **Medium** |
| R-07 | Operating under an outdated (2021–2022) cybersecurity strategy | 1-1 | High — near-certain that a 4–5 year old strategy misses current threats | High — real, uncovered vulnerabilities against modern attack techniques | **Critical** |
| R-08 | Confusion and delayed incident response due to mixed old/new procedures | 1-3 | Medium — surfaces specifically in incidents relying on outdated procedures | Medium — slows response but does not represent total response failure | **Medium** |
| R-09 | Undetected vulnerabilities and compliance gaps due to halted periodic audits | 1-8 | High — no audit for ~9 months with no mandated schedule in place | Medium — indirect impact; increases the chance other issues go undiscovered | **High** |
| R-10 | Misuse of former employees' accounts due to delayed deactivation | 2-2-3 | High — a month-long open window with no automated detection in place | High — includes a Finance department account, raising financial/data risk | **Critical** |

---

## Summary

| Risk Level | Count | Risk IDs |
|---|---|---|
| Critical | 5 | R-01, R-03, R-05, R-07, R-10 |
| High | 2 | R-02, R-09 |
| Medium | 3 | R-04, R-06, R-08 |

This distribution reflects a common pattern in growing organizations: risks tied to **directly exposed sensitive data or a complete absence of a control** (Critical) significantly outweigh risks tied to **partially implemented or purely procedural weaknesses** (Medium).

See [`remediation-plan.md`](./remediation-plan.md) for the corresponding corrective actions.
