# Awesome Federal Identity, Credential, and Access Management (FICAM)
![awesome][(https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)
> A curated list of awesome resources for Federal Identity, Credential, and Access Management (FICAM / ICAM).
> Maintained for the federal cybersecurity, identity engineering, and Zero Trust architecture communities.
> 
> **Last Updated:** August 2026

---

## Contents

- [Official Portals & Program Offices](#official-portals--program-offices)
- [Policy & OMB Guidance](#policy--omb-guidance)
- [NIST Standards & Guidelines](#nist-standards--guidelines)
- [FICAM Architecture](#ficam-architecture)
- [Playbooks](#playbooks)
- [PIV / Personal Identity Verification](#piv--personal-identity-verification)
- [Derived PIV Credentials](#derived-piv-credentials)
- [PIV Federation](#piv-federation)
- [FPKI / Federal Public Key Infrastructure](#fpki--federal-public-key-infrastructure)
- [PACS / Physical Access Control Systems](#pacs--physical-access-control-systems)
- [Zero Trust & ICAM](#zero-trust--icam)
- [CISA Resources](#cisa-resources)
- [GitHub Repositories & Open Source](#github-repositories--open-source)
- [Training & Education](#training--education)
- [Communities of Practice](#communities-of-practice)
- [Historical / Legacy Resources](#historical--legacy-resources)
- [Contributing](#contributing)

---

## Official Portals & Program Offices

*The primary government portals and program offices driving federal ICAM policy and implementation.*

- **[IDManagement.gov](https://www.idmanagement.gov/)** — The federal government's central hub for FICAM guidance, playbooks, architecture, and standards. Managed by GSA's Identity Assurance and Trusted Access Division in coordination with the Federal CIO Council ICAM Subcommittee.
- **[GSA FICAM Program](https://www.gsa.gov/technology/government-it-initiatives/identity-credentialing-and-access-management)** — GSA Office of Government-wide Policy's FICAM program management office.
- **[NIST Identity & Access Management](https://www.nist.gov/identity-access-management)** — NIST's central portal for identity management research, standards, and projects including PIV and digital identity guidelines.
- **[USAccess](https://www.usaccess.gov/)** — The federal shared service provider for HSPD-12 credentialing, offering standardized PIV enrollment and identity proofing services across agencies.
- **[CISA ICAM Resources](https://www.cisa.gov/)** — CISA's identity, credential, and access management guidance tied to Continuous Diagnostics and Mitigation (CDM) and Zero Trust.

---

## Policy & OMB Guidance

*The policy foundations that mandate and shape federal ICAM implementation.*

- **[OMB M-19-17](https://www.whitehouse.gov/wp-content/uploads/2019/05/M-19-17.pdf)** — *Enabling Mission Delivery through Improved Identity, Credential, and Access Management* (May 2019). The cornerstone federal ICAM policy memorandum establishing agency-wide ICAM programs, PIV credential requirements, digital signature mandates, and cross-government identity federation.
- **[OMB M-22-09](https://www.whitehouse.gov/omb/management/ofcio/federal-zero-trust-strategy/)** — *Moving the U.S. Government Toward Zero Trust Cybersecurity Principles* (January 2022). Establishes the Federal Zero Trust Strategy with specific identity pillar requirements including enterprise-managed identities and phishing-resistant MFA.
- **[Executive Order 14028](https://www.whitehouse.gov/briefing-room/presidential-actions/2021/05/12/executive-order-on-improving-the-nations-cybersecurity/)** — *Improving the Nation's Cybersecurity* (May 2021). Directs federal agencies to adopt Zero Trust Architecture, MFA, and encryption requirements.
- **[HSPD-12](https://www.dhs.gov/homeland-security-presidential-directive-12)** — *Policy for a Common Identification Standard for Federal Employees and Contractors*. The 2004 directive that mandates the PIV credential.
- **[FISMA 2014](https://www.congress.gov/bill/113th-congress/senate-bill/2521)** — *Federal Information Security Modernization Act of 2014*. Provides the statutory foundation for federal cybersecurity and risk management frameworks that underpin ICAM.

---

## NIST Standards & Guidelines

*The technical standards that define how federal digital identity and credentials operate.*

### Digital Identity Guidelines (SP 800-63 Suite)

- **[NIST SP 800-63-4](https://pages.nist.gov/800-63-4/)** — *Digital Identity Guidelines* (August 2025). The current revision replacing 800-63-3. Defines IAL, AAL, and FAL with updated risk management processes, fraud requirements, deepfake protections, and syncable authenticator (passkey) guidance.
- **[NIST SP 800-63A](https://pages.nist.gov/800-63-3/sp800-63a.html)** — *Enrollment and Identity Proofing* (superseded by 800-63-4 but still widely referenced).
- **[NIST SP 800-63B](https://pages.nist.gov/800-63-3/sp800-63b.html)** — *Authentication and Lifecycle Management* (superseded by 800-63-4).
- **[NIST SP 800-63C](https://pages.nist.gov/800-63-3/sp800-63c.html)** — *Federation and Assertions* (superseded by 800-63-4).
- **[NIST SP 800-63B Sup 1](https://csrc.nist.gov/pubs/sp/800/63/b/sup1/final)** — *Incorporating Syncable Authenticators into NIST SP 800-63B* (April 2024). Guidance on passkeys and synced authenticators.
- **[NIST SP 800-63-3 FAQ & Implementation Resources](https://pages.nist.gov/800-63-3/)** — Archive of 800-63-3 implementation guidance and conformance criteria.

### PIV Standards

- **[FIPS 201-3](https://csrc.nist.gov/pubs/fips/201-3/final)** — *Personal Identity Verification (PIV) of Federal Employees and Contractors*. The current standard governing PIV credential identity proofing, enrollment, issuance, and lifecycle.
- **[NIST SP 800-73-5](https://csrc.nist.gov/pubs/sp/800/73/5/final)** — *Interfaces for Personal Identity Verification*.
- **[NIST SP 800-76-2](https://csrc.nist.gov/pubs/sp/800/76/2/final)** — *Biometric Specifications for Personal Identity Verification*.
- **[NIST SP 800-78-5](https://csrc.nist.gov/pubs/sp/800/78/5/final)** — *Cryptographic Algorithms and Key Sizes for Personal Identity Verification*.
- **[NIST SP 800-116 Rev. 1](https://csrc.nist.gov/pubs/sp/800/116/r1/final)** — *Guidelines for the Use of PIV Credentials in Facility Access*.
- **[NIST SP 800-157 Rev. 1 (Draft)](https://csrc.nist.gov/pubs/sp/800/157/r1/fpd)** — *Guidelines for Derived Personal Identity Verification (PIV) Credentials* (Final Public Draft, November 2024). Expanded derived credentials including PKI and non-PKI phishing-resistant authenticators.
- **[NIST SP 800-217 (Draft)](https://csrc.nist.gov/pubs/sp/800/217/fpd)** — *Guidelines for Personal Identity Verification (PIV) Federation* (Final Public Draft, November 2024). Technical requirements for federated PIV identity and cross-domain assertions.

### Supporting NIST Publications

- **[NIST SP 800-53 Rev. 5](https://csrc.nist.gov/pubs/sp/800/53/r5/upd1/final)** — *Security and Privacy Controls for Information Systems and Organizations*. Contains the IA (Identification and Authentication) control family referenced across FICAM implementations.
- **[NIST SP 800-207](https://csrc.nist.gov/pubs/sp/800/207/final)** — *Zero Trust Architecture* (August 2020). The foundational NIST publication on Zero Trust principles.

---

## FICAM Architecture

*The structural framework for how federal agencies manage identity, credential, and access management.*

- **[FICAM Architecture v3.0](https://www.idmanagement.gov/architecture/)** — The current FICAM segment architecture hosted on IDManagement.gov, replacing the 2011 FICAM Roadmap v2.0.
- **[FICAM Roadmap and Implementation Guidance v2.0 (2011)](https://www.idmanagement.gov/docs/roadmap-ficam.pdf)** — The original comprehensive FICAM roadmap (legacy reference).
- **[FICAM Program Management Playbook](https://www.idmanagement.gov/playbooks/ficampm/)** — Guidance for establishing and managing agency ICAM programs.
- **[ICAM Governance Framework](https://www.idmanagement.gov/playbooks/icamgov/)** — A tool to help agencies build and improve ICAM governance structures, processes, and policies.

---

## Playbooks

*Practical, step-by-step guidance for federal ICAM implementations.*

- **[Cloud Identity Playbook](https://www.idmanagement.gov/playbooks/cloud/)** — Four-step playbook for expanding Workforce ICAM Services in a cloud operating model.
- **[Digital Identity Risk Assessment Playbook](https://www.idmanagement.gov/playbooks/dira/)** — Six-step playbook for completing digital identity risk assessments per OMB M-19-17 and NIST SP 800-63.
- **[Digital Worker Identity Playbook](https://www.idmanagement.gov/playbooks/dw/)** — Practical guide for managing digital worker (non-person entity / NPE) identities.
- **[Enterprise SSO Playbook](https://www.idmanagement.gov/playbooks/sso/)** — Five-step playbook for planning SSO or Identity Federation services.
- **[Delegated Digital Signature Playbook](https://www.idmanagement.gov/playbooks/sign/)** — Process for implementing delegated digital signatures for Federal Register documents.
- **[Digital Signatures Guide](https://www.idmanagement.gov/playbooks/signfedregister/)** — Steps for digitally signing documents using PIV credentials or PKI-based certificates.
- **[Identity Fraud Playbook](https://www.idmanagement.gov/playbooks/fraud/)** — Resource on identity fraud techniques, detection methods, and mitigation strategies.
- **[Phishing-Resistant Authenticator Playbook](https://www.idmanagement.gov/playbooks/auth/)** — Helps agencies identify phishing-resistant alternative authenticators and design pilots.
- **[Privileged User Playbook](https://www.idmanagement.gov/playbooks/privileged/)** — Best practices for managing privileged user populations.
- **[Identity Lifecycle Management Playbook](https://www.idmanagement.gov/playbooks/ilm/)** — Guidance on shifting from credential lifecycle management to identity lifecycle management per OMB M-19-17 Section III.

---

## PIV / Personal Identity Verification

*Resources for implementing and managing PIV credentials.*

- **[PIV Guides (IDManagement.gov)](https://www.idmanagement.gov/university/piv/)** — Comprehensive guides for PIV credential usage, implementation, and troubleshooting.
- **[PIV Usage Guides (GitHub Pages)](https://gsallewell.github.io/piv-guides/)** — Open-source community guides for common PIV configurations (logical access focus).
- **[FIPS 201 Approved Products List (APL)](https://www.idmanagement.gov/fips201/)** — GSA's approved products list for PIV cards and PACS devices.
- **[NIST PIV Project Page](https://www.nist.gov/identity-access-management/projects/personal-identity-verification-piv)** — Central NIST resource for FIPS 201 and associated special publications.
- **[USAccess Enrollment](https://www.usaccess.gov/)** — Federal shared service for PIV enrollment and credentialing.
- **[PIV Card Visual Appearance Guidelines](https://www.idmanagement.gov/docs/piv-card-graphics.pdf)** — Standardized visual design requirements for PIV credentials.

---

## Derived PIV Credentials

*Mobile and alternative authenticators derived from the PIV credential.*

- **[NIST SP 800-157 Rev. 1 (Draft)](https://csrc.nist.gov/pubs/sp/800/157/r1/fpd)** — *Guidelines for Derived Personal Identity Verification (PIV) Credentials* (Final Public Draft, November 2024). Covers PKI-based and non-PKI derived credentials.
- **[Derived PIV Credentials Overview (IDManagement.gov)](https://www.idmanagement.gov/university/piv/#derived-piv-credentials)** — Federal guidance on implementing derived credentials for mobile devices.
- **[Mobile Identity Management (CISA CDM)](https://www.cisa.gov/continuous-diagnostics-and-mitigation)** — CISA CDM program guidance on mobile identity management as part of ICAM architectures.

---

## PIV Federation

*Cross-domain and interagency use of PIV identity accounts.*

- **[NIST SP 800-217 (Draft)](https://csrc.nist.gov/pubs/sp/800/217/fpd)** — *Guidelines for Personal Identity Verification (PIV) Federation* (Final Public Draft, November 2024). The primary technical reference for PIV federation.
- **[Federation Playbook (IDManagement.gov)](https://www.idmanagement.gov/playbooks/federation/)** — Practical guidance for federating application access across agencies.
- **[Attribute Supported Federation](https://www.idmanagement.gov/playbooks/attributes/)** — Guidance on attribute exchange in federated environments.
- **[Trust Frameworks](https://www.idmanagement.gov/playbooks/trust/)** — Information on federal trust frameworks for identity federation.
- **[GSA FICAM Federation (Archived)](https://github.com/GSA/ficam-federation)** — Archived GitHub repository; content migrated to IDManagement.gov playbooks.

---

## FPKI / Federal Public Key Infrastructure

*The network of certification authorities that underpin federal trust.*

- **[FPKI Guides (IDManagement.gov)](https://www.idmanagement.gov/university/fpki/)** — Federal Public Key Infrastructure guides, tools, and tips.
- **[FPKI Governance](https://www.idmanagement.gov/governance/fpkiaudit/)** — FPKI policies, profiles, annual review schedules, and compliance status.
- **[FPKI Graph](https://www.idmanagement.gov/governance/fpkigraph/)** — Interactive chart of Federal PKI certification authorities and cross-certified communities.
- **[Federal Common Policy CA G2](https://www.idmanagement.gov/governance/fpkiaudit/#federal-common-policy-ca-g2)** — The root CA for federal Executive Branch agencies.
- **[GSA PKI Shared Services Provider Program](https://www.idmanagement.gov/governance/gsapkissp/)** — GSA program helping agencies meet HSPD-12 and digital signature interoperability.
- **[NIST SP 800-32 (Withdrawn)](https://csrc.nist.gov/pubs/sp/800/32/final)** — *Introduction to Public Key Technology and the Federal PKI Infrastructure* (legacy reference; see IDManagement.gov for current guidance).

---

## PACS / Physical Access Control Systems

*Systems controlling physical access to federal facilities via electronic credential authentication.*

- **[PACS 101 (IDManagement.gov)](https://www.idmanagement.gov/university/pacs/)** — Introduction to FICAM-compliant Physical Access Control Systems.
- **[PACS Playbook](https://www.idmanagement.gov/playbooks/pacs/)** — Guidance for planning, procuring, and deploying PIV-enabled PACS.
- **[GSA PACS in GSA-Controlled Space](https://www.gsa.gov/directives-library/physical-access-control-systems-in-us-general-services-administration-controlled-space)** — GSA agency-wide PACS policy and implementation order.
- **[FIPS 201 Evaluation Program](https://www.idmanagement.gov/fips201/)** — Testing and evaluation program for PACS products.
- **[Secure Technology Alliance PACS Webinar Series](https://www.idmanagement.gov/university/pacs/#industry-training)** — Six-part industry webinar on planning, procuring, and deploying PIV-enabled PACS.
- **[NIST SP 800-116 Rev. 1](https://csrc.nist.gov/pubs/sp/800/116/r1/final)** — *Guidelines for the Use of PIV Credentials in Facility Access*.

---

## Zero Trust & ICAM

*Resources connecting identity management to federal Zero Trust implementation.*

- **[OMB M-22-09: Federal Zero Trust Strategy](https://www.whitehouse.gov/omb/management/ofcio/federal-zero-trust-strategy/)** — The policy document requiring agencies to achieve Zero Trust goals by FY2024.
- **[CISA Zero Trust Maturity Model](https://www.cisa.gov/zero-trust-maturity-model)** — CISA's model organizing Zero Trust implementation across five pillars: Identity, Devices, Networks, Applications, and Data.
- **[CISA CDM ICAM Reference Architecture](https://www.cisa.gov/continuous-diagnostics-and-mitigation)** — CISA's 2023 guidance on integrating IDAM capabilities into ICAM architectures to enable Zero Trust.
- **[IDManagement.gov Zero Trust Resources](https://digital.gov/2023/10/02/new-idmanagement-gov-is-refreshing-the-conversation-about-zero-trust/)** — Refreshed IDManagement.gov content focused on Zero Trust and identity-first security.
- **[NIST SP 800-207](https://csrc.nist.gov/pubs/sp/800/207/final)** — *Zero Trust Architecture*.

---

## CISA Resources

*CISA's technical and architectural guidance for federal ICAM.*

- **[CISA Continuous Diagnostics and Mitigation (CDM)](https://www.cisa.gov/continuous-diagnostics-and-mitigation)** — Program providing ISCM capabilities including IDAM/ICAM integration.
- **[CISA ICAM Reference Architecture (2023)](https://www.cisa.gov/continuous-diagnostics-and-mitigation)** — Document clarifying CDM IDAM scope, capabilities, and a reference architecture for robust ICAM deployment.
- **[CISA Zero Trust Maturity Model](https://www.cisa.gov/zero-trust-maturity-model)** — Cross-pillar maturity model for federal Zero Trust implementation.
- **[CISA Cybersecurity Performance Goals](https://www.cisa.gov/cross-sector-cybersecurity-performance-goals)** — Includes identity and access management baseline goals for critical infrastructure.

---

## GitHub Repositories & Open Source

*Open-source repositories, code, and collaborative development spaces for federal ICAM.*

- **[GSA/idmanagement.gov](https://github.com/GSA/idmanagement.gov)** — The public GitHub repository for IDManagement.gov. Contains source files for playbooks, architecture, and FPKI/PACS/PIV guides. Open for community contributions.
- **[GSA/ficam-arch](https://github.com/GSA/ficam-arch)** — FICAM Architecture repository (archived; content migrated to idmanagement.gov).
- **[GSA/ficam-federation](https://github.com/GSA/ficam-federation)** — Federation playbook repository (archived; content migrated to idmanagement.gov).
- **[PIV Guides (Community)](https://gsallewell.github.io/piv-guides/)** — Community-driven open-source PIV usage guides.
- **[USWDS (U.S. Web Design System)](https://github.com/uswds/uswds)** — While not ICAM-specific, many federal identity portals use USWDS for accessible, standardized frontend design.

---

## Training & Education

*Courses, webinars, and self-paced learning resources.*

- **[IDManagement.gov University](https://www.idmanagement.gov/university/)** — Free self-paced training on ICAM basics, PKI, PIV, PACS, and digital identity risk assessment.
- **[NIST Computer Security Resource Center (CSRC)](https://csrc.nist.gov/)** — Publications, workshops, and events on digital identity and PIV standards.
- **[Secure Technology Alliance Webinars](https://www.idmanagement.gov/university/pacs/#industry-training)** — PACS-focused industry training series.
- **[Federal CIO Council ICAM Subcommittee](https://www.cio.gov/)** — Policy and guidance coordination across federal agencies.
- **[Digital.gov Events](https://digital.gov/events/)** — Federal community events often featuring ICAM and identity modernization topics.

---

## Communities of Practice

*Forums, working groups, and collaborative spaces for federal ICAM practitioners.*

- **[Federal CIO Council ICAM Subcommittee](https://www.cio.gov/)** — The interagency body coordinating federal ICAM policy and implementation.
- **[ATARC Identity Management Working Group](https://atarc.org/working-groups/identity-management/)** — Advanced Technology Academic Research Center working group providing industry and government collaboration on identity challenges.
- **[IDManagement.gov Contribute Page](https://www.idmanagement.gov/contribute/)** — Guidelines for contributing to federal ICAM content via GitHub.
- **[ICAMSC (ICAM Subcommittee)](https://www.idmanagement.gov/icamsc/)** — Community space for the Federal CIO Council's ICAM Subcommittee.

---

## Historical / Legacy Resources

*Older resources retained for reference and historical context.*

- **[FICAM Roadmap and Implementation Guidance v2.0 (2011)](https://www.idmanagement.gov/docs/roadmap-ficam.pdf)** — The original comprehensive FICAM roadmap. Superseded by the current FICAM Architecture v3.0 and playbooks.
- **[NIST SP 800-63-3 (Withdrawn)](https://pages.nist.gov/800-63-3/)** — Superseded by SP 800-63-4 (August 2025). Still referenced in many agency implementations during transition.
- **[NIST SP 800-63-2](https://csrc.nist.gov/pubs/sp/800/63/2/final)** — Earlier version using the four LOA model. Superseded by 800-63-3 and now 800-63-4.
- **[GSA FICAM Federation (Archived)](https://github.com/GSA/ficam-federation)** — Archived repository; federation content now lives in IDManagement.gov playbooks.
- **[Awesome FICAM (Legacy)](https://github.com/GSA/ficam-federation)** — Earlier community resource lists (circa 2016-2018). This list aims to replace and modernize those efforts.

---

## Contributing

Contributions welcome! This list is maintained to help federal practitioners, contractors, and identity engineers find current, authoritative FICAM resources quickly.

**Guidelines:**
- Prioritize official government sources (GSA, NIST, CISA, OMB, White House).
- Flag draft or pre-release documents clearly.
- Remove or deprecate links that are superseded by newer guidance.
- Keep descriptions concise and actionable.

**To contribute:** Open a PR or issue. Follow the [IDManagement.gov contribution model](https://www.idmanagement.gov/contribute/) for style and plain-language guidance.

---

## License

This list is provided as a public resource. Where applicable, linked government content is in the public domain or licensed under CC0.

---

> **Disclaimer:** This is an unofficial curated list. Always verify guidance against the latest official publications from GSA, NIST, OMB, and CISA. Standards and policy evolve rapidly in the federal identity space.
