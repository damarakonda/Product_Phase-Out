# Execution controls

Use these controls to extend the repository's workflow into an executable phase-out package. Tailor gates to the product and company QMS; these are planning defaults, not statutory gates.

## Decision gates

| Gate | Evidence required to recommend release | Accountable function | If incomplete |
| --- | --- | --- | --- |
| Scope and classification | Product/market/version scope, rationale, installed-base confidence, safety/field-action screen | Product; separate Regulatory Affairs classification decision | Preserve unknowns; route safety concerns to Quality/Regulatory Affairs |
| Plan baseline | Market obligation assessment, contracts, risk controls, replacement feasibility, funded support, owners and dependencies | Program sponsor | Keep dates provisional and identify decision needed |
| Communication readiness | Reviewed market-specific notice, operationally feasible dates, recipient list, distribution and follow-up plan | Commercial; regulatory notices remain Regulatory Affairs owned | Hold discretionary announcement; escalate any mandatory notification deadline independently |
| Last order/manufacture/ship | Order backlog disposition, inventory allocation, supplier commitments, service stock, market constraints | Operations | Replan the affected milestone and downstream dates |
| End service/software support | Critical customer transition or approved exception, contracts addressed, residual safety/cyber controls, support handover | Service; software support decision owned by Software | Keep affected population open and escalate gaps |
| Program closure | Device/customer outcomes reconciled, exceptions transferred with owners, financial disposition, evidence index and continuing duties accepted | Program sponsor | Partial closure only with explicit scope and unresolved items |

Assess each lifecycle date separately; end-of-sale does not imply end-of-service. Record each gate decision independently where multiple functions own different decisions. Do not use gate review to delay urgent safety or mandatory reporting work.

## Supply, spares and funding

Calculate by SKU, location and time period using documented assumptions. Keep saleable stock, service stock, quarantined units, expired units and allocated stock distinct.

- Gross requirement = expected demand through the support horizon + approved safety stock + other commitments not already counted in demand.
- Net purchase requirement = max(0, gross requirement − usable unallocated inventory − confirmed usable inbound supply). Adjust for validated yield, minimum order quantities, shelf life and supplier lead time; show each adjustment.
- Service demand = sum of active units in each period × estimated failures per unit per period × parts required per failure. Add planned maintenance separately. Deduct repair recoveries only where turnaround and yield are supported by data.
- Forecast low/base/high cases for retirement speed, failure rate, repair yield and lead time. Show the first projected stockout and the decisions needed before supplier exit.
- Separate cash spending, inventory write-offs, accounting provisions and lost revenue to avoid double counting. Finance confirms accounting treatment and funding.

If inputs are missing, provide formulas and required inputs instead of numerical estimates presented as facts. For consumables, consider usage rate and shelf life; for implants, ongoing patient follow-up; for IVDs, reagent/calibrator/control compatibility; for software, infrastructure and security support dependencies.

## Execution records

Use stable IDs and evidence links. Expand these schemas into tables only when relevant.

| Record | Minimum fields |
| --- | --- |
| Milestone | ID, product/market, event, proposed date, approved date, dependency IDs, responsible owner, accountable owner, status, gate, evidence |
| Installed base | Device or aggregated cohort ID, model/version, market, source/as-of date, active/retired/unknown status, clinical dependency, contract end, transition path, owner, completion evidence |
| Transition | ID, customer/site or pseudonymous cohort, affected count, replacement availability and market status, compatibility/validation, training, scheduled date, acceptance evidence, remaining count |
| Obligation | ID, jurisdiction, trigger facts, source/version/access date, applicability conclusion or unknown, deadline and basis, owner, review evidence, submission/acknowledgement evidence |
| Exception | ID, affected devices/customers, reason, risk, interim controls, owner, approver, expiry/review date, exit condition, evidence |
| Decision | ID, question, options, recommendation, decision owner, decision status/date, rationale, affected records, evidence |
| Continuing duty | ID, activity, scope, receiving owner, funding, cadence/next date, applicable retention or reporting basis, handover acceptance |

Store only the personal/customer data necessary for the requested output. Link controlled records rather than copying patient data into planning files.

## Monitoring and closure

Define denominator, as-of date, target and accountable owner for each metric. Useful metrics include reconciled units / in-scope units, transitioned units / units requiring transition, delivered notices / intended recipients, acknowledged notices / recipients requiring acknowledgement, overdue high-risk exceptions, projected stockouts, and overdue gate evidence. Do not count unknown device status as retired or infer acknowledgement from delivery.

Reconcile initial scope plus approved additions minus approved exclusions against transitioned, decommissioned, supported-by-exception and unresolved populations; investigate discrepancies and prevent double counting. Decommissioning evidence may include device disposition, data handling, site acceptance, account/access closure and environmental handling as applicable.

Closure transfers ongoing complaint handling, vigilance/PMS, cybersecurity monitoring, contractual support and record retention to named owners where those duties continue. Document applicable retention basis rather than inventing one universal period. An archive is not proof that obligations have ended. Unaccepted high-risk exceptions keep the affected scope open.

## Behavioral checks

Before delivering, check these failure cases against the plan:

- No installed-base data: use an unresolved cohort and reconciliation action; do not declare closure.
- Vulnerability-driven retirement: initiate safety/regulatory assessment; do not classify as ordinary commercial retirement by assumption.
- Replacement available in one country only: separate market milestones and exception paths.
- Support target earlier than contract expiry: surface the conflict and an owned resolution; do not silently overwrite either date.
- Regulatory notification due before communication readiness: escalate and preserve the applicable reporting timeline.
- Supplier last buy precedes forecast completion: surface a decision deadline and scenarios; do not invent a safe purchase quantity.
