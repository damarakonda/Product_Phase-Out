---
name: medtech-phase-out
description: "Create end-to-end product phase-out plans for MedTech and medical device products. Use when planning end-of-sale, end-of-manufacture, end-of-service, discontinuance, installed-base transition, replacement migration, spare-parts wind-down, software or cybersecurity end-of-support, regulatory notification planning, customer communication, evidence binders, RACI, or cross-functional phase-out governance for regulated medical devices, IVDs, SaMD, connected devices, accessories, or device software."
---

# MedTech Phase-Out

## Overview

Use this skill to turn a MedTech product retirement or discontinuance scenario into a controlled, auditable phase-out package. Optimize for patient safety, regulatory and quality obligations, installed-base continuity, cybersecurity support, customer transition, and evidence traceability.

This skill is planning support, not legal, regulatory, or clinical advice. Flag jurisdiction-specific assumptions and tell the user when regulatory affairs, legal, clinical safety, cybersecurity, or quality owners must confirm a decision.

## Quick Workflow

1. **Clarify scope**
   Capture product family, model/version, device type, jurisdiction, lifecycle event, phase-out reason, target dates, replacement path, installed-base size, and open quality/regulatory issues.

2. **Classify the phase-out**
   Distinguish commercial retirement, market withdrawal, planned discontinuance, end-of-service, spare-parts wind-down, software end-of-support, field correction/removal, recall-adjacent action, or supply interruption. If recall/correction/removal may be implicated, treat it as an escalation and avoid presenting the plan as routine phase-out.

3. **Map obligations**
   Identify likely regulatory, quality, service, supply, cybersecurity, contractual, and customer communication obligations. Load `references/regulatory-context.md` when the task involves jurisdictions, notification duties, recalls, field actions, PMS/vigilance, or cybersecurity.

4. **Build the operating plan**
   Produce milestones, owners, dependencies, decision gates, evidence artifacts, and escalation criteria. Load `references/workflow-patterns.md` for standard milestone models, RACI patterns, and risk controls.

5. **Create deliverables**
   Generate the requested package: phase-out charter, intake checklist, roadmap, RACI, risk register, communications matrix, installed-base transition plan, cybersecurity support plan, evidence binder, or executive brief. Load `references/artifact-templates.md` for output structures.

6. **List assumptions and tests**
   End with open decisions, assumptions to validate, required owner approvals, and data gaps that could change the plan.

## Intake Questions

Ask only for missing details that materially change the plan. If the user wants speed, proceed with clearly stated assumptions.

Minimum useful inputs:
- Product name/family, model, version, UDI/product code if known.
- Device type: capital equipment, consumable, implantable, IVD, SaMD, connected device, accessory, service part, or software module.
- Jurisdictions and markets in scope.
- Phase-out trigger: obsolescence, replacement launch, supplier issue, low demand, cybersecurity risk, quality issue, regulatory change, merger integration, cost, or strategic portfolio cleanup.
- Intended lifecycle dates: last order, last ship, end manufacture, end installation, end service, end spare-parts support, end software support.
- Installed-base data: customers, units, geographies, software versions, contracts, warranties, critical clinical uses.
- Open complaints, CAPAs, recalls, field actions, vigilance signals, cybersecurity vulnerabilities, regulatory commitments, or supply constraints.

## Output Standards

Always make outputs auditable and action-oriented:
- Use tables for milestones, RACI, risk registers, evidence binders, and communication matrices.
- Separate facts, assumptions, recommendations, and decisions needed.
- Include named owners by function when individual names are unknown.
- Include evidence artifacts for every major decision or milestone.
- Include escalation triggers for safety, quality, regulatory, cybersecurity, supply, customer, and contractual risks.
- Avoid claiming that a notification is or is not legally required unless source facts are complete; say what must be evaluated.

## Default Deliverable Set

When the user asks for an end-to-end plan without specifying format, produce:

1. **Phase-out charter**
   Objective, scope, exclusions, phase-out type, reason, products affected, markets affected, target dates, decision owners.

2. **Installed-base impact summary**
   Affected customers, devices, versions, accessories, service parts, software, critical-use segments, and replacement/exception paths.

3. **Risk-ranked roadmap**
   Milestones from decision through closure, with owner, due date, dependency, evidence, and risk level.

4. **RACI**
   Product, regulatory, quality, clinical/safety, service, supply chain, manufacturing, cybersecurity, legal, commercial, customer success, finance, and document control.

5. **Risk and control register**
   Patient safety, supply continuity, complaint/CAPA linkage, regulator notification, recall adjacency, cybersecurity, spare parts, contract commitments, training, customer downtime, revenue, and reputation.

6. **Communication matrix**
   Internal teams, distributors, direct customers, clinicians, patients where applicable, regulators/competent authorities/notified bodies where applicable, service partners, and replacement-product teams.

7. **Evidence binder outline**
   Documents, approvals, meeting records, risk assessments, regulatory assessments, customer communications, service plans, training artifacts, and closure evidence.

8. **Open assumptions**
   Data gaps, decisions needed, accountable approvers, and validation tasks.

## MedTech-Specific Heuristics

- Installed-base risk usually matters more than catalog status. Ask how many units remain active, where they are used, and what happens clinically if support stops.
- Treat software and cybersecurity support as their own phase-out lane. End-of-service may not be acceptable if vulnerabilities, patches, remote connectivity, or SBOM exposure remain unmanaged.
- Do not collapse market withdrawal, discontinuance, correction/removal, field safety corrective action, and recall into one label. Classify carefully and escalate ambiguity.
- Include spare parts, accessories, consumables, calibration tools, service tools, labeling, IFUs, training, and validation support when relevant.
- Tie every customer-facing date to operational readiness: replacement availability, inventory, service capacity, training, contracting, and regulatory status of the replacement product.
- Preserve traceability to QMS records, design history, device master records, complaint handling, CAPA, PMS/PMCF, vigilance, supplier records, cybersecurity records, and document control where applicable.

## Reference Routing

- Read `references/regulatory-context.md` for regulatory, recall, field action, PMS/vigilance, discontinuance, supply interruption, or cybersecurity lifecycle questions.
- Read `references/workflow-patterns.md` to build an end-to-end roadmap, governance plan, risk controls, or RACI.
- Read `references/artifact-templates.md` when producing a phase-out charter, risk register, communication matrix, evidence binder, or executive-ready deliverable.

## Execution and closure

For end-to-end requests, read [execution-controls.md](references/execution-controls.md) and include decision gates, supply/service assumptions, a transition tracker, and continuing obligations in the deliverable package. For a narrow request, produce only the relevant artifacts.

Start by reading supplied project records and identifying their revision and approval status. Maintain source links for facts; label unverified values as unknown. Do not invent dates, customer counts, approvals, regulatory determinations, or completed actions. A requested target date is not an approved commitment.

Use one accountable function per milestone and distinguish proposed, ready for review, approved, executing, blocked, and complete. Complete means evidence exists, not merely that a due date has passed. Record approval authority, date, scope, and evidence reference when supplied; otherwise leave approval pending.

When updating a plan, preserve stable record IDs, compare against the previous baseline, and explain changes to scope, dates, obligations, risks, and dependencies. Reassess affected gates when assumptions change. Planning does not authorize sending notices, submitting regulatory reports, placing orders, disabling systems, or retiring devices.

Verify current primary regulatory sources for the affected markets before making a jurisdiction-specific determination. Capture applicability facts and Regulatory Affairs review; the reference file is a routing aid, not an exhaustive statement of current law.
