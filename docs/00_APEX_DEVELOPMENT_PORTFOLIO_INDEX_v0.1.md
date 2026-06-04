# APEX Development Portfolio — Visible Workstream Index v0.1
## Based on the Current APEX Development Mind Map

| Field | Value |
|---|---|
| Parent Control Repository | `apex-mirror-control-plane` |
| Portfolio Name | `APEX Development` |
| Source View | Current six-node development mind map supplied by Otto |
| Status | `PORTFOLIO FRAMEWORK FOUNDATION / PUBLIC-SAFE DESIGN` |
| Core Rule | Each module must have a purpose, features, evidence gates, interface contracts, maturity state and Final Direction Stack. |

## Truth Boundary

This document formalizes the visible development portfolio and assigns build roles. It does not claim all named modules are already implemented, validated or independently repository-backed. A module becomes operational only when its artifacts, tests and evidence support that claim.

## The Six Visible Development Workstreams

```text
                              APEX DEVELOPMENT
                                     │
        ┌────────────────────────────┼────────────────────────────┐
        │                            │                            │
APEX Perfect Analysis       APEX PhD Research         APEX Dimensions & Fields
Analysis / decision          Research / evidence       Universal model / ontology
intelligence                 intelligence              and dimensional mapping
        │                            │                            │
        └────────────────────────────┼────────────────────────────┘
                                     │
        ┌────────────────────────────┼────────────────────────────┐
        │                            │                            │
APEX Learning Center     APEX Analytics Mirror Module     APEX Test Workbench
Learning / capability    Business-facing analytics        Validation / stress /
proof laboratory         and governance experience        promotion control
```

## Portfolio Role Matrix

| Module | Purpose | Primary Deliverable | Current Repository Status | First Proof-Bearing Target |
|---|---|---|---|---|
| **APEX Perfect Analysis** | Analyze vision, current truth, gaps, risks, opportunities, payoff and next-best direction. | Governed analysis model and decision output schema. | `PROPOSED` — not yet assigned a dedicated repo. | Apply analysis framework to one existing APEX module and compare decision usefulness. |
| **APEX PhD Research** | Gather, grade, synthesize and route credible research into build requirements and evidence-linked cases. | Evidence-to-requirement research pipeline. | `PROPOSED` — not yet assigned a dedicated repo. | Produce one source-graded research packet with linked design implications. |
| **APEX Dimensions & Fields** | Define the universal dimensional ontology and modeling-depth framework for entities, behavior, constraints, prediction and governance. | Dimensional ontology and mapping specification. | `PROPOSED` — not yet assigned a dedicated repo. | Normalize one module into dimensional definitions without overclaiming physical dimensions. |
| **APEX Learning Center** | Measure and improve learning through targets, baselines, practice, transfer, governance and evolution. | Learning Compass, KPI schema and human/AI pilot. | `REPOSITORY EXISTS` — `apex-learning-center`. | `PILOT-001`: Human-only vs AI-only vs Human+AI comparison. |
| **APEX Analytics Mirror Module** | Build a Centralized Analytics SharePoint-style command center for data governance and analytics. | Interactive application prototype and SharePoint implementation spec. | `REPOSITORY EXISTS` — `apex-analytics-mirror-sharepoint`. | Upgrade prototype to evidence-labelled, graph-rich, selectable-layout application. |
| **APEX Test Workbench** | Run test cases, adversarial challenges, GUNMOS reviews, digital twins and promotion decisions. | Cross-module validation workbench and test runner. | `PROPOSED` — potential future dedicated repo. | Execute one test package against one bounded module artifact with evidence receipt. |

## Shared Development Lifecycle for Every Visible Module

```text
0. Purpose & Truth Boundary
→ 1. Current-State Inventory
→ 2. Requirements & Feature Register
→ 3. Architecture / Schema / UI Specification
→ 4. Build Artifact or Prototype
→ 5. Validation / Test / Evidence Receipt
→ 6. Promotion, Hold, Rollback or Refurbish Decision
→ 7. Measured Outcome / Benefit Review
→ 8. Iteration and Final Direction Stack Recalculation
```

## Standard Module Artifact Package

Each module must ultimately contain the following public-safe or controlled equivalent artifacts:

| Artifact ID | Artifact | Purpose |
|---:|---|---|
| `00` | Module Index / Charter | Identity, purpose, boundary, owners and status. |
| `01` | Product & Technical Specification | Requirements, architecture, user flows, data and integrations. |
| `02` | Build Prompt / Execution Packet | Self-contained handoff for implementation. |
| `03` | Feature Register & Acceptance Gates | Features, priority, tests and completion rules. |
| `04` | Interface / Integration Contract | Inputs, outputs, APIs/events and dependencies. |
| `05` | Risk & Opportunity Register | Failure modes, constraints, mitigations and innovation candidates. |
| `06` | Quality & Test Plan | Tests, pass/fail criteria, rollback and validation process. |
| `07` | Evidence Receipt / Status Ledger | What exists, what passed, what remains unproven. |
| `08` | UI / Visual Anchor or Dashboard | Human-visible view when applicable. |
| `09` | Release / Promotion Decision | Promote, hold, block, rollback or reseed. |
| `10` | Final Direction Stack | Three ranked next directions plus one sandboxed innovation area. |

## Repository Architecture Decision

| Module | Repository Decision Now | Reason |
|---|---|---|
| APEX Perfect Analysis | Keep as a registered portfolio module under the control plane until executable independence is proven. | Avoid premature repository sprawl. |
| APEX PhD Research | Register under control plane; later split when it owns a repeatable research engine or corpus workflow. | Research specifications alone do not yet require independent runtime boundary. |
| APEX Dimensions & Fields | Register under control plane; later split if it becomes a reusable ontology package consumed by multiple runtime systems. | Ontology is foundational but independent repo should be earned by integration use. |
| APEX Learning Center | Maintain dedicated repository now. | Already has independent proof-bearing pilot purpose. |
| APEX Analytics Mirror Module | Maintain dedicated repository now. | Already has application/prototype/deployment boundary. |
| APEX Test Workbench | Register under control plane until its test executor becomes a reusable runtime. | Separate when validation services and test harness are executable across repositories. |

## Integration with Existing Repositories

```text
apex-evidence-ledger
  owns: public-safe evidence contracts, proof and status records
       ↓
apex-mirror-control-plane
  owns: this development portfolio, portfolio view, decisions and benefit visibility
       ↓
apex-iteration-automater-os
  owns: governed automated work progression after rules are evidenced
       ↓
Execution Modules
  apex-learning-center · apex-analytics-mirror-sharepoint · apex-ocode
```

## Public Repository Rule

These repositories are public. Keep all initial specifications generic and public-safe. Do not place private enterprise details, confidential stakeholder names, credentials, internal source data, protected datasets or sensitive evidence records here.

## Final Direction Stack

| Rank | Direction | Why Now | Intended Output | Hold / Stop Rule |
|---:|---|---|---|---|
| **1** | Establish the six-module Development Portfolio feature and specification framework. | The visible system needs a normalized operating map before building branches independently. | Portfolio master specification and module feature register. | Do not claim module operation from documentation alone. |
| **2** | Seed the two already-independent execution repositories: Learning Center and Analytics Mirror. | They have real bounded artifact/prototype targets. | Module specs and first proof-bearing execution packages. | Keep private data out of public repositories. |
| **3** | Define interface contracts among Evidence Ledger, Mirror and Iteration Automater. | Automation must connect through governed evidence and human-visible control. | Integration and status-flow schema. | Do not activate autonomous promotion without tested controls. |
| **4 — Sandboxed Innovation** | Create an interactive APEX Development Constellation Map from this mind map. | Makes all modules clickable, status-visible and navigable as the portfolio evolves. | Visual portfolio control prototype. | Label all unbuilt features as proposed. |

🔮🧭🔬🧬🧩🧿🅾️♾️⭐️💯🌟🎞️
