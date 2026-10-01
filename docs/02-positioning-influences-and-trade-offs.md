# 2. Positioning, Influences, and Trade-offs

## 2.1 What this playbook is, in one sentence

Flow-based Kanban coordination across a two-level board system, running over autonomous product teams, with intentional architecture at the boundaries, emergent design inside them, a cadence for delivery, and continuous flow for shaping.

## 2.2 Influences

The playbook builds on established work and reuses its vocabulary. The main influences, and what each contributes:

- **Donald Reinertsen:** the economic view of product development behind the overall design: small batches, explicit queue management, WIP constraints, and cadence as a synchronization mechanism. The Option Pool and the commitment point apply his options thinking. An unstarted item is an option, and exercising it late, with better information, has economic value (The Principles of Product Development Flow).

- **Klaus Leopold:** the two-level board architecture. The VS board is a coordination board (Flight Level 2) and the team boards are operational boards (Flight Level 1). Flight Levels supports the structure used here, which coordinates across teams without owning them.

- **Mary and Tom Poppendieck:** lean software development. Its principles include eliminating waste, amplifying learning, deciding as late as possible, and empowering the team. Stopping work early at the gates is a form of waste elimination, since building the wrong thing is costly.

- **Matthew Skelton and Manuel Pais:** the team-topology vocabulary. The business product team is a stream-aligned team, and the enabler teams are platform teams, shared because they serve many streams.

- **Neal Ford and Rebecca Parsons:** the contract-first view of architectural change. When interfaces are stable, the architecture behind them can evolve safely (Building Evolutionary Architectures).

- **Ivar Jacobson:** Use-Case 2.0, the requirements backbone of this playbook. A use case is described by its flows; a slice bundles one or more flows into a work item carrying its own test cases. Here, the flows are the permanent model and the feature is the slice.

## 2.3 Trade-offs

Three positions in this playbook may not align with a strict reading of agile or lean practice. They are deliberate choices, and each has a cost, described below.

**Trade-off 1: shared enabler teams.** Classic value-stream thinking prefers every team dedicated to one stream, because sharing creates contention and context-switching. This playbook dedicates the business product team but shares the enabler teams, because they own core IT products that serve many streams; duplicating them per stream would itself be waste. This follows the stream-aligned-plus-platform topology. The cost is that enabler teams can become a shared constraint across streams. Capacity shares, the PO as the single arbitration point, and the shared roadmap as a recorded capacity agreement are there to manage this dependency. If contention stays high despite them, the response is to grow enabler capacity rather than change the topology.

**Trade-off 2: intentional architecture over pure emergence.** Agile favors emergent design. This playbook takes the position that purely emergent architecture does not hold up when multiple independent teams share core systems. Emergence optimizes locally, while architecture consists of the decisions whose consequences reach beyond one team. Team-level agility is unaffected; only architecture requires cross-team intent. Section 8 describes the boundary: decide centrally only what is irreversible and cross-cutting, and leave everything else to emergent design inside the teams. The cost is that this requires mature contract discipline and a good working relationship between VSAR and the tech leads. The balance between central decisions and emergence also has to match the organization’s actual maturity, rather than being set once for everyone.

**Trade-off 3: documentation weight.** The Agile Manifesto values working software over comprehensive documentation. This playbook asks for more documentation than a single team would need: living system documentation, one Solution Design per epic, and ADRs where required. At multi-team scale, leaving shared knowledge undocumented is not lean, because it keeps that knowledge in people’s heads, where it is costly to access and easy to lose. A few rules keep the weight under control. Knowledge is permanent, while work items are temporary. Work items point at knowledge instead of holding it. Documentation updates are part of the Definition of Done (section 9). Temporary documents are archived once the living documents have absorbed them.
