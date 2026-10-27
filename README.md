# Google Workspace & Microsoft 365 Security Audit Framework

An Excel-based security assessment framework for reviewing cloud configurations, documenting control gaps, and planning alerts for Google Workspace and Microsoft 365.

This project brings together **58 security controls** and **27 alert scenarios**, supported by screenshot walkthroughs for selected configurations. It is designed for GRC analysts and administrators who need a structured way to compare tenant settings with a defined baseline, record evidence, and prioritize remediation.

## Project objectives

- Prioritize security configurations by their proposed impact on preventing attacks and limiting exposure.
- Provide specific administrative steps for validating each control.
- Record expected settings, assessment results, and evidence references.
- Identify incident alerts and changes that diverge from the security baseline.
- Summarize assessment progress and findings through workbook scorecards.

## Included resources

| File | Contents |
| --- | --- |
| `GWS_Security_Audit_Guide.xlsx` | 25 Google Workspace controls, 12 alert scenarios, an assessment scorecard, and a priority key |
| `GWS_Security_Audit_Guide Screenshot.pdf` | Screenshot walkthroughs for selected Google Workspace controls |
| `M365_Security_Audit_Guide.xlsx` | 33 Microsoft 365 controls, 15 alert scenarios, an assessment scorecard, an admin portal map, and a priority key |
| `M365_Security_Audit_Guide Screenshot.pdf` | Screenshot walkthroughs for selected Microsoft 365 controls |

## Security coverage

### Google Workspace

The guide covers multifactor authentication, privileged access, OAuth and third-party applications, Gmail protections, email authentication, endpoint management, Drive sharing, forwarding, data loss prevention, audit visibility, offboarding, and retention.

### Microsoft 365

The guide covers Microsoft Entra ID authentication and Conditional Access, privileged identity management, application consent, Defender email and endpoint protections, Exchange forwarding, SharePoint and OneDrive sharing, Teams access, Intune device compliance, Purview data protection, audit logging, lifecycle management, and recovery.

## Workbook structure

- **README:** Purpose, usage instructions, access requirements, and assessment context.
- **Controls:** Control IDs, priorities, security domains, risk rationale, validation steps, expected baseline states, PASS/FAIL/NA results, and evidence references.
- **Alerts:** Linked controls, trigger conditions, incident or baseline-divergence classifications, configuration guidance, recommended responses, and configured-status fields.
- **Scorecard:** Assessment totals and result summaries.
- **Priority Key:** Priority definitions and suggested review cadences.
- **Portal Map:** Microsoft 365 administrative portal references, included in the Microsoft 365 workbook.

## How to use

1. Download the workbook for the platform being assessed and save a working copy.
2. Review its README, required permissions, and licensing notes.
3. Start with P1 controls and continue through the remaining priorities.
4. Follow the validation steps and compare effective settings with the expected baseline. Use the screenshot PDFs as supporting navigation examples.
5. Record PASS, FAIL, or NA and an evidence reference for each control. Document the reason for NA and any licensing limitations.
6. Review linked alert scenarios, confirm available detection options, and record whether the alerts are configured.
7. Use the scorecard to review progress and create a remediation plan for failed controls.

## Priority levels

| Priority | Tier | Suggested review cadence |
| --- | --- | --- |
| P1 | Critical | Monthly and after relevant changes |
| P2 | High | Quarterly |
| P3 | Medium | Semiannually |
| P4 | Foundational | Semiannually |

These priorities and cadences reflect the guides' assessment approach. Adapt them to the organization's risks, operating requirements, and approved exceptions.

## Assessment scope and evidence

This repository provides assessment documentation and configuration walkthroughs. It does not automatically scan tenants, deploy security policies, or create alerts. Screenshots illustrate selected settings and do not establish that every control is implemented or effective.

Administrative menus, event names, permissions, and licensed features can change. Confirm current product behavior before applying settings or relying on a detection rule. Store real tenant evidence in an approved private location and sanitize examples before publishing them.
