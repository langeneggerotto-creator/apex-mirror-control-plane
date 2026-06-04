# APEX Mirror Visibility Policy v1.0
## Default Iteration Operation: Verified Vertical Slice First

| Field | Value |
|---|---|
| Policy ID | `MIRROR-ITER-VVSF-001` |
| Applies To | All APEX / Perfect AI module cards, dashboards, task views and direction panels |
| Default Mode Display | `VERIFIED VERTICAL SLICE FIRST` |
| Conditional Scale Display | `APEX 1M / 🧪Ⓥ1M🅾️♾️💯 — INACTIVE UNTIL SLICE VERIFIED` |
| Status | `LOCKED VISIBILITY RULE / PUBLIC-SAFE CONTROL RECORD` |
| Truth Boundary | Visibility of this policy is not evidence that a slice has passed or scale has been approved. |

## Operator-Facing Rule

The APEX Mirror must show that each module begins with a smallest complete proof-bearing workflow rather than automatic mass iteration.

```text
Verified Vertical Slice First
→ Build one smallest useful end-to-end path
→ Run defined tests
→ Capture evidence and limitations
→ Decide if the loop is worth repeating
→ Permit only approved, bounded scale progression
```

## Mirror Required Display Fields

Every active module status card or module inspector must display:

| Display Field | Required Value / Behavior |
|---|---|
| `iteration_mode` | Defaults to `VERIFIED_VERTICAL_SLICE_FIRST`. |
| `vertical_slice_id` | Shows current bounded proof path, or `NOT YET DEFINED`. |
| `slice_status` | `NOT_DEFINED`, `DEFINED`, `RUN_RECORDED`, `REPAIR_REQUIRED`, `VERIFIED_IN_SCOPE`, `SCALE_CANDIDATE`, `HOLD`, `STOP`, `ROLLBACK`. |
| `benefit_tested` | What payoff/value the slice is intended to prove. |
| `evidence_status` | Receipt/test/commit status from Evidence Ledger. |
| `known_limitations` | Visible before any scale eligibility is shown. |
| `scale_eligibility` | `INACTIVE`, `NOT_ELIGIBLE`, `REVIEW_CANDIDATE`, or `APPROVED_BOUNDED_RUN`. |
| `operator_choice` | `STAY`, `SWITCH`, `HOLD`, `STOP`, `ROLLBACK`, `REVIEW SCALE`. |
| `next_action` | Smallest controlled action to close the next proof gap. |

## APEX 1M Display Rule

`APEX 1M / 🧪Ⓥ1M🅾️♾️💯` must not appear as an active current execution mode by default. Until evidence and approval are complete, it must display as:

```text
CONDITIONAL SCALE MODE — LOCKED PENDING VERIFIED VERTICAL SLICE
```

### Mirror Must Block the Following Displays Without Evidence

- `APEX 1M ACTIVE`
- `READY TO SCALE`
- `LOOP PROVEN`
- `PRODUCTION READY`
- `REAL-WORLD IMPACT VERIFIED`

unless the applicable evidence, scope and approval status exist.

## Module Architect Console Integration

For `SCR-DEV-001 — APEX Development Module Architect Console`, add the following controls and states:

| Region | Required Addition |
|---|---|
| Header Status Bar | Global default: `Verified Vertical Slice First`. |
| Module Node Badge | Slice status badge and evidence indicator. |
| Module Inspector → Directions Tab | Selected vertical slice, benefit tested, proof gate and next decision. |
| Evidence View Mode | Slice receipts and scale-eligibility status. |
| Roadmap View Mode | `Slice → Verify → Small Repeat → Scale Review`, not immediate mass iteration. |
| Decision Control Bar | Add `REVIEW SCALE` only when eligibility is supported by evidence. |

## Initial Slice Candidate Display

The screen should present these bounded candidates for operator selection rather than activate all at once:

| Candidate ID | Module | Vertical Slice | Intended Benefit Test | Initial Status |
|---|---|---|---|---|
| `VS-DEV-CONSOLE-001` | APEX Mirror Control Plane | One module node → details → direction selection → exported task packet → evidence record. | Prove the development console can guide controlled work. | `DEFINED_CANDIDATE` |
| `VS-LRN-PILOT-001` | APEX Learning Center | One matched learning task across Human-only, AI-only and Human+AI. | Prove whether Human+AI improves learning performance in scope. | `DEFINED_CANDIDATE` |
| `VS-OCODE-001` | OCODE | One supported source → OCODE map → web output → behavior check. | Prove first bridging-code path. | `DEFINED_CANDIDATE` |

## UI Acceptance Criteria

| Test ID | Acceptance Criterion |
|---|---|
| `MIR-VVSF-T001` | Every active module card displays an iteration-mode field. |
| `MIR-VVSF-T002` | New modules default to `VERIFIED_VERTICAL_SLICE_FIRST`. |
| `MIR-VVSF-T003` | `APEX 1M` is shown inactive until verified-slice evidence and scale approval exist. |
| `MIR-VVSF-T004` | Operator can view evidence, limitations and hold rule before selecting scale review. |
| `MIR-VVSF-T005` | Any unsupported scale or production claim appears as blocked, not active. |

## Final Direction Stack

| Rank | Direction | Why Now | Evidence / Control Gate | Intended Output | Hold / Stop Rule |
|---:|---|---|---|---|---|
| 1 | Add `iteration_mode`, `vertical_slice_id`, `slice_status` and `scale_eligibility` fields to the Module Architect Console data model. | The new rule must become visible behavior, not only policy text. | Registry/schema update validates required fields. | VVSF-ready module registry. | Hold prototype promotion if scale status can be unlabeled. |
| 2 | Select and execute one first vertical slice from the three candidates. | The default operation must generate real proof. | Operator-selected scope, acceptance criteria and evidence route. | First verified-slice execution record. | Do not execute all candidates in parallel before one loop proves value. |
| 3 | Connect Mirror evidence display to the Evidence Ledger scale gate. | Operator control depends on seeing why scaling is or is not allowed. | Receipt and commit state render accurately. | Scale-eligibility control panel. | Do not allow active scale labels without receipt. |
| 4 — LAB | Visualize scale readiness as a bridge that only illuminates when each slice gate is satisfied. | A strong visual metaphor may make governance instantly legible. | Prototype-only usability review. | Evidence-lit scale bridge concept. | No automated decision from visuals alone. |

🔮🧭🧿🅾️♾️💯
