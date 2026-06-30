# EG2 Public Note (Capture and Restart)

Mature wording: `transport / local-to-global transfer`.

In-paper anchor: `paper/SCHINZEL_HYPOTHESIS_H_PREPRINT.md` (`SHH_G2`).

## Goal
Expand the compressed capture/restart language into the local-to-global transport gate for `proving simultaneous prime values for admissible polynomial families through an admissible polynomial-pattern closure architecture`.

## Objects

- transport carrier: the admissible evolution, deformation, or routed lattice declared in the preprint.
- capture floor: `sigma_local`.
- restart law: the normalization/re-entry rule that keeps corrective steps inside the admissible class.
- carried losses: defect, restart, and normalization losses that must remain explicit.

## Closure Criterion

`SHH_G2` closes when `sigma_local` survives admissible losses and restart corrections: local defect stays above capture floor across congruence and restart losses.
This is the transport contribution to `M_SHH`.

## Lemma Chain and Proof Payload

### Lemma EG2.1 (transport accounting)
Every transport step used by the lane is charged to the declared defect ledger instead of being absorbed into prose.

Payload: verify that the capture constant `sigma_local` is present in the constants registry and extraction inputs.

### Lemma EG2.2 (restart preservation)
Restart or normalization preserves the declared admissible class and does not create an untracked remainder.

Payload: inspect the repro script and guard output for the gate tied to `sigma_local`.

### Theorem EG2.3 (capture gate closure)
If transport accounting and restart preservation hold, then `SHH_G2` carries local control forward without breaking admissibility.

## Current Instantiation

- gate: `SHH_G2`
- artifact key: `sigma_local`
- mature equivalent: `transport / local-to-global transfer`
- audit surface: `repro/run_repro.sh` and `repro/certificate_runtime.json`
