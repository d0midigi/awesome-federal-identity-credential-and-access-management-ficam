Awesome FICAM
> A curated list of awesome resources for Federal Identity, Credential, and Access Management (FICAM / ICAM).
> Maintained for the federal cybersecurity, identity engineering, and Zero Trust architecture communities.
> 
> **Last Updated:** August 2026
---
Contents
Official Portals & Program Offices
Policy & OMB Guidance
NIST Standards & Guidelines
FICAM Architecture
Playbooks
PIV / Personal Identity Verification
Derived PIV Credentials
PIV Federation
FPKI / Federal Public Key Infrastructure
PACS / Physical Access Control Systems
Zero Trust & ICAM
CISA Resources
GitHub Repositories & Open Source
Training & Education
Communities of Practice
Historical / Legacy Resources
Contributing
---
Official Portals & Program Offices
The primary government portals and program offices driving federal ICAM policy and implementation.
IDManagement.gov — The federal government's central hub for FICAM guidance, playbooks, architecture, and standards. Managed by GSA's Identity Assurance and Trusted Access Division in coordination with the Federal CIO Council ICAM Subcommittee.
GSA FICAM Program — GSA Office of Government-wide Policy's FICAM program management office.
NIST Identity & Access Management — NIST's central portal for identity management research, standards, and projects including PIV and digital identity guidelines.
USAccess — The federal shared service provider for HSPD-12 credentialing, offering standardized PIV enrollment and identity proofing services across agencies.
CISA ICAM Resources — CISA's identity, credential, and access management guidance tied to Continuous Diagnostics and Mitigation (CDM) and Zero Trust.
---
Policy & OMB Guidance
The policy foundations that mandate and shape federal ICAM implementation.
OMB M-19-17 — Enabling Mission Delivery through Improved Identity, Credential, and Access Management (May 2019). The cornerstone federal ICAM policy memorandum establishing agency-wide ICAM programs, PIV credential requirements, digital signature mandates, and cross-government identity federation.
OMB M-22-09 — Moving the U.S. Government Toward Zero Trust Cybersecurity Principles (January 2022). Establishes the Federal Zero Trust Strategy with specific identity pillar requirements including enterprise-managed identities and phishing-resistant MFA.
Executive Order 14028 — Improving the Nation's Cybersecurity (May 2021). Directs federal agencies to adopt Zero Trust Architecture, MFA, and encryption requirements.
HSPD-12 — Policy for a Common Identification Standard for Federal Employees and Contractors. The 2004 directive that mandates the PIV credential.
FISMA 2014 — Federal Information Security Modernization Act of 2014. Provides the statutory foundation for federal cybersecurity and risk management frameworks that underpin ICAM.
---
NIST Standards & Guidelines
The technical standards that define how federal digital identity and credentials operate.
Digital Identity Guidelines (SP 800-63 Suite)
NIST SP 800-63-4 — Digital Identity Guidelines (August 2025). The current revision replacing 800-63-3. Defines IAL, AAL, and FAL with updated risk management processes, fraud requirements, deepfake protections, and syncable authenticator (passkey) guidance.
NIST SP 800-63A — Enrollment and Identity Proofing (superseded by 800-63-4 but still widely referenced).
NIST SP 800-63B — Authentication and Lifecycle Management (superseded by 800-63-4).
NIST SP 800-63C — Federation and Assertions (superseded by 800-63-4).
NIST SP 800-63B Sup 1 — Incorporating Syncable Authenticators into NIST SP 800-63B (April 2024). Guidance on passkeys and synced authenticators.
NIST SP 800-63-3 FAQ & Implementation Resources — Archive of 800-63-3 implementation guidance and conformance criteria.
PIV Standards
FIPS 201-3 — Personal Identity Verification (PIV) of Federal Employees and Contractors. The current standard governing PIV credential identity proofing, enrollment, issuance, and lifecycle.
NIST SP 800-73-5 — Interfaces for Personal Identity Verification.
NIST SP 800-76-2 — Biometric Specifications for Personal Identity Verification.
NIST SP 800-78-5 — Cryptographic Algorithms and Key Sizes for Personal Identity Verification.
NIST SP 800-116 Rev. 1 — Guidelines for the Use of PIV Credentials in Facility Access.
NIST SP 800-157 Rev. 1 (Draft) — Guidelines for Derived Personal Identity Verification (PIV) Credentials (Final Public Draft, November 2024). Expanded derived credentials including PKI and non-PKI phishing-resistant authenticators.
NIST SP 800-217 (Draft) — Guidelines for Personal Identity Verification (PIV) Federation (Final Public Draft, November 2024). Technical requirements for federated PIV identity and cross-domain assertions.
Supporting NIST Publications
NIST SP 800-53 Rev. 5 — Security and Privacy Controls for Information Systems and Organizations. Contains the IA (Identification and Authentication) control family referenced across FICAM implementations.
NIST SP 800-207 — Zero Trust Architecture (August 2020). The foundational NIST publication on Zero Trust principles.
---
FICAM Architecture
The structural framework for how federal agencies manage identity, credential, and access management.
FICAM Architecture v3.0 — The current FICAM segment architecture hosted on IDManagement.gov, replacing the 2011 FICAM Roadmap v2.0.
FICAM Roadmap and Implementation Guidance v2.0 (2011) — The original comprehensive FICAM roadmap (legacy reference).
FICAM Program Management Playbook — Guidance for establishing and managing agency ICAM programs.
ICAM Governance Framework — A tool to help agencies build and improve ICAM governance structures, processes, and policies.
---
Playbooks
Practical, step-by-step guidance for federal ICAM implementations.
Cloud Identity Playbook — Four-step playbook for expanding Workforce ICAM Services in a cloud operating model.
Digital Identity Risk Assessment Playbook — Six-step playbook for completing digital identity risk assessments per OMB M-19-17 and NIST SP 800-63.
Digital Worker Identity Playbook — Practical guide for managing digital worker (non-person entity / NPE) identities.
Enterprise SSO Playbook — Five-step playbook for planning SSO or Identity Federation services.
Delegated Digital Signature Playbook — Process for implementing delegated digital signatures for Federal Register documents.
Digital Signatures Guide — Steps for digitally signing documents using PIV credentials or PKI-based certificates.
Identity Fraud Playbook — Resource on identity fraud techniques, detection methods, and mitigation strategies.
Phishing-Resistant Authenticator Playbook — Helps agencies identify phishing-resistant alternative authenticators and design pilots.
Privileged User Playbook — Best practices for managing privileged user populations.
Identity Lifecycle Management Playbook — Guidance on shifting from credential lifecycle management to identity lifecycle management per OMB M-19-17 Section III.
---
PIV / Personal Identity Verification
Resources for implementing and managing PIV credentials.
PIV Guides (IDManagement.gov) — Comprehensive guides for PIV credential usage, implementation, and troubleshooting.
PIV Usage Guides (GitHub Pages) — Open-source community guides for common PIV configurations (logical access focus).
FIPS 201 Approved Products List (APL) — GSA's approved products list for PIV cards and PACS devices.
NIST PIV Project Page — Central NIST resource for FIPS 201 and associated special publications.
USAccess Enrollment — Federal shared service for PIV enrollment and credentialing.
PIV Card Visual Appearance Guidelines — Standardized visual design requirements for PIV credentials.
---
Derived PIV Credentials
Mobile and alternative authenticators derived from the PIV credential.
NIST SP 800-157 Rev. 1 (Draft) — Guidelines for Derived Personal Identity Verification (PIV) Credentials (Final Public Draft, November 2024). Covers PKI-based and non-PKI derived credentials.
Derived PIV Credentials Overview (IDManagement.gov) — Federal guidance on implementing derived credentials for mobile devices.
Mobile Identity Management (CISA CDM) — CISA CDM program guidance on mobile identity management as part of ICAM architectures.
---
PIV Federation
Cross-domain and interagency use of PIV identity accounts.
NIST SP 800-217 (Draft) — Guidelines for Personal Identity Verification (PIV) Federation (Final Public Draft, November 2024). The primary technical reference for PIV federation.
Federation Playbook (IDManagement.gov) — Practical guidance for federating application access across agencies.
Attribute Supported Federation — Guidance on attribute exchange in federated environments.
Trust Frameworks — Information on federal trust frameworks for identity federation.
GSA FICAM Federation (Archived) — Archived GitHub repository; content migrated to IDManagement.gov playbooks.
---
FPKI / Federal Public Key Infrastructure
The network of certification authorities that underpin federal trust.
FPKI Guides (IDManagement.gov) — Federal Public Key Infrastructure guides, tools, and tips.
FPKI Governance — FPKI policies, profiles, annual review schedules, and compliance status.
FPKI Graph — Interactive chart of Federal PKI certification authorities and cross-certified communities.
Federal Common Policy CA G2 — The root CA for federal Executive Branch agencies.
GSA PKI Shared Services Provider Program — GSA program helping agencies meet HSPD-12 and digital signature interoperability.
NIST SP 800-32 (Withdrawn) — Introduction to Public Key Technology and the Federal PKI Infrastructure (legacy reference; see IDManagement.gov for current guidance).
---
PACS / Physical Access Control Systems
Systems controlling physical access to federal facilities via electronic credential authentication.
PACS 101 (IDManagement.gov) — Introduction to FICAM-compliant Physical Access Control Systems.
PACS Playbook — Guidance for planning, procuring, and deploying PIV-enabled PACS.
GSA PACS in GSA-Controlled Space — GSA agency-wide PACS policy and implementation order.
FIPS 201 Evaluation Program — Testing and evaluation program for PACS products.
Secure Technology Alliance PACS Webinar Series — Six-part industry webinar on planning, procuring, and deploying PIV-enabled PACS.
NIST SP 800-116 Rev. 1 — Guidelines for the Use of PIV Credentials in Facility Access.
---
Zero Trust & ICAM
Resources connecting identity management to federal Zero Trust implementation.
OMB M-22-09: Federal Zero Trust Strategy — The policy document requiring agencies to achieve Zero Trust goals by FY2024.
CISA Zero Trust Maturity Model — CISA's model organizing Zero Trust implementation across five pillars: Identity, Devices, Networks, Applications, and Data.
CISA CDM ICAM Reference Architecture — CISA's 2023 guidance on integrating IDAM capabilities into ICAM architectures to enable Zero Trust.
IDManagement.gov Zero Trust Resources — Refreshed IDManagement.gov content focused on Zero Trust and identity-first security.
NIST SP 800-207 — Zero Trust Architecture.
---
CISA Resources
CISA's technical and architectural guidance for federal ICAM.
CISA Continuous Diagnostics and Mitigation (CDM) — Program providing ISCM capabilities including IDAM/ICAM integration.
CISA ICAM Reference Architecture (2023) — Document clarifying CDM IDAM scope, capabilities, and a reference architecture for robust ICAM deployment.
CISA Zero Trust Maturity Model — Cross-pillar maturity model for federal Zero Trust implementation.
CISA Cybersecurity Performance Goals — Includes identity and access management baseline goals for critical infrastructure.
---
GitHub Repositories & Open Source
Open-source repositories, code, and collaborative development spaces for federal ICAM.
GSA/idmanagement.gov — The public GitHub repository for IDManagement.gov. Contains source files for playbooks, architecture, and FPKI/PACS/PIV guides. Open for community contributions.
GSA/ficam-arch — FICAM Architecture repository (archived; content migrated to idmanagement.gov).
GSA/ficam-federation — Federation playbook repository (archived; content migrated to idmanagement.gov).
PIV Guides (Community) — Community-driven open-source PIV usage guides.
USWDS (U.S. Web Design System) — While not ICAM-specific, many federal identity portals use USWDS for accessible, standardized frontend design.
---
Training & Education
Courses, webinars, and self-paced learning resources.
IDManagement.gov University — Free self-paced training on ICAM basics, PKI, PIV, PACS, and digital identity risk assessment.
NIST Computer Security Resource Center (CSRC) — Publications, workshops, and events on digital identity and PIV standards.
Secure Technology Alliance Webinars — PACS-focused industry training series.
Federal CIO Council ICAM Subcommittee — Policy and guidance coordination across federal agencies.
Digital.gov Events — Federal community events often featuring ICAM and identity modernization topics.
---
Communities of Practice
Forums, working groups, and collaborative spaces for federal ICAM practitioners.
Federal CIO Council ICAM Subcommittee — The interagency body coordinating federal ICAM policy and implementation.
ATARC Identity Management Working Group — Advanced Technology Academic Research Center working group providing industry and government collaboration on identity challenges.
IDManagement.gov Contribute Page — Guidelines for contributing to federal ICAM content via GitHub.
ICAMSC (ICAM Subcommittee) — Community space for the Federal CIO Council's ICAM Subcommittee.
---
Historical / Legacy Resources
Older resources retained for reference and historical context.
FICAM Roadmap and Implementation Guidance v2.0 (2011) — The original comprehensive FICAM roadmap. Superseded by the current FICAM Architecture v3.0 and playbooks.
NIST SP 800-63-3 (Withdrawn) — Superseded by SP 800-63-4 (August 2025). Still referenced in many agency implementations during transition.
NIST SP 800-63-2 — Earlier version using the four LOA model. Superseded by 800-63-3 and now 800-63-4.
GSA FICAM Federation (Archived) — Archived repository; federation content now lives in IDManagement.gov playbooks.
Awesome FICAM (Legacy) — Earlier community resource lists (circa 2016-2018). This list aims to replace and modernize those efforts.
---
Contributing
Contributions welcome! This list is maintained to help federal practitioners, contractors, and identity engineers find current, authoritative FICAM resources quickly.
Guidelines:
Prioritize official government sources (GSA, NIST, CISA, OMB, White House).
Flag draft or pre-release documents clearly.
Remove or deprecate links that are superseded by newer guidance.
Keep descriptions concise and actionable.
To contribute: Open a PR or issue. Follow the IDManagement.gov contribution model for style and plain-language guidance.
---
License
This list is provided as a public resource. Where applicable, linked government content is in the public domain or licensed under CC0.
---
> **Disclaimer:** This is an unofficial curated list. Always verify guidance against the latest official publications from GSA, NIST, OMB, and CISA. Standards and policy evolve rapidly in the federal identity space.
