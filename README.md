# Risk Assessment & Standards — Microsoft Entra Connect

**Module:** Risk Assessment and Standards  
**Programme:** MSc Cybersecurity — University College Dublin  
**Framework:** NIST SP 800-53 (Rev. 5, September 2020)  
**System Under Assessment:** Microsoft Entra Connect (Hybrid Identity Infrastructure)

---

## Project Overview

This project delivers a security assessment of a hybrid identity environment built around **Microsoft Entra Connect**, the service that bridges on-premises Active Directory with Microsoft Entra ID (formerly Azure AD). The work applies the NIST SP 800-53 control framework to a realistic enterprise scenario, producing two core deliverables:

| Deliverable | Description |
|---|---|
| `Microsoft_Entra_Connect-800-53_Controls.docx` | Full control implementation assessment across AC, SC, CM, AU, and IR families |
| `Microsoft_Entra_Connect-SSP_Part2.xlsx` | System Security Plan (SSP) — system identification, environment, information types, applicable laws, and audit controls |

---

## Control Families Covered

### DOCX — Security Controls Document

- **AC — Access Control** (25 controls): Account management, RBAC, least privilege, remote access, session management
- **SC — System & Communications Protection**: Boundary protection, TLS enforcement, cryptographic controls
- **CM — Configuration Management**: Baseline configuration, change control, inventory, least functionality
- **AU — Audit & Accountability**: Event logging, log retention, timestamps, audit protection
- **IR — Incident Response**: IR policy, training, testing, handling, monitoring, reporting

Each control entry documents:
1. Control ID and NIST description summary
2. Implementation status (Implemented / Partially Implemented / Not Implemented)
3. Required vs Optional classification
4. Scoping guidance (Increase / Decrease / Aligned)
5. Rationale specific to the Entra Connect deployment

### XLSX — System Security Plan

- **System Identification**: System owner, CISO contact, operational status, user counts
- **Environment**: Information types with CIA ratings, network port inventory
- **Laws & Standards**: GDPR, NIS 2, ISO/IEC 27001, PCI DSS, and others
- **Audit & Accountability**: AU control family summary (AU-1 through AU-12)
- **NIST 800-53 AU Compliance**: Audit preparation checklist with evidence requirements and responsible roles

---

## Key Technical Highlights

- Applied NIST 800-53 **tailoring guidance** — identified controls where the hybrid cloud context warrants increased or decreased scope
- Documented **risk acceptance decisions** (e.g., SC-12 cryptographic key management delegated to Microsoft infrastructure)
- Mapped information types to **NIST SP 800-60** identifiers with CIA impact ratings (High/Moderate/Low)
- Assessed **partial implementations** with specific remediation paths (e.g., AC-5 Separation of Duties, AC-20 External Systems)
- Aligned the SSP to **FedRAMP Moderate Baseline** template structure and **CMMC 2.0** requirements

---

## Framework References

- [NIST SP 800-53 Rev. 5](https://csrc.nist.gov/publications/detail/sp/800-53/rev-5/final) — Security and Privacy Controls
- [NIST SP 800-18 Rev. 1](https://csrc.nist.gov/publications/detail/sp/800-18/rev-1/final) — Guide for Developing Security Plans
- [NIST SP 800-60 Vol. 1](https://csrc.nist.gov/publications/detail/sp/800-60/vol-1/rev-1/final) — Information Types
- [FedRAMP SSP Templates](https://www.fedramp.gov/templates/)
- [Microsoft Entra Connect Documentation](https://learn.microsoft.com/en-us/entra/identity/hybrid/connect/whatis-azure-ad-connect)
