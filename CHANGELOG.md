# Changelog

[pdl]: https://psydata.net
[gh]: https://github.com/psydatalabsllc
[gl]: https://gitlab.com/psydatalabsllc

All notable changes to the **PsyData Labs L.L.C.** organization profile and master repository template are documented in this file.

The format is based on [Keep a Changelog v1.1.0](https://keepachangelog.com/en/1.1.0/), and this project adheres strictly to [Semantic Versioning v2.0.0](https://semver.org/spec/v2.0.0.html).

---

## [Unreleased]

### Planned
- Automated CI/CD compliance verification pipelines (`.gitlab-ci.yml`) for continuous SAST, secret detection, and SBOM generation.

---

## [0.1.0] - 2026-10-14T05:43:00.0870937Z

### Added
- **Root Repository Governance & Licensing:**
  - `LICENSE.md`: Established the formal **PsyData Labs L.L.C. Proprietary License (`PDL-LIC-001`)** with explicit Intellectual Property reservations and public viewing clauses.
  - `CODEOWNERS`: Enforced Zero-Trust sectional change control across executive leadership, core architects, security, compliance, and legal teams.
  - `VERSION`: Initialized baseline semantic version tracking (`0.1.0-alpha.1`).
  - `CHANGELOG.md`: Instituted standardized audit and release history tracking.
  - `.pre-commit-config.yaml`: Configured local DevSecOps pre-commit hooks enforcing private key blocking, file hygiene, Gitleaks cryptographic secret scanning, and Conventional Commits (`commit-msg`) validation.
- **Documentation & Governance Suite (`./docs/`):**
  - `docs/ACKNOWLEDGMENTS.md`: Added formal attributions, foundational recognitions, and ecosystem acknowledgments.
  - `docs/CODE_OF_CONDUCT.md`: Established the Corporate Code of Conduct & Professional Ethics Charter, reporting channels (`conduct@psydata.net`), and enforcement ladder.
  - `docs/CONTRIBUTING.md`: Defined contributor workflows, mandatory cryptographic commit signing (`GPG`/`SSH`/`X.509`), Developer Certificate of Origin (`DCO`) sign-offs, and Zero-PHI/PII guardrails.
  - `docs/EARLY-ACCESS-PROGRAM.md`: Documented the **PsyData Labs Early Access Program (EAP)** structure, benefits, NDA/security expectations, and onboarding channels.
  - `docs/FIVE-DOMAINS.md`: Detailed the architectural blueprint across our Five Foundational Domains (Software Native Ecosystems, Technology & Infrastructure, IAM & PKI, Compliance & AI Governance, and Secure Data Platforms).
  - `docs/GOVERNANCE.md`: Codified the Corporate, Security & AI Governance Charter mapping Day-One engineering controls to **SOC 2 Type II**, **ISO/IEC 27001**, **ISO/IEC 42001**, **GDPR & UK GDPR**, **HIPAA Safeguards**, and **NIST AI RMF**.
  - `docs/SECURITY.md`: Instituted the Coordinated Vulnerability Disclosure (CVD) policy, CVSS v4.0 response SLOs, encrypted reporting boundaries (`security@psydata.net`), and researcher Safe Harbor provisions.
  - `docs/SUPPORT.md`: Created the support routing matrix directing community, EAP, security, compliance, and enterprise inquiries across official channels.
- **GitLab Issue & Merge Request Automation (`./.gitlab/`):**
  - `.gitlab/issue_templates/Bug_Report.md`: Standardized reproducible defect reporting with mandatory Zero-PHI/PII sanitization checks and automated triage labeling.
  - `.gitlab/issue_templates/Feature_Proposal.md`: Created the Architectural RFC & Feature Proposal template aligned with the Five Domains and Six Premier Compliance Frameworks.
  - `.gitlab/merge_request_templates/Default.md`: Enforced pre-merge verification checklists for cryptographic commit provenance, secret scanning, test coverage, and documentation parity.
- **Brand & Visual Assets (`./assets/`):**
  - Added official **PsyData Labs L.L.C.** visual identity assets (`assets/PDL-NAME-WIDE.png`).

### Changed
- `README.md`: Refined the organization overview, updated Day-One Compliance badges and framework definitions, polished typography, and linked directly to `./docs/FIVE-DOMAINS.md`, `./docs/EARLY-ACCESS-PROGRAM.md`, and `./LICENSE.md`.
- `.gitignore`: Expanded master Zero-Trust ignore rules to strictly block cryptographic keys/certificates (`*.pem`, `*.key`, `*.p12`), regulated datasets (`*.parquet`, `*.csv`, `*.sqlite`), AI/ML model weights (`*.safetensors`, `*.onnx`, `*.gguf`), cloud state files, and local IDE artifacts (`.idea/`, `.vscode/`).

---

<small>
Copyright © 2026 PsyData Labs L.L.C. | All Rights Reserved (PDL-LIC-001)<br />
Website: <a href="https://psydata.net">https://psydata.net</a>
</small>

[Unreleased]: https://gitlab.com/psydatalabsllc/gitlab-profile/-/compare/v0.1.0-alpha.1...HEAD
[0.1.0-alpha.1]: https://gitlab.com/psydatalabsllc/gitlab-profile/-/tags/v0.1.0-alpha.1