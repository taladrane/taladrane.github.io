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
| [**About Coordinated Disclosure of Security Vulnerabilities**](https://docs.github.com/en/code-security/security-advisories/guidance-on-reporting-and-writing-information-about-vulnerabilities/about-coordinated-disclosure-of-security-vulnerabilities) (GitHub Docs — Advisory Guidance) | GitHub's comprehensive documentation on the principles, expectations, and mechanics of coordinated vulnerability disclosure, situated within the advisory writing guidance. | Covers both the "why" and "how" of CVD in a single authoritative reference — useful for both newcomers and experienced practitioners. |
| [**Coordinated Vulnerability Disclosure (CVD) for Open Source Projects**](https://github.blog/security/vulnerability-research/coordinated-vulnerability-disclosure-cvd-open-source-projects/) (GitHub Blog) | A blog post discussing CVD practices tailored to the realities of open source development. | Provides practical context for why CVD in OSS is different from CVD in commercial software. |
| [**Step 4: Write an Effective Report**](https://github.blog/security/vulnerability-research/coordinated-vulnerability-disclosure-cvd-open-source-projects/#step-4-write-an-effective-report) (GitHub Blog — CVD for OSS) | The "write an effective report" section of GitHub's CVD blog post, covering what to include in a vulnerability report and how to communicate clearly. | A practical complement to the CVD blog post — focused specifically on the craft of writing a disclosure. |
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
| [**Adding a Security Policy to Your Repository**](https://docs.github.com/en/code-security/getting-started/adding-a-security-policy-to-your-repository) (GitHub Docs) | Step-by-step guidance on creating a SECURITY.md file that tells users how to report vulnerabilities, including where to place it and what to include. | Directly answers "What should a SECURITY.md include?" — the first step most maintainers should take. |
| [**Managing Privately Reported Security Vulnerabilities**](https://docs.github.com/en/code-security/security-advisories/working-with-repository-security-advisories/managing-privately-reported-security-vulnerabilities) (GitHub Docs) | Explains how maintainers can review, triage, and respond to vulnerability reports submitted through GitHub's private reporting feature. | Practical guidance for the triage and response workflow — especially useful for solo maintainers or small teams receiving their first report. |
| [**disclose.io Policymaker**](https://policymaker.disclose.io/) (disclose.io) | A free, open source tool that generates customized vulnerability disclosure policies with safe harbor language, covering intake channels, scope, and legal protections. | Helps maintainers create a professional, legally sound disclosure policy quickly — addresses the "how do I set up my project?" question without starting from scratch. |
| [**security.txt (RFC 9116)**](https://securitytxt.org/) | A proposed internet standard that defines a machine-readable file format for websites to communicate security vulnerability reporting contact information and policies. | A lightweight, widely adopted way to make your project's security contact discoverable — complements SECURITY.md for web-facing projects. |

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
| [**Vulnerability Disclosure Cheat Sheet**](https://cheatsheetseries.owasp.org/cheatsheets/Vulnerability_Disclosure_Cheat_Sheet.html) (OWASP) | A concise cheat sheet covering the end-to-end disclosure process — from discovery through reporting, communication, and public disclosure — with practical guidance for researchers and organizations alike. | An accessible quick-reference that distills vulnerability disclosure best practices into an actionable checklist format. |
| [**OpenSSF Vulnerability Disclosure Template**](https://github.com/ossf/oss-vulnerability-guide/blob/main/templates/notifications/disclosure.md) (OpenSSF) | A ready-to-use security advisory template for structuring vulnerability disclosures, including sections for summary, severity, proof of concept, remediation, and timeline. | Saves time when writing a disclosure — provides a consistent, professional structure that ensures critical information isn't missed. |
| [**Privately Reporting a Security Vulnerability**](https://docs.github.com/en/code-security/security-advisories/guidance-on-reporting-and-writing-information-about-vulnerabilities/privately-reporting-a-security-vulnerability) (GitHub Docs) | How to use GitHub's private vulnerability reporting feature to submit a report directly to a repository's maintainers without publicly exposing the issue. | The practical how-to for researchers who find a vulnerability in a GitHub-hosted project — the most common reporting path for open source. |
| [**disclose.io**](https://disclose.io/) | A community-driven project that maintains a database of vulnerability disclosure programs, standardized safe harbor terms, and resources for researchers navigating the disclosure process. | Helps researchers find whether a project has a disclosure program, understand safe harbor protections, and set expectations for the process. |

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
| [**Best Practices for Writing Repository Security Advisories**](https://docs.github.com/en/code-security/security-advisories/guidance-on-reporting-and-writing-information-about-vulnerabilities/best-practices-for-writing-repository-security-advisories) (GitHub Docs) | GitHub's guidance on how to write clear, complete, and actionable security advisories for repository vulnerabilities, including what information to include and how to structure it. | Directly applicable when drafting a GitHub Security Advisory — helps ensure advisories are useful to downstream consumers. |
| [**Collaborating in a Temporary Private Fork**](https://docs.github.com/en/code-security/security-advisories/working-with-repository-security-advisories/collaborating-in-a-temporary-private-fork-to-resolve-a-repository-security-vulnerability) (GitHub Docs) | How to create and use a temporary private fork within a security advisory to privately develop, review, and test a fix before public disclosure. | The key mechanism for private patch development on GitHub — answers "How can I use GitHub to privately develop and test a security patch?" |
| [**Publishing a Repository Security Advisory**](https://docs.github.com/en/code-security/security-advisories/working-with-repository-security-advisories/publishing-a-repository-security-advisory) (GitHub Docs) | How to publish a security advisory once a fix is ready, including how the advisory becomes public and how CVE IDs are associated. | Covers the final step of the advisory lifecycle — including the relationship between GHSA IDs and CVE IDs. |
| [**About the GitHub Advisory Database**](https://docs.github.com/en/code-security/security-advisories/global-security-advisories/about-the-github-advisory-database) (GitHub Docs) | An overview of the GitHub Advisory Database — a free, open database of security advisories organized by ecosystem, with GitHub-reviewed and unreviewed entries in the OSV format. | Explains how published advisories feed into the broader vulnerability ecosystem and power tools like Dependabot. |

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
| [**RFC 9116 — A File Format to Aid in Security Vulnerability Disclosure (security.txt)**](https://www.rfc-editor.org/rfc/rfc9116) | The IETF standard defining a machine-readable `security.txt` file that organizations place on their websites to communicate security contact information, disclosure policies, and encryption keys. | A practical, low-effort standard that makes security contacts discoverable — endorsed by CISA and widely adopted across the industry. |
| [**disclose.io — Open Source Vulnerability Disclosure Framework**](https://github.com/disclose/dioterms) (disclose.io) | A set of open source, community-driven vulnerability disclosure policy templates providing standardized safe harbor language, scope definitions, and legal protections for both organizations and researchers. | Fills the gap between ad hoc policies and formal standards — gives organizations a vetted starting point for disclosure terms without legal overhead. |

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
| [**National Vulnerability Database (NVD)**](https://nvd.nist.gov/) (NIST) | The U.S. government's comprehensive repository of standards-based vulnerability management data, enriching CVE entries with severity scores (CVSS), affected product mappings (CPE), and remediation references. | The primary source for enriched vulnerability metadata — widely used for compliance, risk assessment, and vulnerability prioritization. |
| [**OSV — Open Source Vulnerabilities**](https://osv.dev/) (Google/OpenSSF) | An open, distributed database of vulnerabilities in open source software, using the OSV schema to precisely map vulnerabilities to package versions and commit hashes across ecosystems like npm, PyPI, Maven, Go, and more. | The most developer-friendly vulnerability database — designed for automated querying and integration into CI/CD pipelines, and a key complement to CVE/NVD. |
| [**CISA Known Exploited Vulnerabilities (KEV) Catalog**](https://www.cisa.gov/known-exploited-vulnerabilities-catalog) | A catalog maintained by CISA of vulnerabilities that are confirmed to be actively exploited in the wild, with remediation deadlines for federal agencies. | Critical for prioritizing patching — if a vulnerability appears here, it should be treated as urgent regardless of CVSS score. |
| [**European Vulnerability Database (EUVD)**](https://euvd.enisa.europa.eu/) (ENISA) | The EU's centralized vulnerability database launched under the NIS2 Directive, aggregating data from national CSIRTs, vendors, and existing databases like CVE/NVD, with dashboards for critical, exploited, and EU-coordinated vulnerabilities. | An increasingly important regional complement to CVE/NVD — relevant for organizations operating in or supplying to the European market. |
| [**CISA Coordinated Vulnerability Disclosure Program**](https://www.cisa.gov/resources-tools/programs/coordinated-vulnerability-disclosure-program) | CISA's program for coordinating disclosure of vulnerabilities, especially those affecting critical infrastructure, using the VINCE platform. | Relevant for vulnerabilities with broad national or infrastructure impact, and as a coordination escalation path. |
| [**Becoming a CNA as an Open Source Project**](https://github.com/ossf/wg-vulnerability-disclosures/blob/main/docs/guides/becoming-a-cna-as-an-open-source-org-or-project.md) (OpenSSF) | A step-by-step guide for open source projects considering becoming a CVE Numbering Authority (CNA), covering self-evaluation, application, onboarding, and ongoing responsibilities. | The definitive resource for projects that want to assign their own CVE IDs — answers "What is a CNA and how do I become one?" |
| [**GitHub Advisory Database**](https://github.com/advisories) (GitHub) | A free, open, browsable database of security advisories across open source ecosystems, with GitHub-reviewed entries, severity scores, and links to affected packages. | A practical tool for checking whether a vulnerability has already been reported and for discovering advisories relevant to your dependencies. |