# 3. Principles

- **Value-stream based:** A business product drives each development value stream; enabler products support it. The unit of optimization is the stream rather than the project.

- **Use-case driven:** Requirements flow from customer journeys through use cases and their flows to epics, features, and stories. The use case model is the master, and work items are created to track changes to it. Every functional work item traces to a use case. Enabler work (runway, tech debt, compliance) traces to its architectural rationale instead, meaning an ADR, the Solution Design, or a named runway item.

- **Intentional architecture, emergent design:** Architecture at the boundaries is intentional; design within them is emergent. The dividing line is reversibility: irreversible, cross-team decisions are made deliberately and early; everything cheap to reverse belongs to the teams.

- **Multi-track, options-based:** Shaping runs as continuous flow; Delivery runs on a fixed cadence; Acceptance and Release return to flow. Two explicit buffers decouple the zones: the Delivery Backlog (the commitment point) and the Acceptance Queue (the delivered line). Unstarted work is treated as an option that can still be dropped.

- **Kanban-governed:** Stages, gates, WIP limits, and pull policies govern how work moves. Nothing advances until it meets the stage’s exit policy.

- **Team autonomy:** Product teams own their backlog, method, cadence, and board, and may serve several value streams concurrently.

- **Low ceremony:** The only scheduled ceremony is the increment planning event every 6 weeks. Everything else is handled through board policies, applied as work arrives.
