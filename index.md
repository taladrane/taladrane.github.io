A best-effort collection of open source references related to vulnerability reporting, disclosure, and coordination. This page is intended to serve the community — maintainers, security researchers, and anyone involved in making software safer. Contributions and suggestions are welcome.

---

## Table of Contents

1. [Understanding Coordinated Vulnerability Disclosure](#understanding-coordinated-vulnerability-disclosure)
2. [Guidance for Maintainers](#guidance-for-maintainers)
3. [Guidance for Security Researchers & Finders](#guidance-for-security-researchers--finders)
4. [GitHub Platform Tools & Configuration](#github-platform-tools--configuration)
5. [Standards & Frameworks](#standards--frameworks)
6. [Vulnerability Identification & Tracking](#vulnerability-identification--tracking)

---

## Understanding Coordinated Vulnerability Disclosure

**Themes to explore:**
- *What is coordinated vulnerability disclosure (CVD) and how does it differ from full or no disclosure?*
- *Why does CVD matter for open source software specifically?*
- *What cultural barriers exist around CVD, and how can we overcome them?*
- *What does a healthy disclosure culture look like in a project or organization?*

| Resource | Description | Why Reference It |
|---|---|---|
| [**About Coordinated Disclosure of Security Vulnerabilities**](https://docs.github.com/code-security/concepts/vulnerability-reporting-and-management/about-coordinated-disclosure-of-security-vulnerabilities) (GitHub Docs) | GitHub's overview of the principles and rationale behind coordinated vulnerability disclosure. | A concise starting point for understanding what CVD is and why it matters. |
| [**Coordinated Vulnerability Disclosure (CVD) for Open Source Projects**](https://github.blog/security/vulnerability-research/coordinated-vulnerability-disclosure-cvd-open-source-projects/) (GitHub Blog) | A blog post discussing CVD practices tailored to the realities of open source development. | Provides practical context for why CVD in OSS is different from CVD in commercial software. |
| [**Removing the Stigma of a CVE**](https://github.blog/security/vulnerability-research/removing-the-stigma-of-a-cve/) (GitHub Blog) | Reframes CVEs as a normal, healthy part of software development rather than something to fear. | Helps maintainers and organizations adopt a positive mindset around vulnerability disclosure. |

---

## Guidance for Maintainers

**Themes to explore:**
- *How do I set up my project to receive vulnerability reports?*
- *What should a SECURITY.md or security policy include?*
- *How do I build a vulnerability management team (VMT)?*
- *How do I triage a report and decide if something is a vulnerability?*
- *What is an embargo period and how do I negotiate one?*
- *How do I develop and release a patch privately?*
- *How do I handle a report when I'm the only maintainer?*
- *What do I do if a vulnerability is disclosed publicly before I can fix it?*

| Resource | Description | Why Reference It |
|---|---|---|
| [**Guide to Implementing a CVD Process for Open Source Projects**](https://github.com/ossf/oss-vulnerability-guide/blob/main/maintainer-guide.md) (OpenSSF) | A comprehensive guide covering VMT creation, intake methods, private patch development, embargo lists, and the full response lifecycle. | The most complete open source playbook for maintainers — from preparation through disclosure. |

---

## Guidance for Security Researchers & Finders

**Themes to explore:**
- *I found a vulnerability — what do I do first?*
- *How do I find the right contact or security policy for a project?*
- *What information should I include in a vulnerability report?*
- *What are reasonable expectations for response timelines?*
- *How do I handle a situation where a maintainer is unresponsive?*
- *What is a CVE and how do I request one as a researcher?*
- *What are my options if the maintainer disagrees with my assessment?*
- *Can I publish my findings, and when is it appropriate to do so?*

| Resource | Description | Why Reference It |
|---|---|---|
| [**Guidance for Security Researchers to Coordinate Vulnerability Disclosures with OSS Projects**](https://github.com/ossf/oss-vulnerability-guide/blob/main/finder-guide.md) (OpenSSF) | Covers researcher motivations, how to write effective reports, disclosure options, obtaining CVE IDs, and troubleshooting unresponsive maintainers. | The definitive open source guide from the finder's perspective — including expectations-setting and templates. |

---

## GitHub Platform Tools & Configuration

**Themes to explore:**
- *How do I enable private vulnerability reporting on my repository?*
- *What are GitHub Security Advisories and how do they work?*
- *How can I use GitHub to privately develop and test a security patch?*
- *How do I publish a security advisory and notify users?*
- *What is the relationship between GHSA IDs and CVE IDs?*

| Resource | Description | Why Reference It |
|---|---|---|
| [**About Repository Security Advisories**](https://docs.github.com/code-security/concepts/vulnerability-reporting-and-management/about-repository-security-advisories) (GitHub Docs) | Explains GitHub Security Advisories — how maintainers can privately discuss, fix, and publish vulnerability information. | Essential reading for any GitHub-hosted project managing security issues. |
| [**Configuring Private Vulnerability Reporting for a Repository**](https://docs.github.com/code-security/how-tos/report-and-fix-vulnerabilities/configure-vulnerability-reporting/configuring-private-vulnerability-reporting-for-a-repository) (GitHub Docs) | Step-by-step instructions for enabling private vulnerability reporting on GitHub repositories. | The how-to guide for turning on the intake mechanism recommended by both GitHub and OpenSSF. |

---

## Standards & Frameworks

**Themes to explore:**
- *What standards exist for vulnerability disclosure and handling?*
- *How do I build or mature an incident response team (CSIRT or PSIRT)?*
- *What does a formal vulnerability handling process look like?*
- *How do government and international guidelines apply to open source?*
- *What is the relationship between ISO 29147, ISO 30111, and NIST guidance?*

| Resource | Description | Why Reference It |
|---|---|---|
| [**FIRST CSIRT Services Framework v2.1**](https://www.first.org/standards/frameworks/csirts/csirt_services_framework_v2.1) | A structured reference model describing cybersecurity services that Computer Security Incident Response Teams (CSIRTs) may provide, including monitoring, detection, analysis, and coordination. | Helps organizations define, structure, and evolve their incident response team's service portfolio. |
| [**FIRST PSIRT Services Framework v1.1**](https://www.first.org/standards/frameworks/psirts/psirt_services_framework_v1.1) | Describes services that Product Security Incident Response Teams (PSIRTs) may provide, organized into service areas covering stakeholder engagement, vulnerability intake, triage, remediation, and disclosure. | Essential for organizations building product-focused security response capabilities across the software development lifecycle. |
| [**The CERT Guide to Coordinated Vulnerability Disclosure**](https://certcc.github.io/CERT-Guide-to-CVD/) (CERT/CC) | The foundational, in-depth reference covering CVD principles, stakeholder roles, process phases, troubleshooting, and policy templates — continuously maintained by Carnegie Mellon's CERT/CC. | The authoritative academic and practitioner reference for CVD — cited by nearly every other guide in this list. |
| [**NIST SP 800-216: Recommendations for Federal Vulnerability Disclosure Guidelines**](https://csrc.nist.gov/pubs/sp/800/216/final) | NIST's guidelines for vulnerability disclosure aligned with ISO 29147 and ISO 30111, covering policies, roles, and communication. | Useful for organizations seeking compliance-oriented or government-aligned disclosure processes. |
| [**ISO/IEC 29147:2018 — Vulnerability Disclosure**](https://www.iso.org/standard/72311.html) | The international standard for how organizations should receive, process, and communicate vulnerability reports from external parties. | The global standard of record for external-facing disclosure policy and communication. |
| [**ISO/IEC 30111:2019 — Vulnerability Handling Processes**](https://www.iso.org/standard/69725.html) | The international standard for internal processes to investigate, assess, remediate, and learn from reported vulnerabilities. | Complements ISO 29147 — together they provide a complete framework for disclosure and handling. |

---

## Vulnerability Identification & Tracking

**Themes to explore:**
- *What is a CVE and how does the CVE program work?*
- *What is a CNA and how do I become one?*
- *What other vulnerability databases and identifiers exist beyond CVE?*
- *How do I look up whether a vulnerability has already been reported?*
- *Where can I find the disclosure program for a specific project?*

| Resource | Description | Why Reference It |
|---|---|---|
| [**CVE Program**](https://www.cve.org/) (MITRE/CVE.org) | The global system for identifying and cataloging publicly known cybersecurity vulnerabilities with unique CVE IDs. | The starting point for understanding vulnerability identification — referenced by every guide and framework above. |
| [**CISA Coordinated Vulnerability Disclosure Program**](https://www.cisa.gov/resources-tools/programs/coordinated-vulnerability-disclosure-program) | CISA's program for coordinating disclosure of vulnerabilities, especially those affecting critical infrastructure, using the VINCE platform. | Relevant for vulnerabilities with broad national or infrastructure impact, and as a coordination escalation path. |
| [**disclose.io**](https://disclose.io/) | A community-driven framework providing open legal/policy templates, safe harbor language, and a database of vulnerability disclosure programs. | Provides ready-to-use policy templates and helps researchers find the right disclosure channel for any project. |
