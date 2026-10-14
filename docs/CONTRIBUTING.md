# Contributing Policy 

[pdl]: https://psydata.net
[gh]: https://github.com/psydatalabsllc
[gl]: https://gitlab.com/psydatalabsllc

Thank you for your interest in contributing to [PsyData Labs L.L.C.][pdl][^1]. Because we engineer foundational technology across zero-trust infrastructure, identity/PKI, and regulated AI and data ecosystems, **every contribution must** adhere to **strict security**, **cryptographic**, and **compliance standards** from day one.

This document outlines the mandatory protocols for submitting issues, merge/pull requests, and code or documentation changes across our [GitHub][gh] and [GitLab][gl] repositories[^2].

---

## 1. Zero-Trust & Compliance Gateways

All contributions are evaluated against our Six Premier Governance Standards (**SOC 2 Type II**, **ISO/IEC 27001**, **ISO/IEC 42001**, **GDPR & UK GDPR**, **HIPAA Safeguards**, and **NIST AI RMF**). 

### Mandatory Rules for All Contributors:
1. **Zero PHI/PII Policy:** Never include real Protected Health Information (PHI), Personally Identifiable Information (PII), production telemetry, or customer data in code, tests, comments, commit messages, or issue descriptions. Use exclusively synthetic, non-identifiable mock data.
2. **Zero Secrets in VCS:** Never commit API keys, X.509 private keys, certificates, `.env` files, internal IP topologies, or credentials. All commits must pass local `pre-commit` hooks (Gitleaks + PII scanners) before pushing.
3. **Cryptographic Commit Signing:** All commits **must** be cryptographically signed using a valid **GPG**, **SSH**, or **S/MIME (X.509)** key registered to your GitLab/GitHub identity (`git commit -S`). Unsigned commits will be automatically rejected by CI/CD branch protection gates.
4. **Developer Certificate of Origin (DCO):** Every commit must include a `Signed-off-by` trailer (`git commit -s`) certifying that you have the legal right to submit the contribution under the repository's license (`PDL-LIC-001` or specified open-source license).

## 2. Contribution Workflow

### Step 1: Pre-Flight Alignment
Before writing code for major features or architectural changes:
- Check existing **Issues** on [GitLab][gl] or [GitHub][gh] to avoid duplicate work.
- Open a **Proposal / RFC Issue** if your change impacts IAM/PKI, cryptographic primitives, data schemas, or AI governance pipelines.

### Step 2: Environment & Pre-Commit Setup
Clone the repository and initialize the mandatory security hooks:

```bash
git clone <repository-url>
cd <repository-name>
pre-commit install --install-hooks
pre-commit install --hook-type commit-msg
```

### Step 3: Branching Strategy

Create a descriptively named branch from the default integration branch (`main`):

* `feat/<domain>-<short-description>` (New capabilities)
* `fix/<domain>-<short-description>` (Bug patches)
* `sec/<domain>-<short-description>` (Non-embargoed security hardening)
* `docs/<domain>-<short-description>` (Documentation & compliance artifacts)
* `gov/<domain>-<short-description>` (ISO 42001 / NIST AI RMF / SOC 2 policy updates)

### Step 4: Conventional Commits

We strictly enforce the [Conventional Commits v1.0.0](https://www.conventionalcommits.org/) specification to automate semantic versioning and audit changelogs:

```text
<type>(<scope>): <concise summary in imperative mood>

[Optional body explaining architectural rationale, security impact, and compliance alignment]

Signed-off-by: Your Full Name <your.email@domain.com>
```

## 3. Merge Request (MR) / Pull Request (PR) Standards

Before requesting a review from `@psydatalabsllc/codeowners`:

* [ ] All automated CI/CD pipelines (SAST, DAST, dependency auditing, secret detection, and unit/integration suites) pass with zero high/critical findings.
* [ ] New functionality includes comprehensive unit and integration tests.
* [ ] Changes impacting AI models or datasets include updated **Model Cards** or **Data Sheets** aligned with ISO/IEC 42001 and NIST AI RMF.
* [ ] Documentation (`README.md`, `./docs/`, inline docstrings) is updated to reflect architectural changes.

## 4. Intellectual Property & Licensing

Unless explicitly stated otherwise in a repository-specific `LICENSE.md`, all contributions to PsyData Labs L.L.C. repositories are governed by **PDL-LIC-001** and our Corporate Contributor License Policy. By submitting a Merge Request or Pull Request, you agree that your contribution does not violate any third-party intellectual property rights.

---

![PsyData Labs L.L.C. Wide Logo](./assets/PDL-NAME-WIDE.png)

[^1]: PsyData Labs L.L.C. is an emerging applied systems company and hybrid intelligence lab. We are engineering zero-trust software ecosystems, infrastructure, identity, and providing AI governance and secure data services. PsyData Labs L.L.C. is also referred to as "PsyData Labs", "PsyData", "PDL", our as "us", "our", or the "Company". We encourage you to visit our [website][pdl], [GitHub][gh], and [GitLab][gl].

[^2]: Individuals may have to follow protocols outlined in this document within other repository or PDL platforms.

Read about our [Five Domains](./docs/FIVE-DOMAINS.md) - Read about our [Early Access Program](./docs/EARLY-ACCESS-PROGRAM.md) <br />

<small>
Copyright © 2026 PsyData Labs L.L.C.
All Rights Reserved (PDL-LIC-001)
Website: https://psydata.net/
</small>

See our [License](./LICENSE.md)

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