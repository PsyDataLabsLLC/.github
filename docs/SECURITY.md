# Security Policy & Coordinated Vulnerability Disclosure

![Zero Trust](https://img.shields.io/badge/Zero%20Trust-Architecture%20Enforced-teal?style=for-the-badge)
![Security First](https://img.shields.io/badge/Security-First-B60205?style=for-the-badge)

[pdl]: https://psydata.net
[gh]: https://github.com/psydatalabsllc
[gl]: https://gitlab.com/psydatalabsllc

[PsyData Labs L.L.C.][pdl][^1]

Security, cryptographic integrity, and privacy engineering form the bedrock of **[PsyData Labs L.L.C.][pdl][^1]**. Every repository, service, and infrastructure node is architected to satisfy **SOC 2 Type II**, **ISO/IEC 27001**, **ISO/IEC 42001**, **GDPR/UK GDPR**, **HIPAA**, and **NIST AI RMF** safeguards.

---

## Reporting a Vulnerability

> [!CAUTION]
> **Never report security vulnerabilities, cryptographic weaknesses, IAM bypasses, or secret exposures via public GitLab/GitHub Issues, Merge/Pull Requests, or public Discord channels.**

If you discover a security vulnerability across any PsyData Labs L.L.C. domains (`psydata.net`, `psydata.org`, `psydata.us`, `psydata.dev`, `psydata.tech`), software repository, or Early Access Program environment, please report it immediately via our encrypted disclosure channels:

* **Primary Security Inbox:** [security@psydata.org](mailto:security@psydata.org)
* **GitHub Private Vulnerability Reporting:** Use the **"Report a vulnerability"** tab under the repository's `Security` section on [GitHub][gh].
* **GitLab Confidential Issues:** If submitting via [GitLab][gl], you **must** check `"This issue is confidential"` and assign the `[SECURITY-EMBARGO]` label.

### Required Disclosure Telemetry
To accelerate triage and remediation, please include:
1. **Affected Component & Domain:** Repository name, commit SHA/version tag, or web domain/endpoint.
2. **Vulnerability Classification:** CWE identifier, OWASP category, or MITRE ATLAS classification (for AI/ML adversarial vulnerabilities).
3. **Minimal Proof of Concept (PoC):** Step-by-step reproduction instructions, configuration states, and non-destructive exploit payloads.
4. **Impact Assessment:** Potential impact on Confidentiality, Integrity, or Availability (CIA triad) or regulatory compliance posture.

## Service Level Objectives (SLOs) for Response

PsyData Labs L.L.C. adheres to strict incident response timelines aligned with ISO/IEC 27001 and SOC 2 criteria:

| Severity Tier (CVSS v4.0) | Initial Acknowledgment | Triage & Validation | Target Remediation / Patch |
| :--- | :--- | :--- | :--- |
| **Critical (9.0 – 10.0)** | $\le 12\text{ Hours}$ | $\le 24\text{ Hours}$ | $\le 72\text{ Hours}$ |
| **High (7.0 – 8.9)** | $\le 24\text{ Hours}$ | $\le 72\text{ Hours}$ | $\le 7\text{ Days}$ |
| **Medium (4.0 – 6.9)** | $\le 48\text{ Hours}$ | $\le 5\text{ Business Days}$ | $\le 30\text{ Days}$ |
| **Low (0.1 – 3.9)** | $\le 5\text{ Business Days}$ | $\le 10\text{ Business Days}$ | Next Scheduled Release |

## Rules of Engagement & Safe Harbor

PsyData Labs L.L.C. extends **Legal Safe Harbor** to good-faith security researchers who adhere to the following boundaries:
- **Zero Data Exfiltration:** Do not access, download, modify, or destroy data belonging to other users or Early Access Program tenants. If you encounter PII/PHI or cryptographic keys, halt testing immediately and report the finding.
- **No Denial of Service (DoS):** Do not execute volumetric network floods, resource exhaustion attacks, or automated brute-force spraying against production or staging nodes.
- **No Social Engineering:** Phishing, vishing, or physical intrusion attempts against PDL personnel or data centers are strictly out of scope.
- **Coordinated Embargo:** Maintain strict confidentiality regarding the vulnerability until PDL has released a verified patch and mutually agreed upon a public disclosure window (typically 90 days post-remediation).

---

![PsyData Labs L.L.C. Wide Logo](/assets/PDL-NAME-WIDE.png)

[^1]: PsyData Labs L.L.C. is an emerging applied systems company and hybrid intelligence lab. We are engineering zero-trust software ecosystems, infrastructure, identity, and providing AI governance and secure data services. PsyData Labs L.L.C. is also referred to as "PsyData Labs", "PsyData", "PDL", our as "us", "our", or the "Company". We encourage you to visit our [website][pdl], [GitHub][gh], and [GitLab][gl].

<small>
Copyright © 2026 PsyData Labs L.L.C.
All Rights Reserved (PDL-LIC-001)
Website: https://psydata.net/
</small>

See our [License](./LICENSE.md)

[discord]: https://discord.gg/DzKmYWrNpD

<!-- 

Website: https://psydata.net
GitHub: https://github.com/psydatalabsllc
GitLab: https://gitlab.com/psydatalabsllc

Discord Invite (raw): https://discord.gg/DzKmYWrNpD
Discord Invite (PDL): https://discord.psydata.net/


PsyData Labs L.L.C. is an emerging applied systems company and hybrid intelligence lab. We are engineering zero-trust software ecosystems, infrastructure, identity, and providing AI governance and secure data services. PsyData Labs L.L.C. is also referred to as "PsyData Labs", "PsyData", "PDL", our as "us", "our", or the "Company". We encourage you to visit our [website][pdl], [GitHub][gh], and [GitLab][gl].

Copyright © 2026 PsyData Labs L.L.C.
All Rights Reserved (PDL-LIC-001)
Website: https://psydata.net

-->