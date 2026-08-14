# Workflow Patterns

Use these patterns to build phase-out operating plans.

## Standard Phase-Out Lanes

1. **Governance**
   Decision brief, scope approval, phase-out classification, steering cadence, decision log, closure approval.

2. **Regulatory and quality**
   Regulatory assessment, recall/correction/removal screen, jurisdictional notification assessment, QMS linkage, document control, PMS/vigilance review, CAPA/complaint review.

3. **Installed base and customer transition**
   Customer inventory, active-device reconciliation, contract/warranty review, clinical criticality segmentation, replacement eligibility, exceptions, transition schedule.

4. **Operations and supply**
   Last-time-buy, last manufacture, last ship, inventory disposition, spare parts, supplier commitments, repair depot readiness, service tools, calibration, labeling, controlled destruction.

5. **Cybersecurity and software**
   Supported versions, vulnerability monitoring, patch strategy, compensating controls, remote access, SBOM exposure, end-of-support notices, residual risk acceptance.

6. **Commercial and finance**
   Revenue impact, customer retention, pricing, replacement offers, sales enablement, distributor plans, write-offs, reserves, margin impact.

7. **Communications and training**
   Internal briefings, sales/service scripts, customer letters, distributor instructions, clinician/patient communications where applicable, training for migration or decommissioning.

8. **Closure**
   Completion metrics, unresolved exceptions, evidence binder, final approvals, archive, post-closure monitoring.

## Milestone Skeleton

| Phase | Milestone | Typical Owner | Evidence |
| --- | --- | --- | --- |
| Initiate | Phase-out request and rationale | Product | Decision brief |
| Assess | Regulatory/quality classification | Regulatory + Quality | Assessment memo |
| Assess | Installed-base reconciliation | Service + Commercial Ops | Affected customer/device list |
| Plan | Phase-out roadmap approval | Product + Steering Team | Approved roadmap |
| Prepare | Replacement/exception paths | Product + Commercial + Service | Migration plan |
| Prepare | Communication approvals | Legal + Regulatory + Quality | Approved notices |
| Execute | Last order / last ship / end service milestones | Operations + Service | ERP/service records |
| Monitor | Complaints, vigilance, cyber, exceptions | Quality + Cybersecurity | Monitoring log |
| Close | Evidence binder and closure approval | Quality + Product | Closure report |

## RACI Defaults

- **Product**: Accountable for business rationale, lifecycle roadmap, replacement strategy, scope, and cross-functional tradeoffs.
- **Regulatory affairs**: Accountable for jurisdictional assessment, authority/notified-body interactions, labeling implications, and notification strategy.
- **Quality**: Accountable for QMS linkage, risk management file updates, CAPA/complaint review, evidence binder, and closure readiness.
- **Clinical/safety**: Consulted on clinical dependency, patient risk, use interruption, and risk-benefit questions.
- **Cybersecurity/software**: Accountable for vulnerability lifecycle, software support commitments, patching, SBOM, and residual cyber risk.
- **Service**: Responsible for installed-base data, service dates, spare parts, repair capacity, decommissioning, and customer site execution.
- **Supply chain/manufacturing**: Responsible for last-time-buy, supplier exits, inventory, tooling, manufacturing shutdown, and disposition.
- **Commercial/customer success**: Responsible for customer segmentation, account plans, retention risk, and external communication execution.
- **Legal/contracts**: Consulted or accountable for contractual obligations, liability exposure, and approved customer language.
- **Document control**: Responsible for records, approvals, templates, and archive.

## Risk Controls To Include

- Stage gates before external communication, last order, last ship, end service, and closure.
- No end-service date until replacement/exception handling is defined for clinically critical customers.
- Separate escalation for potential correction/removal/recall/FSCA classification.
- Explicit cybersecurity residual-risk acceptance when support ends before all devices are retired.
- Customer communication tracking with acknowledgement status for high-risk devices.
- Exception log for customers, jurisdictions, contracts, or devices outside the standard path.
