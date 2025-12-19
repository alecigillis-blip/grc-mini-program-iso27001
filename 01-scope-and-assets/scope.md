Compliance Program Overview – NimbusPay (Fintech SaaS on Azure)
Scope & Context
NimbusPay is a fictional fintech SaaS startup providing digital wallet and instant payment services. The environment is hosted entirely on Microsoft Azure, with assets including Azure AD (identity), Azure SQL Database (transaction data), Azure Blob Storage (documents/logs), Azure Key Vault (secrets), Azure App Service (front-end), and Azure Functions (payment microservices). Endpoints are Intune-managed Windows 11 laptops. Data types handled: Personally Identifiable Information (PII), PCI data (card tokens), financial transaction logs, and audit records. Users: Developers, support staff, compliance officers, and external customers.
Framework & Approach
The compliance program is aligned to ISO 27001 Annex A controls, chosen for its audit-ready structure and relevance to fintech SaaS environments. Controls were selected based on risk to sensitive financial data, cloud-native architecture, and regulatory expectations (PCI DSS, SOC 2).
Current Maturity
Strengths:
Multi-factor authentication enforced via Azure AD Conditional Access.
Encryption at rest (Transparent Data Encryption in SQL, Key Vault-managed keys) and in transit (TLS 1.2+).
Asset inventory managed through Intune and Azure Resource Graph.
Developing areas:
Incident response plan drafted but not yet tested.
Supplier security assessments not formalized.
Secure SDLC practices partially integrated (basic code reviews, limited automated scanning).
Gaps:
Centralized logging and monitoring not yet deployed.
Formal quarterly access reviews missing.
Vendor due diligence process absent.
Gap Remediation Roadmap
30 Days:
Finalize and approve Information Security Policy.
Establish quarterly access review process in Azure AD.
60 Days:
Deploy Azure Sentinel SIEM for centralized logging and monitoring.
Conduct first incident response tabletop exercise.
90 Days:
Implement vendor risk assessment checklist and review critical suppliers.
Integrate SAST/DAST tools into CI/CD pipeline for secure SDLC.
