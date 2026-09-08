# Gap Assessment — NCA ECC Compliance

**Organization:** TechNova Solutions (fictional SaaS company, 80 employees, hybrid work model)
**Framework:** NCA Essential Cybersecurity Controls (ECC)
**Domains Assessed:** Domain 1 (Cybersecurity Governance), Domain 2 — Control 2-2 (Identity and Access Management)

---

## Domain 1 — Cybersecurity Governance

| Control | Description | Status | Evidence | Gap |
|---|---|---|---|---|
| **1-1** Cybersecurity Strategy | A documented, approved cybersecurity strategy aligned with business objectives | Partially Compliant | Strategy document exists but dates from 2021–2022 and was never reviewed after the departure of the previous cybersecurity lead | Outdated strategy does not reflect current (2026) threats and technologies, leaving the organization operating on obsolete security assumptions |
| **1-2** Cybersecurity Management | A formally appointed function/person responsible for cybersecurity | Partially Compliant | No formal appointment exists; the same individual manages cybersecurity informally alongside another department | Dual role reduces time and focus dedicated to cybersecurity management, and the lack of formal appointment weakens accountability |
| **1-3** Cybersecurity Policies and Procedures | Documented and approved security policies and procedures | Partially Compliant | Some procedures updated in 2026, others still dated 2021; inconsistency discovered while handling a recent security incident | Delayed incident response due to conflicting old and new procedures, increasing potential damage before containment |
| **1-4** Cybersecurity Roles and Responsibilities | Formally documented roles and responsibilities for cybersecurity | Non-Compliant | No formal document exists; understanding of who is responsible for what is based entirely on verbal/informal communication | High likelihood of confusion and delayed response during any security incident, since there is no formal reference point |
| **1-5** Cybersecurity Risk Management | A formal, recurring process for identifying, assessing, and managing risk | Non-Compliant | A data breach on 08/15/2026 revealed there was no formal risk management process in place beforehand | Delayed detection of incidents and difficulty meeting the mandatory 72-hour breach notification window under PDPL, in addition to potential financial and reputational damage |
| **1-8** Periodical Cybersecurity Review and Audit | Regular review/audit of the organization's cybersecurity posture | Partially Compliant | A person is assigned to this role, but the last actual audit was conducted in December 2025; no audit records existed when requested at a mid-year board meeting | Lack of proactive vulnerability discovery, and difficulty demonstrating compliance to management or regulators |

---

## Domain 2 — Cybersecurity Defence: Control 2-2 (Identity and Access Management)

| Sub-Requirement | Description | Status | Evidence | Gap |
|---|---|---|---|---|
| **2-2-3** Account Management | Documented process for creating, modifying, and deactivating user accounts | Partially Compliant | New employee had to temporarily use a colleague's device while HR processed account creation; two employees (Finance, Marketing) who left on 07/08/2026 still had active accounts as of 07/09/2026 | A month-long window during which former employees' accounts remained active created a real risk of unauthorized access, especially given the Finance department account |
| **2-2-3-2** Multi-Factor Authentication (MFA) | MFA required for remote access and privileged accounts | Non-Compliant | Review of login configurations for email and the admin dashboard showed reliance on username and password only, with no additional verification | High likelihood of account compromise through credential guessing or leakage, particularly with sensitive customer PII (salary, ID data) at stake |
| **2-2-3-2** Remote Access Control | Secure, governed remote connectivity (e.g., VPN) for off-site access | Non-Compliant | Employees connect directly to company systems over the internet using only username and password; no VPN or additional access layer is in use | Elevated breach risk via credential leakage, due to the absence of a VPN layer that would otherwise restrict access to a trusted network |
| **2-2-3-3** Least Privilege | Users are granted the minimum access necessary for their role | Partially Compliant | Access is well-controlled in Finance and HR, but a review found a Marketing employee had access to executive management systems unrelated to their role | Increased attack surface — compromise of a single low-privilege account could expose unrelated, sensitive systems |
| **2-2-3-5** Periodic Access Review | Regular review of granted access rights | Non-Compliant | No record or process exists for reviewing access rights periodically or upon role change | Leads to privilege creep and duplicated access rights when employees change roles or leave the organization |

---

## Summary

| Status | Count |
|---|---|
| Compliant | 0 |
| Partially Compliant | 5 |
| Non-Compliant | 6 |

The assessment shows TechNova Solutions has informal or partial practices in most governance areas, but lacks formalization, documentation, and periodic review across nearly all controls in scope — a common pattern for growing SaaS organizations that have not yet invested in a dedicated GRC function.
