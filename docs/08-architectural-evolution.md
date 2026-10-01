# 8. Architectural Evolution

This section applies the principle of intentional architecture and emergent design (Trade-off 2 in section 2.3). Decisions whose consequences reach beyond a single team are made deliberately across teams; everything else belongs to the teams.

## 8.1 Reversibility is the dividing line

Not every architectural decision needs central attention. The test is reversibility: decide centrally and early only what is hard to undo and affects several teams, such as public API contracts, data ownership, and integration patterns between systems. Decisions that are cheap to undo, such as internal structure, local patterns, and implementation choices, are made and changed by the teams themselves, without formal process. G3 checks that the one-way-door decisions have been identified and that the list is kept as short as possible.

## 8.2 Runway, not blueprint

The Design stage builds architectural runway: enough settled architecture to support the next features, and no more. Runway built long before it is needed becomes inventory. It is half-decided design that ages, constrains the teams, and is often wrong, and it carries the cost of deciding early without the benefit of deciding later with better information. The Solution Design names the minimum set of decisions, marks each as a one-way or two-way door, and leaves the rest to the teams.

## 8.3 The architecture feedback path

Architecture must also change in response to delivery. When a team finds an architectural constraint or a better boundary while building, it raises the finding to VSAR. If the change is local and easy to undo, the team acts on it. If it reaches beyond one team, VSAR either amends the current Solution Design, while the epic is still in progress, or logs the finding in the Option Pool as future work.

## 8.4 Contracts are the stability guarantee

Emergence is safe at scale when the contracts between teams are stable; the design itself does not need to be frozen. As long as API and integration contracts hold, and change only through a visible, versioned process, teams can change everything behind them without asking permission. This follows the evolutionary-architecture principle of guaranteeing interfaces rather than implementations.
