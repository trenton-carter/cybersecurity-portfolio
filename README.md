# Trenton Carter — Cybersecurity Portfolio

Cybersecurity professional focused on **Identity and Access Management (IAM)**,
**privileged access**, and **Active Directory security**. Current cloud-security
experience building least-privilege access controls across a 50+ account AWS
environment, plus hands-on hybrid-identity work across a 15-site clinical network
(Active Directory / Entra ID provisioning and MFA rollout). CompTIA Security+ and
AWS Certified Cloud Practitioner.

This portfolio centers on a three-part IAM project series covering the core
pillars of the field — privileged access, identity governance, and federation —
each built end-to-end on a self-hosted Active Directory lab and documented with
verification at every step.

💼 [LinkedIn](#) · 📧 trentonmcarter@gmail.com

---

## Featured Projects — Identity & Access Management

Three projects spanning the three pillars of IAM. Each is production-representative,
verified, and thoroughly documented.

### 🔐 [Tiered Privileged Access Lab](https://github.com/trenton-carter/tiered-pam-lab)
*Privileged Access Management*

A self-hosted PAM environment implementing the controls of an enterprise
privileged-access program — an open-source build of what CyberArk provides:

- **Credential vaulting & automated rotation** with HashiCorp Vault, rotating
  real Active Directory service-account passwords over LDAPS (static roles,
  check-out/check-in libraries, and root-credential rotation)
- **Session recording & brokered access** with Teleport — MFA-enforced,
  certificate-based, with full session replay
- **Tiered least-privilege administration** (Tier 0/1/2) with GPO deny-logon
  boundaries, proven with a live cross-tier logon denial
- **PKI**: AD CS enterprise CA for LDAPS, plus short-lived machine-identity
  certificates with ACME auto-renewal (step-ca)

### 📋 [AD Identity Governance Toolkit](https://github.com/trenton-carter/ad-governance-toolkit)
*Identity Governance & Administration (IGA)*

A PowerShell toolkit implementing core identity-governance controls against
Active Directory, with a Pester test suite:

- **Privileged access inventory** (nested-inclusive membership resolution)
- **Stale-account detection** (dormant, never-expiring, disabled accounts)
- **Segregation of Duties analysis** — detects toxic access combinations
- **Access-review certification reports** — consolidated, reviewer-facing
  attestation output
- Designed directory-agnostic with a documented Microsoft Graph / Entra
  extension path

### 🔑 [Keycloak SSO & AD Federation](https://github.com/trenton-carter/keycloak-ad-federation)
*Federation & Single Sign-On*

Keycloak stood up as an identity provider, federated to Active Directory over
LDAPS, demonstrating SSO across both dominant federation protocols:

- **AD federation over LDAPS** — domain users authenticated read-only against
  Active Directory
- **OIDC (OpenID Connect)** — full authorization-code flow
- **SAML 2.0** — IdP metadata with signing certificate and SSO/SLO endpoints
- **Single Sign-On** — one login, access across applications

---

## Competition Results

- **National Cyber League (NCL), Spring 2026** — ranked **156th of 7,010**
  nationally (individual game), a Wittenberg University school record.
- Detailed score reports in [`reports/`](reports/).

---

---

## Additional Projects

Earlier hands-on labs demonstrating PowerShell automation for security workflows:

- **[PowerShell Incident Response Data Collector](projects/PowerShell_Incident_Response_Data_Collector.pdf)** *(PowerShell, JSON, CSV)* — an `Invoke-IncidentResponse` script that snapshots host state during an incident: collects system information and running-process detail, exports structured JSON/CSV artifacts, and generates a human-readable triage summary. Demonstrates function design, file automation, and evidence preparation for IR workflows.

- **[PowerShell File Integrity Hash Calculator](projects/PowerShell_File_Integrity_Hash_Calculator.pdf)** *(PowerShell, MD5/SHA1/SHA256)* — a `Get-FileHashReport` script that recursively hashes all files in a directory across multiple algorithms, captures file metadata, handles errors gracefully, and exports a timestamped CSV for tamper detection and integrity verification.

*Additional network-analysis labs (ARP spoofing detection, Wireshark traffic analysis) are also available in [`projects/`](projects/).*

---

## Skills

**Identity & Access:** Active Directory · Entra ID / Azure AD · LDAP / LDAPS ·
MFA · privileged access management · identity governance · access reviews · SSO ·
OIDC / OAuth2 · SAML · federation · RBAC · least privilege · account lifecycle
(joiner-mover-leaver)

**Cloud Security:** AWS IAM Identity Center · Service Control Policies (SCPs) ·
Control Tower · multi-account governance · GuardDuty · Security Hub

**Tools & Platforms:** HashiCorp Vault · Teleport · Keycloak · AD CS / PKI ·
step-ca · Windows Server · Ubuntu Server

**Scripting & Automation:** PowerShell · Pester · Python · Bash · Git/GitHub ·
CI/CD

**Security Foundations:** threat modeling · least-privilege administration ·
network analysis · CTF (NCL)

---

## Certifications

- **CompTIA Security+**
- **AWS Certified Cloud Practitioner**
- *AWS Solutions Architect Associate (in progress)*

---

## Education

**Wittenberg University** — B.A. Computer Science, Cybersecurity concentration ·
Business minor
