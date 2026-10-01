# 9. Definitions of Ready and Done

## 9.1 Feature: Definition of Ready (entry to Delivery Backlog)

- Traces to an epic and bundles specific use case flows of exactly one use case.

- Parent epic passed G1, G2, and G3.

- Boundary-level detailed design for this feature exists in the living artifacts: its bundled flows at testable precision, and draft contract versions wherever it crosses team lines.

- Low-fidelity UX concept exists where the feature is user-facing (VSCX).

- E2E test scenarios derived from its bundled flows exist.

- Acceptance criteria are written and testable.

- Delivering teams are identified and within their agreed capacity share.

- Small enough to complete within one VS Increment.

## 9.2 Feature: Definition of Delivered (entry to the Acceptance Queue)

- All child stories done on their team boards (including team-level functional and NFR testing).

- E2E automated tests, both functional and NFR, bound from the test scenarios and green in staging.

- Living system documentation updated (architecture, use case flows, API contracts as applicable).

- Deployed dark to production.

## 9.3 Feature: Definition of Done

- All Delivered criteria met.

- Accepted by business stakeholders (UAT).

- No open defects above the stream’s agreed severity threshold.

## 9.4 Epic: Definition of Done

- All features done or explicitly descoped.

- Living documentation reflects the target state described in the Solution Design.

- ADRs promoted from the Solution Design into the permanent record.

- Solution Design archived.
