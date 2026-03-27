# Compliance Framework Comparison Matrix

Detailed comparison tables for 20+ compliance frameworks with industry applicability, control overlap, cost analysis, and a "comply once, satisfy many" implementation guide.

Last Reviewed: March 2026

---

## Table of Contents

1. [Framework Overview Matrix](#framework-overview-matrix)
2. [Control Domain Overlap Matrix](#control-domain-overlap-matrix)
3. [Industry Applicability Matrix](#industry-applicability-matrix)
4. [Cost and Effort Matrix](#cost-and-effort-matrix)
5. [Assessment and Certification Matrix](#assessment-and-certification-matrix)
6. [Enforcement and Penalties Matrix](#enforcement-and-penalties-matrix)
7. [Framework-to-Framework Overlap Percentages](#framework-to-framework-overlap-percentages)
8. [Comply Once Satisfy Many Implementation Guide](#comply-once-satisfy-many-implementation-guide)

---

## Framework Overview Matrix

### Federal and Government Frameworks

| Framework | Governing Body | Current Version | Effective Date | Legal Authority | Scope |
|---|---|---|---|---|---|
| NIST SP 800-53 | NIST | Rev. 5 | September 2020 | FISMA (44 U.S.C. 3551) | Federal info systems, voluntary for private sector |
| NIST SP 800-171 | NIST | Rev. 2 (Rev. 3 published May 2024) | February 2020 | DFARS 252.204-7012 | Nonfederal systems with CUI |
| CMMC 2.0 | DoD / CyberAB | 2.0 | October 2024 (32 CFR 170) | 32 CFR Part 170 | Defense Industrial Base |
| FedRAMP | GSA / FedRAMP PMO | Current baselines | Ongoing | OMB Memo, FISMA | Cloud services for federal agencies |
| StateRAMP | StateRAMP | Current baselines | Ongoing | State-level policies | Cloud services for state/local government |
| FISMA | OMB / NIST | 2014 (amended) | 2014 | FISMA Modernization Act | Federal agencies and contractors |
| IRS Pub 1075 | IRS | 2021 revision | 2021 | IRC 6103 | Federal Tax Information recipients |
| CJIS Security Policy | FBI / CJIS Division | v5.9.1 | June 2023 | 28 CFR Part 20 | Criminal Justice Information access |

### Industry-Specific Frameworks

| Framework | Governing Body | Current Version | Effective Date | Legal Authority | Scope |
|---|---|---|---|---|---|
| HIPAA Security Rule | HHS / OCR | 2003 (NPRM 2024) | April 2003 | HIPAA (42 U.S.C. 1320d) | Covered entities and business associates |
| PCI DSS | PCI SSC | 4.0.1 | March 2024 | Payment card brand contracts | Cardholder data handlers |
| GLBA / FTC Safeguards | FTC | Amended 2023 | June 2023 | GLBA (15 U.S.C. 6801) | Non-bank financial institutions |
| SOX (IT Controls) | SEC / PCAOB | 2002 | July 2002 | Sarbanes-Oxley Act | Public companies |
| ITAR | DDTC / State Dept | 22 CFR 120-130 | Ongoing | AECA (22 U.S.C. 2778) | Defense articles and services |
| FERPA | Dept of Education | 34 CFR Part 99 | 1974 (amended) | FERPA (20 U.S.C. 1232g) | Education institutions receiving federal funds |
| SEC Cyber Rules | SEC | Final Rule | December 2023 | Securities Exchange Act | SEC registrants (public companies) |

### Voluntary and Best-Practice Frameworks

| Framework | Governing Body | Current Version | Published | Certification Available | Scope |
|---|---|---|---|---|---|
| NIST CSF | NIST | 2.0 | February 2024 | No | All organizations |
| ISO 27001 | ISO/IEC | 2022 | October 2022 | Yes (accredited CBs) | Any organization (ISMS) |
| SOC 2 | AICPA | TSC 2017 (updated) | Ongoing | SOC 2 report (attestation) | Service organizations |
| HITRUST CSF | HITRUST Alliance | v11 | 2023 | Yes (HITRUST assessors) | Multi-framework harmonization |
| CIS Controls | CIS | v8.1 | June 2024 | CIS Benchmarks | All organizations |
| CCPA/CPRA | California AG / CPPA | CPRA effective 2023 | January 2023 | No | Businesses meeting CA thresholds |
| GDPR | EU Commission | 2016/679 | May 2018 | No (but certifications exist) | EU personal data processors |

---

## Control Domain Overlap Matrix

This table shows which security domains each framework addresses:

| Security Domain | 800-53 | 800-171 | CMMC L2 | HIPAA | SOC 2 | ISO 27001 | PCI DSS | FedRAMP | CIS v8 | NIST CSF | HITRUST |
|---|---|---|---|---|---|---|---|---|---|---|---|
| Access Control | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
| Awareness & Training | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
| Audit & Accountability | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
| Security Assessment | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
| Configuration Management | Yes | Yes | Yes | Partial | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
| Contingency Planning | Yes | No | No | Yes | Yes | Yes | Partial | Yes | Partial | Yes | Yes |
| Identification & Authentication | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
| Incident Response | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
| Maintenance | Yes | Yes | Yes | Partial | Partial | Yes | Partial | Yes | Partial | Yes | Yes |
| Media Protection | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
| Physical Security | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
| Personnel Security | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Partial | Yes | Yes |
| Risk Assessment | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
| System & Comms Protection | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
| System Integrity | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
| Privacy | Yes | No | No | Yes | Yes | Yes | Partial | Yes | No | Yes | Yes |
| Supply Chain | Yes | No | No | No | Yes | Yes | Partial | Yes | Yes | Yes | Partial |
| Program Management | Yes | No | No | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
| Data Classification | Yes | Partial | Partial | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
| Vulnerability Management | Yes | Yes | Yes | Partial | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
| Encryption | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
| Change Management | Yes | Yes | Yes | Partial | Yes | Yes | Yes | Yes | Yes | Yes | Yes |
| **Domain Coverage** | **22/22** | **14/22** | **14/22** | **18/22** | **21/22** | **22/22** | **19/22** | **22/22** | **18/22** | **22/22** | **21/22** |

---

## Industry Applicability Matrix

| Industry | Primary Frameworks | Secondary Frameworks | Optional Best Practices |
|---|---|---|---|
| **Defense Contractors (CUI)** | CMMC L2, DFARS 7012, 800-171 | ITAR (if defense articles), NIST CSF | ISO 27001, SOC 2 |
| **Defense Contractors (FCI only)** | CMMC L1, FAR 52.204-21 | NIST CSF | CIS Controls |
| **Healthcare Providers** | HIPAA Security Rule | State health privacy laws | HITRUST, NIST CSF |
| **Healthcare SaaS** | HIPAA (BA), SOC 2 | HITRUST | FedRAMP (if federal health) |
| **Health Plans** | HIPAA Security Rule | State insurance regs | HITRUST, NIST CSF |
| **Banks & Credit Unions** | GLBA, FFIEC | SOX (if public), PCI DSS | ISO 27001, NIST CSF |
| **Non-Bank Financial** | GLBA/FTC Safeguards | State financial regs | SOC 2, NIST CSF |
| **Payment Processors** | PCI DSS | SOC 2 | ISO 27001 |
| **Federal Agencies** | FISMA, 800-53 | FedRAMP (cloud), CJIS (if CJI) | NIST CSF |
| **State/Local Government** | State security policies | StateRAMP, CJIS (if CJI) | NIST CSF, CIS Controls |
| **Cloud SaaS (Enterprise)** | SOC 2 | ISO 27001 | CSA STAR, NIST CSF |
| **Cloud SaaS (Government)** | FedRAMP | SOC 2, StateRAMP | ISO 27001 |
| **Public Companies** | SOX, SEC Cyber Rules | Industry-specific | SOC 2, ISO 27001 |
| **Education (K-12)** | FERPA | State student privacy | CIS Controls, NIST CSF |
| **Higher Education** | FERPA | GLBA (student financial aid) | NIST CSF, CIS Controls |
| **Law Enforcement IT** | CJIS Security Policy | FedRAMP/StateRAMP (cloud) | NIST CSF |
| **Tax Processing** | IRS Pub 1075 | GLBA | SOC 2, NIST CSF |
| **Defense Exporters** | ITAR | CMMC, EAR | ISO 27001 |
| **EU-Facing Business** | GDPR | Country DPA requirements | ISO 27001 |
| **CA-Facing Business** | CCPA/CPRA | Other state privacy laws | CIS Controls, SOC 2 |
| **Retail (with cards)** | PCI DSS | CCPA/CPRA (if CA customers) | CIS Controls |
| **Manufacturing (DoD)** | CMMC, ITAR (if applicable) | ISO 27001 | NIST CSF |
| **MSP/MSSP** | SOC 2 | Frameworks of served industries | ISO 27001, NIST CSF |

---

## Cost and Effort Matrix

### Initial Implementation Cost (SMB: 50-250 Employees)

| Framework | Technology | Consulting | Internal Labor | Assessment/Audit | Total Range |
|---|---|---|---|---|---|
| NIST CSF 2.0 | $5K-$15K | $10K-$25K | 80-200 hours | $15K-$30K | $15K-$50K |
| CIS Controls IG1 | $10K-$30K | $10K-$25K | 100-300 hours | Self-assessment | $20K-$75K |
| CMMC Level 1 | $2K-$5K | $3K-$8K | 40-80 hours | Self-assessment | $5K-$15K |
| CMMC Level 2 | $20K-$60K | $30K-$80K | 500-1,500 hours | $30K-$100K | $50K-$200K |
| HIPAA | $10K-$40K | $15K-$50K | 200-600 hours | $20K-$50K | $30K-$150K |
| SOC 2 Type II | $10K-$30K | $15K-$40K | 300-700 hours | $25K-$75K | $30K-$100K |
| ISO 27001 | $15K-$40K | $20K-$60K | 400-800 hours | $15K-$50K | $40K-$150K |
| PCI DSS (SAQ) | $5K-$15K | $10K-$20K | 100-300 hours | $5K-$20K | $20K-$50K |
| PCI DSS (QSA) | $30K-$100K | $40K-$100K | 500-1,000 hours | $50K-$200K | $100K-$500K |
| FedRAMP Moderate | $100K-$500K | $200K-$500K | 2,000-5,000 hours | $200K-$500K | $500K-$2M |
| HITRUST r2 | $15K-$50K | $25K-$75K | 400-1,000 hours | $30K-$100K | $50K-$200K |
| GLBA Safeguards | $10K-$30K | $10K-$30K | 150-400 hours | Regulator exam | $25K-$100K |
| GDPR Full Program | $20K-$100K | $30K-$200K | 500-2,000 hours | Varies | $50K-$500K |

### Annual Maintenance Cost

| Framework | Technology Ops | Ongoing Consulting | Internal Labor | Re-Assessment | Total Range |
|---|---|---|---|---|---|
| NIST CSF 2.0 | $3K-$10K | $5K-$10K | 40-100 hours | $5K-$15K | $10K-$25K |
| CMMC Level 1 | $1K-$3K | $2K-$5K | 20-40 hours | Self-assessment | $3K-$10K |
| CMMC Level 2 | $10K-$30K | $15K-$30K | 200-500 hours | $15K-$50K (triennial) | $25K-$75K |
| HIPAA | $5K-$15K | $10K-$25K | 100-300 hours | $10K-$25K | $15K-$50K |
| SOC 2 Type II | $8K-$20K | $10K-$25K | 150-400 hours | $25K-$75K | $20K-$60K |
| ISO 27001 | $8K-$20K | $10K-$25K | 150-400 hours | $10K-$30K (surveillance) | $20K-$60K |
| FedRAMP Moderate | $50K-$150K | $50K-$150K | 1,000-2,500 hours | $100K-$250K (ConMon) | $200K-$500K |

---

## Assessment and Certification Matrix

| Framework | Assessment Type | Assessor | Frequency | Duration | Output |
|---|---|---|---|---|---|
| NIST CSF 2.0 | Gap assessment | Self or consultant | Ad hoc | 2-4 weeks | Gap report + roadmap |
| CMMC Level 1 | Self-assessment | Internal team | Annual | 1-2 weeks | SPRS score + affirmation |
| CMMC Level 2 | Third-party assessment | C3PAO (CyberAB authorized) | Triennial | 4-8 weeks | CMMC certificate or conditional |
| CMMC Level 3 | Government assessment | DIBCAC | Triennial | 6-12 weeks | CMMC Level 3 status |
| HIPAA | Risk analysis + evaluation | Internal or consultant | Annual (best practice) | 4-8 weeks | Risk assessment report |
| SOC 2 Type I | Point-in-time | Licensed CPA firm | One-time | 4-6 weeks | SOC 2 Type I report |
| SOC 2 Type II | Period of time (6-12 months) | Licensed CPA firm | Annual | 6-12 months observation | SOC 2 Type II report |
| ISO 27001 | Stage 1 + Stage 2 | Accredited certification body | Triennial (annual surveillance) | 3-6 weeks | ISO 27001 certificate |
| PCI DSS (SAQ) | Self-assessment questionnaire | Internal (with ASV scans) | Annual | 2-4 weeks | Completed SAQ + AOC |
| PCI DSS (QSA) | On-site assessment | QSA company | Annual | 6-10 weeks | ROC + AOC |
| FedRAMP | Full security assessment | 3PAO | Initial + annual ConMon | 16-26 weeks | ATO package + P-ATO/Agency ATO |
| HITRUST r2 | Validated assessment | HITRUST authorized assessor | Biennial | 8-16 weeks | HITRUST r2 validated report |
| HITRUST i1 | Implemented assessment | HITRUST authorized assessor | Annual | 4-8 weeks | HITRUST i1 validated report |
| CIS Controls | Self-assessment | Internal team | Ad hoc | 1-3 weeks | CIS CSAT score |

---

## Enforcement and Penalties Matrix

| Framework | Enforcement Body | Max Penalty per Violation | Max Annual Penalty | Criminal Liability | Recent Notable Penalties |
|---|---|---|---|---|---|
| HIPAA | HHS OCR | $1,931,280 (2024 adjusted) | $1,931,280 per category | Yes (knowingly) | $4.75M (Banner Health, 2023) |
| PCI DSS | Card brands (Visa, MC, etc.) | $100,000/month | Unlimited + card brand fines | No | Varies by acquirer |
| GDPR | EU/EEA DPAs | 4% of global annual revenue | No explicit cap | Varies by country | $1.3B (Meta, 2023) |
| CCPA/CPRA | California AG / CPPA | $7,500 per intentional violation | No explicit cap | No | $1.2M (Sephora, 2022) |
| GLBA | FTC / banking regulators | Varies by regulator | Varies | Yes (financial fraud) | Varies |
| SOX | SEC / DOJ | $5M + 20 years (officers) | Varies | Yes | Varies |
| FISMA | OMB / agency IGs | Funding impact, IG findings | N/A | No | Agency reporting scores |
| FERPA | Dept of Education | Loss of federal funding | N/A | No | Funding investigations |
| ITAR | DDTC / DOJ | $1.3M civil / $1M criminal per violation | Debarment possible | Yes | $290M (Lockheed, historical) |
| CMMC | DoD (contract-level) | Contract loss / False Claims Act | Treble damages under FCA | Yes (FCA) | Pending (CMMC effective 2025) |
| SEC Cyber Rules | SEC | Varies | Varies | Yes (fraud) | $10M+ (SolarWinds investigation) |

---

## Framework-to-Framework Overlap Percentages

Estimated control overlap between major frameworks (percentage of Row framework satisfied by implementing Column framework):

| Implementing... | Satisfies 800-53 M | Satisfies 800-171 | Satisfies HIPAA | Satisfies SOC 2 | Satisfies ISO 27001 | Satisfies PCI DSS | Satisfies FedRAMP |
|---|---|---|---|---|---|---|---|
| **800-53 Moderate** | 100% | 95%+ | 85% | 80% | 75% | 60% | 70% |
| **800-171** | 52% | 100% | 50% | 55% | 45% | 40% | 45% |
| **HIPAA (full)** | 40% | 45% | 100% | 55% | 50% | 35% | 35% |
| **SOC 2 Type II** | 45% | 50% | 55% | 100% | 60% | 40% | 40% |
| **ISO 27001** | 50% | 55% | 55% | 65% | 100% | 45% | 45% |
| **PCI DSS 4.0** | 35% | 35% | 35% | 40% | 40% | 100% | 30% |
| **FedRAMP Moderate** | 95% | 95% | 85% | 80% | 75% | 60% | 100% |
| **HITRUST r2** | 70% | 75% | 90% | 75% | 70% | 55% | 65% |
| **NIST CSF 2.0** | 60% | 65% | 60% | 60% | 55% | 45% | 55% |
| **CIS Controls IG2** | 50% | 55% | 50% | 50% | 45% | 40% | 45% |

Key insight: **800-53 Moderate and FedRAMP Moderate provide the highest coverage across all other frameworks.** Organizations implementing either as their baseline satisfy 60-95% of every other framework.

---

## Comply Once, Satisfy Many Implementation Guide

### Phase 1: Foundation (Months 1-3)

Implement these 800-53 control families first, as they provide the broadest coverage across all frameworks:

| 800-53 Family | Frameworks Satisfied | Priority |
|---|---|---|
| AC (Access Control) | All 20+ frameworks | Critical |
| IA (Identification and Authentication) | All 20+ frameworks | Critical |
| AU (Audit and Accountability) | All 20+ frameworks | Critical |
| RA (Risk Assessment) | All 20+ frameworks | Critical |
| SC (System and Communications Protection) | All 20+ frameworks | Critical |

### Phase 2: Core Security (Months 3-6)

| 800-53 Family | Frameworks Satisfied | Priority |
|---|---|---|
| CM (Configuration Management) | 18+ frameworks | High |
| SI (System and Information Integrity) | 18+ frameworks | High |
| IR (Incident Response) | All 20+ frameworks | High |
| AT (Awareness and Training) | 18+ frameworks | High |
| PS (Personnel Security) | 16+ frameworks | High |

### Phase 3: Operational Security (Months 6-9)

| 800-53 Family | Frameworks Satisfied | Priority |
|---|---|---|
| PE (Physical and Environmental Protection) | 15+ frameworks | Medium |
| MP (Media Protection) | 14+ frameworks | Medium |
| MA (Maintenance) | 12+ frameworks | Medium |
| CA (Assessment, Authorization, Monitoring) | 14+ frameworks | Medium |
| CP (Contingency Planning) | 12+ frameworks | Medium |

### Phase 4: Governance and Specialization (Months 9-12)

| 800-53 Family | Frameworks Satisfied | Priority |
|---|---|---|
| PL (Planning) | 10+ frameworks | Medium |
| PM (Program Management) | 10+ frameworks | Medium |
| SA (System and Services Acquisition) | 12+ frameworks | Medium |
| SR (Supply Chain Risk Management) | 8+ frameworks | Medium |
| PT (PII Processing and Transparency) | Privacy frameworks | As applicable |

### After Foundation: Framework-Specific Gap Closure

Once the 800-53 Moderate baseline is implemented, close remaining gaps for each required framework:

| Target Framework | Remaining Gap After 800-53 | Effort to Close |
|---|---|---|
| CMMC Level 2 | Minimal; SSP documentation, SPRS submission | 2-4 weeks |
| HIPAA | BAA program, breach notification procedures, 6-year retention | 4-6 weeks |
| SOC 2 Type II | Observation period, audit report generation, service commitments | 3-6 months |
| ISO 27001 | ISMS documentation, management review, internal audit, certification audit | 3-6 months |
| PCI DSS | CDE scoping, ASV scanning, SAQ/ROC documentation, PAN-specific controls | 4-8 weeks |
| FedRAMP | Cloud-specific controls, ConMon, 3PAO assessment, POA&M | 6-12 months |
| GDPR | DPO appointment, DPIA process, data subject rights, cross-border transfers | 2-4 months |
| GLBA | Customer notice requirements, FTC-specific reporting | 2-4 weeks |

---

## Framework Retirement and Sunset Tracker

| Framework/Version | Status | Sunset Date | Replacement |
|---|---|---|---|
| 800-53 Rev. 4 | Superseded | September 2020 | 800-53 Rev. 5 |
| 800-171 Rev. 2 | Current (CMMC reference) | TBD (Rev. 3 published May 2024) | 800-171 Rev. 3 |
| CMMC 1.0 | Superseded | October 2024 | CMMC 2.0 |
| PCI DSS 3.2.1 | Superseded | March 2024 | PCI DSS 4.0 |
| ISO 27001:2013 | Transition period | October 2025 | ISO 27001:2022 |
| NIST CSF 1.1 | Superseded | February 2024 | NIST CSF 2.0 |
| HITRUST CSF v9 | Superseded | 2023 | HITRUST CSF v11 |
| CIS Controls v7 | Superseded | 2021 | CIS Controls v8 |

---

## Sources

- [NIST SP 800-53 Rev. 5](https://csrc.nist.gov/publications/detail/sp/800-53/rev-5/final)
- [NIST SP 800-171 Rev. 2](https://csrc.nist.gov/publications/detail/sp/800-171/rev-2/final)
- [NIST CSF 2.0](https://csrc.nist.gov/publications/detail/nistir/8286/final)
- [32 CFR Part 170 (CMMC)](https://www.ecfr.gov/current/title-32/subtitle-A/chapter-I/subchapter-D/part-170)
- [45 CFR Part 164 (HIPAA)](https://www.ecfr.gov/current/title-45/subtitle-A/subchapter-C/part-164)
- [PCI DSS 4.0](https://www.pcisecuritystandards.org/document_library/)
- [ISO/IEC 27001:2022](https://www.iso.org/standard/27001)
- [AICPA SOC 2 TSC](https://www.aicpa.org/interestareas/frc/assuranceadvisoryservices/trustservicescriteria.html)
- [FedRAMP Baselines](https://www.fedramp.gov/baselines/)
- [HITRUST CSF](https://hitrustalliance.net/csf/)
- [CIS Controls v8](https://www.cisecurity.org/controls/v8)
- [GDPR (2016/679)](https://eur-lex.europa.eu/eli/reg/2016/679/oj)
- [CCPA/CPRA](https://oag.ca.gov/privacy/ccpa)
- [GLBA FTC Safeguards Rule](https://www.ftc.gov/legal-library/browse/rules/safeguards-rule)
- [SEC Cybersecurity Disclosure Rules](https://www.sec.gov/rules/final/2023/33-11216.pdf)

---

Maintained by [Petronella Technology Group, Inc.](https://petronellatech.com) | Call 919-348-4912 for multi-framework compliance assessment
