# Digital Installment Loan – Hansebank

Requirements analysis for digitalizing the installment loan process of a fictional regional bank – from the starting situation through process and customer journey analysis to implementation-ready user stories and KPI analysis.

## Starting situation

Hansebank currently grants installment loans to retail customers almost exclusively through its branches:

- The customer books an appointment and fills out a paper application.
- Proof of income is copied and entered manually.
- Case workers trigger the SCHUFA credit bureau query and the creditworthiness check manually.
- It takes about **5 working days** on average to reach a credit decision.

Consequences: customers move to direct banks that offer instant approval, case workers are tied up with routine cases, and media breaks lead to data entry errors.

## Goals

| Goal | Today | Target |
|---|---|---|
| Time to (pre-)decision | approx. 5 working days | **under 10 minutes** for standard cases |
| Drop-out rate in the application process | not measured | **under 30%**, measurable per step |
| Manually processed applications | 100% | **max. 30%** (special cases only) |

## Stakeholders

| Stakeholder | Interest | Role in the project |
|---|---|---|
| Retail customer | Fast, simple application without a branch visit | End user, input through interviews and journey |
| Loan case processing | Fewer routine cases, complete application data | Domain expert, approval of processes |
| Risk management | Control credit risk, steer decision rules | Provides scoring and decision rules |
| Compliance / data protection | Compliance with MaRisk, GDPR and consumer credit law | Reviews requirements, sign-off |
| Product Owner (retail banking) | Market share, customer satisfaction | Prioritizes the backlog |
| IT / development team | Clear, actionable requirements and interfaces | Implementation, story estimation |

## Scope

**In scope**
- Installment loans for retail customers up to €50,000
- Online application journey (web, mobile-friendly)
- Automatic pre-check including SCHUFA query and preliminary decision
- Forwarding of special cases to case processing

**Out of scope**
- Mortgage financing and business loans
- Payout and contract management after closing
- Changes to the core banking system

## Approach & artifacts

| Artifact | Content | File |
|---|---|---|
| Process model (BPMN) | As-is and to-be process with marked weak points | [diagramme/](diagramme/) |
| Customer journey map | Phases, touchpoints, pain points from the customer's view | [diagramme/](diagramme/) |
| Epics & user stories | Requirements with acceptance criteria (Given/When/Then) | [docs/](docs/) |
| KPI analysis (SQL) | Metrics based on the public German Credit dataset | [sql/](sql/) |

Data basis: [Statlog (German Credit Data)](https://archive.ics.uci.edu/dataset/144/statlog+german+credit+data), UCI Machine Learning Repository – 1,000 anonymized credit applications from a German bank.

## Next steps

- Elaborate the SCHUFA interface as an API specification (OpenAPI)
- Model the pre-check flow as a UML sequence diagram
- Document the risk management decision rules as a decision table (DMN)
- Test a clickable prototype of the application journey with users
