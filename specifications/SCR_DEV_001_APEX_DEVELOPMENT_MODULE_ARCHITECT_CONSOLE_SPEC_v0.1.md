# SCR-DEV-001 — APEX Development Module Architect Console Specification v0.1
## Converting the On-Screen XMind Map into an Interactive Governed Development Interface

| Field | Specification |
|---|---|
| Screen ID | `SCR-DEV-001` |
| Product | `APEX Development Framework / Module Architect Console` |
| Repository | `apex-mirror-control-plane` |
| Source Visual | Current APEX Development mind map with six module nodes and linked dimensional reference visual |
| Status | `FUNCTIONAL + TECHNICAL SPECIFICATION / NOT YET BUILT` |
| Primary Operator | Otto |
| Core Purpose | Let the operator open, compare, direct and monitor development of each visible APEX module from one controlled surface. |
| Truth Boundary | This specification defines an interactive UI and its feature behavior; it is not evidence that the UI or module engines are operating yet. |

---

# 1. Screen Objective

Transform the simple central mind map into the first usable APEX development workspace:

```text
                      APEX PERFECT ANALYSIS
                              │
       APEX PHD RESEARCH ─────┤───── APEX LEARNING CENTER
                              │
APEX DIMENSIONS & FIELDS ─ APEX DEVELOPMENT ─ APEX ANALYTICS MIRROR
                              │
                              └───── APEX TEST WORKBENCH
```

The interface must preserve the clarity of the current view while enabling the user to:

- click a module to inspect it;
- see current state, features, gaps, repository route and next direction;
- change visual view mode without leaving the screen;
- inspect module coverage against the 0D–17D development lens;
- view available evidence and unresolved claims;
- choose whether to stay on a path, switch, hold, stop or innovate;
- create a controlled task packet for the Iteration Automater only after approval.

---

# 2. User Outcomes

| User Outcome ID | User Outcome | Proof of Completion |
|---|---|---|
| `UO-001` | See all visible modules in one architecture. | Six required nodes appear and are selectable. |
| `UO-002` | Understand the meaning and status of any module. | Selecting a node opens a detail drawer with mandatory fields. |
| `UO-003` | See what should be built next and why. | Each module has a Final Direction Stack and evidence/hold rule. |
| `UO-004` | Compare modules by structure, benefit, dependencies or proof. | Five view modes rearrange or replace visible content. |
| `UO-005` | Prevent visual ambition from becoming false status. | Every module and feature displays truth/lifecycle state. |
| `UO-006` | Hand off approved work into controlled execution. | Approved task packet export is available and includes a human-approval record. |

---

# 3. Main Screen Layout

## 3.1 Desktop Layout — First Target

```text
┌────────────────────────────────────────────────────────────────────────────────┐
│ APEX DEVELOPMENT  | Truth Status | Evidence | Active Cycle | GitHub | Operator  │
├───────────────┬────────────────────────────────────────────┬───────────────────┤
│ LEFT PANEL    │ CENTRAL ARCHITECTURE CANVAS                │ RIGHT CONTROL     │
│ Module list   │                                            │ View Modes        │
│ Search        │          APEX DEVELOPMENT                  │ Architecture      │
│ Filters       │        /   |   |   |   \                   │ Feature Set       │
│ Status legend │  Six selectable visible module nodes       │ Dependencies      │
│               │                                            │ Evidence          │
│               │ Selected connection/path highlights        │ Roadmap           │
├───────────────┴────────────────────────────────────────────┴───────────────────┤
│ DETAIL DRAWER / MODULE INSPECTOR — opens after selecting a node                │
├────────────────────────────────────────────────────────────────────────────────┤
│ DEVELOPMENT FLOW: Observe → Define → Model → Build → Verify → Preserve → Decide │
└────────────────────────────────────────────────────────────────────────────────┘
```

## 3.2 Core Visual Philosophy

- Start clean like the supplied mind map: a clear center node with six surrounding working areas.
- Add capability gradually through drawers, toggles and overlays rather than dense always-visible text.
- Use midnight-blue/electric-blue as the current/evidence foundation; warm gold for purpose/direction; purple for governance; green-teal for verified progress; amber/red for constraint/blocker.
- Use short in-interface labels and structured detail panels for exact wording.

---

# 4. Interface Regions

| Region ID | Region | Contents | Required Interaction |
|---|---|---|---|
| `REG-001` | Global Header | Product name, active cycle, truth indicator, evidence maturity, repository state, operator menu. | Open status, repository and truth-boundary panels. |
| `REG-002` | Module Navigator | Six modules, search, status filter, repo filter. | Select module; filter nodes; reset view. |
| `REG-003` | Architecture Canvas | Central APEX Development node; six connected module nodes; dependency lines. | Click node; hover relation; select connection. |
| `REG-004` | Right View-Control Rail | Five view modes plus display settings. | Switching view changes layout/content emphasis. |
| `REG-005` | Module Inspector Drawer | Purpose, status, outputs, features, repo, evidence, gaps, Final Direction Stack. | Tabs, open artifact, choose direction. |
| `REG-006` | 0D–17D Coverage Overlay | Development-layer coverage and gap matrix for selected module. | Toggle layer; open proof required; compare modules. |
| `REG-007` | Evidence / Truth Overlay | Commits, tests, evidence receipts, known gaps and blocked claims. | Filter by status; open receipt; mark review needed. |
| `REG-008` | Decision Control Bar | `STAY`, `SWITCH`, `HOLD`, `STOP`, `INNOVATE`, `CREATE TASK PACKET`. | Record approved intent; do not silently execute deployment. |
| `REG-009` | Development Flow Rail | Observe, Define, Model, Build, Verify, Preserve, Decide, Improve. | Show active stage and required gate. |

---

# 5. Required Module Nodes

| Node ID | Display Label | Icon Intent | Default Status at Screen Specification Stage | Detail Tabs Required |
|---|---|---|---|---|
| `NODE-APA` | APEX Perfect Analysis | Analytical prism / magnifier | `SPECIFIED` | Purpose, Features, Inputs/Outputs, Evidence, Directions |
| `NODE-PHD` | APEX PhD Research | Microscope / evidence book | `SPECIFIED` | Questions, Sources, Synthesis, Translation, Gaps |
| `NODE-DIM` | APEX Dimensions and Fields | Coordinate/layer grid | `SPECIFIED` | Layers, Fields, Dependencies, Unknowns, Quality |
| `NODE-LRN` | APEX Learning Center | Learning/brain/graph | `REPOSITORY CREATED / FOUNDATION PENDING` | Compass, Pilot, Metrics, Evidence, Roadmap |
| `NODE-ANM` | APEX Analytics Mirror Module | Dashboard/mirror | `PROTOTYPE ARTIFACT EXISTS LOCALLY` | Site, Features, Governance, Prototype, Deployment |
| `NODE-TWB` | APEX Test Workbench | Flask/check/gate | `SPECIFIED` | Tests, Cases, Failures, Promotion, Evidence |

---

# 6. Five Right-Rail View Modes

The user requested the ability to switch layouts and information emphasis. For the APEX Development screen, the first five design/view modes are:

| Mode ID | Mode | Purpose | Canvas Change | Right/Drawer Emphasis |
|---|---|---|---|---|
| `VIEW-01` | **Architecture** | Understand the ecosystem structure. | Central module constellation with colored dependency lines. | Components, links, repositories. |
| `VIEW-02` | **Feature Set** | Plan what is being built. | Nodes expand into feature progress cards; unfinished P0/P1 items surface. | Feature backlog, acceptance criteria. |
| `VIEW-03` | **Dependencies** | Identify what blocks or enables progress. | Nodes reposition by upstream/downstream flow. | Data/artifact/interface contracts, blockers. |
| `VIEW-04` | **Evidence** | Inspect what is real and proven. | Nodes size/color by evidenced status; proposed items fade/dash. | Commits, tests, receipts, missing evidence. |
| `VIEW-05` | **Roadmap** | Guide next execution. | Nodes arrange along development flow/pathway. | Final Direction Stack, hold/stop rules, task packet. |

### View Mode Acceptance Requirement

Switching modes must do more than change color. It must visibly change position, prominence, visible metrics, relationship lines or information cards in a way relevant to that mode.

---

# 7. Module Inspector Drawer Specification

When the user selects a module node, open a detail drawer with the following tabs:

| Tab | Content | Mandatory Elements |
|---|---|---|
| `Overview` | Why the module exists and its scope. | Purpose, beneficiary/user, truth boundary, status. |
| `Features` | What must be built. | P0–P3/LAB backlog with progress status. |
| `Layers` | How complete the specification is. | 0D–17D coverage heatmap and missing-lens indicators. |
| `Connections` | How it interacts with other modules. | Inputs, outputs, dependencies, repository route. |
| `Evidence` | What supports its current status. | Artifact, test, commit, limitation, evidence maturity. |
| `Directions` | What to do next. | Ranked next three, innovation option, stay/switch/hold/stop. |

---

# 8. Dimensional Coverage Overlay — Feature Definition

## Purpose

Use the supplied 0D–17D layer design as a repeatable checklist for developing each module thoroughly and truthfully.

## Display Form

For the selected module, display a layer ladder or grid with this status coding:

| State | Meaning | UI Treatment |
|---|---|---|
| `COVERED` | Required specification exists. | Green-teal check. |
| `PARTIAL` | Some definition exists; details or evidence missing. | Amber dot. |
| `MISSING` | Required layer not defined. | Red gap indicator. |
| `NOT_APPLICABLE` | Layer intentionally excluded with reason. | Grey struck marker with rationale. |
| `EVIDENCED` | Spec and named validation record exist. | Blue/green verified marker. |

## First Coverage Assessment for Visible Modules

At this stage, all six modules have identity/purpose/features specified at a high level; no module should yet be shown as fully evidenced through all layers. The UI must therefore default to `PARTIAL / SPECIFICATION STAGE` until real module artifacts and tests are linked.

---

# 9. Data Model — First Implementation Contract

## 9.1 Required Entities

| Entity | Key Fields |
|---|---|
| `Module` | `module_id`, `name`, `purpose`, `repository`, `lifecycle_status`, `truth_status`, `owner`, `description`, `risk_level` |
| `Feature` | `feature_id`, `module_id`, `name`, `priority`, `status`, `acceptance_criteria`, `evidence_required` |
| `Connection` | `connection_id`, `from_module`, `to_module`, `artifact_or_data_flow`, `status`, `blocker` |
| `LayerCoverage` | `module_id`, `layer_id`, `coverage_status`, `required_output`, `evidence_reference`, `gap` |
| `EvidenceRecord` | `evidence_id`, `module_id`, `artifact`, `claim`, `truth_label`, `validation_status`, `repository_commit` |
| `Direction` | `direction_id`, `module_id`, `rank`, `description`, `why_now`, `gate`, `hold_rule`, `decision_status` |
| `TaskPacket` | `task_id`, `module_id`, `approved_direction`, `scope`, `expected_output`, `close_when`, `block_if`, `repository_route` |

## 9.2 Sample Lifecycle Values

```text
VISION | SPECIFIED | PROTOTYPE | TESTED | PILOT_READY | PROMOTE_CANDIDATE | BLOCKED | RETIRED
```

## 9.3 Claim / Truth Values

```text
OBSERVED | IMPLEMENTED | TESTED | INFERRED | PROPOSED | BLOCKED | ASPIRATIONAL
```

---

# 10. Functional Requirements

| Requirement ID | Functional Requirement | Priority | Acceptance Criterion |
|---|---|---:|---|
| `FR-001` | Display the six module nodes around the central APEX Development node. | `P0` | All seven nodes appear with correct labels. |
| `FR-002` | Select a module node to open its inspector drawer. | `P0` | Click reveals correct module details. |
| `FR-003` | Provide search/filter by module name, status and repository. | `P1` | Filter updates visible nodes without refresh. |
| `FR-004` | Switch among five view modes. | `P1` | Layout/content materially changes by selected mode. |
| `FR-005` | Display truth and lifecycle status for each module. | `P0` | No unlabeled module status. |
| `FR-006` | Display feature backlog and acceptance criteria per module. | `P0` | Selected module shows required feature rows. |
| `FR-007` | Display 0D–17D coverage overlay per module. | `P1` | Layer coverage can be opened, filtered and reviewed. |
| `FR-008` | Display dependency/data/artifact connections. | `P1` | Connection selection opens contract details. |
| `FR-009` | Display GitHub repository and evidence records. | `P0` | Evidence status is distinguishable from proposal. |
| `FR-010` | Display Final Direction Stack and allow user to choose path state. | `P0` | User may select stay/switch/hold/stop/innovate with confirmation. |
| `FR-011` | Export an approved task packet for Iteration Automater OS. | `P2` | Packet has scope, gate, route and human approval indicator. |
| `FR-012` | Preserve prototype state locally for review sessions. | `P2` | View mode/selection survives page reload in local prototype. |

---

# 11. Non-Functional Requirements

| Requirement ID | Category | Requirement | Test Condition |
|---|---|---|---|
| `NFR-001` | Accessibility | Keyboard-selectable nodes, controls and drawer tabs. | User can complete primary flow without mouse. |
| `NFR-002` | Legibility | No critical detail depends on tiny text inside a generated visual. | Exact detail is text-rendered in UI panels. |
| `NFR-003` | Truth Integrity | Proposed or visual-reference content cannot be styled as validated. | Status test fails if claim is unlabeled. |
| `NFR-004` | Performance | Prototype navigation and mode changes respond promptly on modern desktop browser. | Interaction test confirms no blocking errors. |
| `NFR-005` | Privacy | Public prototype stores only synthetic/public-safe records. | No sensitive sample data in package. |
| `NFR-006` | Traceability | Every visible module can point to its intended repository and evidence state. | Repository-routing validation passes. |
| `NFR-007` | Reversibility | Direction selection does not automatically execute irreversible action. | UI requires approval/task export gate. |

---

# 12. Technical Architecture — Browser Prototype First

```text
modules.registry.json
connections.registry.json
features.registry.json
layers.registry.json
        ↓
APEX Module Architect Console Renderer
HTML + CSS + JavaScript, local-first prototype
        ↓
Interactive Canvas + Detail Drawer + View Modes + Evidence Overlay
        ↓
Exportable Task Packet / Evidence Candidate JSON
        ↓
Future Integration: Mirror API · Evidence Ledger · Iteration Automater
```

## Recommended Prototype Files

```text
prototype/
  index.html
  assets/
    apex-dimension-reference.png
  data/
    modules.registry.json
    features.registry.json
    connections.registry.json
    layers.registry.json
  src/
    app.js
    state.js
    views.js
    drawer.js
    evidence.js
    directions.js
  tests/
    interaction-tests.js
    truth-status-tests.js
    layer-coverage-tests.js
  evidence/
    build_receipt.json
```

## Implementation Boundary

First build is a local, synthetic, browser-openable prototype. Any GitHub, SharePoint, Power BI, live analytics, or execution-engine integration must be shown as future connection until configured and tested.

---

# 13. Primary User Flow

```text
1. Open APEX Development Console
2. View six-module architecture canvas
3. Select a module node
4. Inspect purpose, features, status and gaps
5. Select one of five view modes
6. Open 0D–17D coverage overlay
7. Inspect evidence / repository status
8. Select STAY, SWITCH, HOLD, STOP or INNOVATE
9. Review proposed direction and control gate
10. Export approved task packet or return to portfolio view
```

---

# 14. Acceptance Test Set for First Prototype

| Test ID | Test | Pass Condition |
|---|---|---|
| `TST-DEV-001` | Initial architecture renders. | Central APEX Development and six correct nodes visible. |
| `TST-DEV-002` | Each module opens detail drawer. | Six module clicks resolve to matching detail data. |
| `TST-DEV-003` | Five mode switcher works. | Each mode changes layout/emphasis, not only palette. |
| `TST-DEV-004` | Layer overlay works. | Selected module displays 0D–17D coverage records. |
| `TST-DEV-005` | Truth status is preserved. | No module without visible lifecycle/truth status. |
| `TST-DEV-006` | Feature details available. | At least P0/P1 features and acceptance criteria appear per module. |
| `TST-DEV-007` | Decision controls are bounded. | No click causes unapproved external write/deployment. |
| `TST-DEV-008` | Task packet export. | Export includes direction, gate, repo route and approval status. |
| `TST-DEV-009` | Accessibility basics. | Keyboard can navigate major controls and open drawer. |
| `TST-DEV-010` | Public-safe boundary. | No confidential content embedded in prototype data. |

---

# 15. Build Decision

The correct immediate build is not to develop every module deeply at once. It is to build the **Module Architect Console shell** and load the six module specifications into it, because that gives the whole development program a visible, controlled and extendable center.

## Final Direction Stack

| Rank | Direction | Why Now | Evidence Gate | Intended Output | Hold Rule |
|---:|---|---|---|---|---|
| `1` | Build the first local interactive Module Architect Console from this specification. | Converts the on-screen map into a usable development surface. | `TST-DEV-001` through `TST-DEV-010`. | Browser-openable governed prototype. | Do not call it operating control plane until tests pass. |
| `2` | Create JSON registries for modules, features, connections and dimensional coverage. | Prevents one-off hard-coded screens and prepares OCODE generation later. | Schema validation and data completeness checks. | Reusable normalized data layer. | Hold UI promotion if registry is incomplete. |
| `3` | Seed connected module repositories with public-safe feature/spec artifacts and evidence routing. | The console needs real artifact homes and traceability. | Verified commits and public-content review. | Connected repository constellation. | Do not place sensitive content in public repos. |
| `4 — LAB` | Add visual zoom navigation from the module constellation into feature, layer, test and GitHub evidence levels. | Creates the living architecture feel requested in APEX. | Sandboxed usability demonstration only. | Zoomable development navigator. | No automated promotion from visual navigation. |

🔮🧭🧿🅾️♾️💯
