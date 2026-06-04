# MIRROR-PROTOTYPE-001 — Build Execution Packet v0.1
## Interactive APEX Mirror-First Control Plane Prototype

**Repository:** `apex-mirror-control-plane`  
**Status:** `APPROVED DESIGN TARGET / NOT YET IMPLEMENTED`  
**Primary Source Anchors:** Otto-supplied *APEX Mirror Dashboard — The Complete Human System Map* and *APEX Mirror-First Operating System — Module Master Map* concept visuals.  
**Data Boundary:** All first-prototype module metrics and activity entries must be drawn from public-safe fixture records or evidence-ledger records and visibly classified as `VERIFIED_STATUS`, `DESIGNED_NOT_CONNECTED`, `DEMO_DATA`, `BLOCKED` or `ASPIRATIONAL`.

---

# 1. Builder Role

You are building the first interactive public-safe implementation of the APEX Mirror Control Plane.

Your output must create a realistic, high-fidelity application that looks and behaves like a real system control dashboard while remaining absolutely truthful about what is real, proposed, blocked or simulated.

## Core Design Law

```text
Do not make the dashboard look less powerful to preserve truth.
Make truth, evidence and human control the reason it looks powerful.
```

---

# 2. Application Purpose

Create an interactive dashboard through which Otto can:

- view all currently registered APEX modules;
- see current status, evidence, gaps, risks and next proof gates;
- select a module and explore its purpose, features, repositories and dependencies;
- switch between multiple management views;
- evaluate ranked next actions and their benefit/risk/control justification;
- record prototype decisions: `STAY`, `SWITCH`, `HOLD`, `STOP`, `INNOVATE`;
- separate present truth from future vision at all times.

---

# 3. First Prototype Data Contract

## Required Input Record Types

| Object | Purpose | Minimum First-Prototype Source |
|---|---|---|
| `ModuleRegistryRecord` | Show module identity, role, status, repo and next gate. | `APEX_ACTIVE_MODULE_REGISTRY_v0.1.json` from Evidence Ledger. |
| `EvidenceReceipt` | Explain why a claim/status is shown. | Public-safe fixtures until validation wiring exists. |
| `BlockerRecord` | Display gaps that prevent promotion. | Derived public-safe module limitations. |
| `DirectionStackRecord` | Show ranked next work and one innovation option. | Registered module/spec direction stacks. |
| `DecisionRecord` | Store Stay/Switch/Hold/Stop/Innovate actions in prototype. | Browser/local session storage only. |
| `HealthMetricRecord` | Display evidence/status/connection indicators. | Use labelled fixture or computed schema-coverage measures only. |
| `ActivityEvent` | Show recent build/provenance events. | Public-safe commit/artefact records. |

## Data-Truth State Enum

Every displayed value must visibly include one state:

```text
VERIFIED_STATUS
MEASURED
DEMO_DATA
DESIGNED_NOT_CONNECTED
BLOCKED
ASPIRATIONAL
```

### Hard Rule

A metric such as `92% active`, `1,842 evidence packages`, `12,640 cycles completed`, `84% integration health` or `live telemetry` must not appear as a real active metric unless its record includes actual evidence source and calculation. It may appear only as clearly labelled demo content during visual testing.

---

# 4. Required Navigation Architecture

Build a primary navigation sequence inspired by the supplied design anchors:

```text
VISION → DIRECTION → BRIDGE → MIRROR → OBSERVE → EXECUTE → ITERATE
→ MEASURE → EVIDENCE → LEARN → PARTNER → AI → PURPOSE → INFINITE → QUALITY
```

## Page/View Definition

| View | Required Function |
|---|---|
| `MIRROR / Overview` | Current truth state, selected module, evidence state, blockers, priorities and human control. |
| `VISION` | Future-state north star clearly separated from active capability status. |
| `DIRECTION` | Final Direction Stack, Benefit Governor concepts and recorded decisions. |
| `BRIDGE` | Integration/dependency map across APEX modules and OCODE. |
| `OBSERVE` | Module registry and current-state discovery. |
| `EXECUTE` | Bounded work orders only; show not active until evidence-gated execution exists. |
| `ITERATE` | Iteration cycles, C∞ option and convergence boundary. |
| `MEASURE` | Metrics, labels and measurement readiness. |
| `EVIDENCE` | Evidence receipts, sources, commit references, tests and gaps. |
| `LEARN` | Learning Center and research-to-capability feed. |
| `PARTNER` | Human-AI complementarity and stakeholder control concepts. |
| `AI` | AI capability modules and boundaries. |
| `PURPOSE` | Purpose kernel, guardrails and human benefit. |
| `INFINITE` | Aspirational direction only; no current status inflation. |
| `QUALITY` | Tests, acceptance gates, hold rules and promotion decisions. |

---

# 5. Required Dashboard Layout

## Overview Screen Regions

```text
┌───────────────────────────────────────────────────────────────────────┐
│ HEADER: APEX Mirror · Truth Status · Data Mode · Human Authority        │
├──────────────────────┬──────────────────────────┬─────────────────────┤
│ CURRENT TRUTH STATE  │ APEX MIRROR CORE         │ EVIDENCE / STATUS   │
│ verified & blocked   │ selected module & action │ receipts & gaps      │
├──────────────────────┼──────────────────────────┼─────────────────────┤
│ MODULE REGISTRY      │ PRIORITIES & DECISIONS   │ HEALTH / RISKS       │
│ clickable cards/map  │ 3+1 stack / controls    │ labelled indicators  │
├──────────────────────┴──────────────────────────┴─────────────────────┤
│ BUILD ROADMAP · ACTIVITY FEED · GUARDRAILS · NORTH STAR                 │
└───────────────────────────────────────────────────────────────────────┘
```

## Displayed Module Cards

At minimum, show these cards from the active registry:

1. APEX Mirror Control Plane.
2. APEX Evidence Ledger.
3. APEX Iteration Automater OS.
4. OCODE.
5. APEX Learning Center.
6. APEX Analytics Mirror SharePoint Module.
7. APEX Perfect Analysis.
8. APEX PhD Research.
9. APEX Dimensions & Fields.
10. APEX Test Workbench.

Each card must include:

- module title;
- role;
- truth status badge;
- repository status;
- evidence status;
- next proof gate;
- open-detail action.

---

# 6. Required Five View/Layout Modes

A fixed or slide-out control panel on the right side must allow the user to select a layout mode. Selecting a mode must visibly rearrange or reprioritize widgets, not just alter color styling.

| Mode | Design Goal | Highest-Priority Widgets |
|---|---|---|
| `Executive Overview` | Decide what matters next. | Outcomes, priorities, blockers, benefit hypotheses, approvals. |
| `Governance & Evidence` | Determine what can be trusted/promoted. | Evidence, truth status, tests, approvals, privacy, guardrails. |
| `Development Command` | Manage construction across modules. | Module cards, dependencies, work orders, artifacts, commits, gates. |
| `Learning & Research` | Guide evidence-backed capability growth. | Learning Center, PhD Research, gaps, experiments, transfer tests. |
| `Minimal Focus` | Focus on a single module/action. | Selected module, next gate, direction stack, decision controls. |

### Optional Additional Toggle — Human Benefit Lens

A sandbox-only toggle may reprioritize cards by intended benefit, safety/harm avoidance, learning opportunity, dignity and evidence quality. It must never conceal risks, lack of proof or effort.

---

# 7. Required Interactive Behaviors

| Interaction | Required Behavior | Persistence / Boundary |
|---|---|---|
| Select module card | Update Mirror Core detail, blockers, evidence and direction stack. | Local state; no live system claim. |
| Switch layout mode | Rearrange visible panels/widgets. | Local preference state. |
| Filter by status | Show verified/designed/prototype/blocked/aspirational categories. | Registry data only. |
| Open Evidence Drawer | Show claimed status, artifact/reference, limitations and next gate. | Evidence fixture/record. |
| Open Blocker Drawer | Show blocker impact, closure action and hold rule. | Derived registered blocker. |
| Record Decision | Create a local `STAY`, `SWITCH`, `HOLD`, `STOP` or `INNOVATE` record. | Prototype record; not an actual authorization. |
| Expand Direction | Show benefit, risk, cost/effort, proof gate and stop rule. | Spec data. |
| Open Vision View | Reveal aspirational future panels separately from present state. | Always labelled `ASPIRATIONAL`. |
| Open Activity Item | Reveal public-safe commit/artifact reference. | May link to public GitHub record where included. |

---

# 8. Required Visual Design Principles

Use the strengths of the visual anchors without preserving misleading states.

| Principle | Implementation Direction |
|---|---|
| Dark mission-control aesthetic | Navy/black background, gold/cyan status lights, clear panel borders and readable typography. |
| Golden central compass / Mirror | Centerpiece communicates orientation and control, not magical automation. |
| Visible system status | Use truth-labelled chips rather than unsupported green “active” claims. |
| Elegant density | Many panels permitted, but content remains readable and selectable. |
| Human-centered framing | Human authority and value-alignment remain visible in header/core area. |
| Future-state inspiration | North-star view is inspiring but visually marked separate from current truth. |
| Graph/data richness | Use real derived counts from registry or visibly labelled demonstration datasets only. |
| Modular expansion | New cards/views can be added through registry objects without redesigning the whole UI. |

---

# 9. Guardrail Requirements

| Guardrail | UI Requirement | Functional Stop Rule |
|---|---|---|
| Truth | Every capability/metric includes data-status state. | Block unsupported active/deployed claims. |
| Safety | Guardrail panel and risk indicator. | Hold consequential tasks without risk/rollback path. |
| Privacy | Public-safe data notice always visible. | Do not ingest or display protected/confidential information. |
| Transparency | Evidence and decision histories inspectable. | Do not hide rationale or source. |
| Consent / Approval | Human approval state shown for consequences. | No automated consequential promotion. |
| Accountability | Ownership and next gate shown. | Hold status if no closure/accountability path exists. |
| Dignity / Benefit | Human benefit lens available as optional view. | Do not rank benefits without showing evidence status and risks. |

---

# 10. Technical Implementation Direction

## Shortest Responsible Build Path

```text
Public-safe registry JSON
→ Static SPA prototype using HTML/CSS/JavaScript
→ Local state for selection/layout/decision interactions
→ Visual interaction tests
→ Evidence receipt and test report
→ Commit artifact into Control Plane repository
```

## Recommended File Structure

```text
apex-mirror-control-plane/
├── docs/
│   └── 04_MIRROR_PROTOTYPE_001_BUILD_EXECUTION_PACKET_v0.1.md
├── app/
│   ├── index.html
│   ├── styles.css
│   ├── app.js
│   └── data/
│       ├── module_registry.json
│       ├── direction_stacks.json
│       ├── evidence_fixtures.json
│       └── blockers.json
├── tests/
│   └── mirror_prototype_interactions.test.*
├── evidence/
│   └── MIRROR_PROTOTYPE_001_EVIDENCE_RECEIPT.json
└── .github/workflows/
    └── validate-mirror-prototype.yml
```

## Adapter / Integration Boundary

The first prototype should consume a public-safe copy of the Evidence Ledger registry. Live cross-repository fetching or authenticated services are optional later stages and must not be assumed operational in the first prototype.

---

# 11. Acceptance Tests

| Gate ID | Test | Pass Condition |
|---|---|---|
| `MIR-GATE-001` | Truth badge coverage. | All module cards and metrics display a valid state label. |
| `MIR-GATE-002` | Module interaction. | Selecting a module changes the central detail and relevant panels. |
| `MIR-GATE-003` | Five layout modes. | Five modes are selectable and result in visible layout/prioritization changes. |
| `MIR-GATE-004` | Evidence drawer. | Each module has evidence status, limitations and next gate visible. |
| `MIR-GATE-005` | Decision controls. | Local decision record can be created for each of five decision types. |
| `MIR-GATE-006` | Blocker integrity. | Blocked/proposed state cannot be displayed as operationally active without warning. |
| `MIR-GATE-007` | Future/current separation. | Future vision view is visibly aspirational and isolated from present metrics. |
| `MIR-GATE-008` | Public-safe content. | No sensitive content or credential-bearing data included. |
| `MIR-GATE-009` | Accessibility baseline. | Keyboard navigation, readable focus state and meaningful labels included. |
| `MIR-GATE-010` | Mobile/review responsiveness. | Dashboard remains navigable at common desktop/tablet widths. |

---

# 12. Truth-Labeled First Demo Values

The builder may use demonstration content for UI fidelity, but must label it persistently:

```json
{
  "data_status": "DEMO_DATA",
  "display_notice": "Interface demonstration values — not measured operational status.",
  "metrics": {
    "evidence_coverage": "Not measured",
    "integration_health": "Not measured",
    "iteration_velocity": "Not measured",
    "module_connectivity": "Designed connections only",
    "human_approval": "Control framework proposed"
  }
}
```

Where a repository or committed document has been verified, the builder may show categorical status such as:

```json
{
  "data_status": "VERIFIED_STATUS",
  "statement": "Repository exists and contains committed specification artifacts.",
  "evidence_reference": "repository/path/commit_sha"
}
```

---

# 13. Exact Implementation Instruction for a Coding Agent

```text
Build MIRROR-PROTOTYPE-001 as an interactive public-safe SPA prototype in the apex-mirror-control-plane repository.

Read and preserve:
- docs/00_APEX_DEVELOPMENT_PORTFOLIO_INDEX_v0.1.md
- docs/01_APEX_DEVELOPMENT_MASTER_FRAMEWORK_AND_SPECIFICATION_v0.1.md
- docs/02_APEX_DEVELOPMENT_FEATURE_REGISTER_AND_ACCEPTANCE_GATES_v0.1.md
- docs/03_APEX_MIRROR_FIRST_CAPABILITY_EXTRACTION_AND_APPLICATION_SPEC_v0.1.md
- this execution packet
- the active module registry JSON exported from apex-evidence-ledger

Implement:
- overview dashboard with Mirror-first center;
- clickable registered module cards;
- evidence, blockers, direction stack and activity panels;
- persistent data-status labels;
- Stay/Switch/Hold/Stop/Innovate local decision controls;
- five selectable right-hand layout modes;
- separate future-state Vision view;
- local public-safe fixture data only;
- tests for all MIR-GATE-001 through MIR-GATE-010.

Do not:
- show unsourced live percentages or performance measures;
- claim integrated automation, deployment, digital twins or real outcomes;
- use private/confidential data;
- remove human authority or evidence boundaries.

Deliver:
- application files;
- test results;
- evidence receipt;
- README for review;
- Final Direction Stack.
```

---

# 14. Final Direction Stack

| Rank | Direction | Immediate Build Outcome | Evidence / Control Gate | Stop Rule |
|---:|---|---|---|---|
| **1 — Highest Priority** | Build the interactive Mirror prototype from the registry and this packet. | Reviewable Mirror-first application with truthful module navigation. | Pass `MIR-GATE-001` through `010`. | Hold if status/metric labels can mislead reviewers. |
| **2 — Next Priority** | Add evidence receipt fixtures and registered artifact/commit references. | Evidence drawer and public-safe provenance feed. | Evidence objects validate against ledger schema. | Do not display unsupported verified states. |
| **3 — Governance / Visibility** | Connect decision records and bounded work-order design to the Iteration Automater contract. | Visible user-control-to-execution interface. | Human control, hold and rollback rules explicitly tested. | No autonomous execution promotion from prototype actions. |
| **4 — Random Innovation Area — Sandboxed** | Implement the Human Benefit Lens alternative view. | Dashboard can rank actions through benefit/dignity/learning/opportunity perspectives with evidence visible. | Prototype-only; user can switch it off at any moment. | Reject any ranking that hides risk, evidence gaps or user override. |

**Module Signature:** `🪞🧿🧭📊🅾️♾️💯`  
**Build Mode:** `🔮🧭🔬🧬🧩🧿🅾️♾️⭐️💯🌟🎞️`
