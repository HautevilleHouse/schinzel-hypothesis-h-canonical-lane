# Reviewer Map

    ## Claim Scope

    - Canonical-lane claim: inside the `manifold_constrained` lane, if the theorem chain in this repository holds and the guard certificate passes, the repository-level closure claim is satisfied.
    - Standard target claim: carried by the in-repo bridge theorems tying the lane to the target statement.

    ## Theorem Dependency Chain

    1. `EG1`: coercive response and active control floor.
    2. `EG2`: capture and admissible continuation.
    3. `EG3`: compactness and no-collapse spacing.
    4. `EG4`: rigidity and transfer.
    5. Identification bridge: strict coherence on the determining class.
    6. Scalar closure: `SHH_G1, SHH_G2, SHH_G3, SHH_G4, SHH_G5, SHH_G6, SHH_GM` all `PASS`.

    Primary files:

    - `paper/SCHINZEL_HYPOTHESIS_H_PREPRINT.md`
    - `notes/EG1_public.md`
    - `notes/EG2_public.md`
    - `notes/EG3_public.md`
    - `notes/EG4_public.md`
    - `notes/IDENTIFICATION_BRIDGE.md`

    ## Closure Gates

    | Gate | Constant | Description |
    |------|----------|-------------|
    | `SHH_G1` | `kappa_pattern` | projected polynomial-pattern response has a strict positive floor |
| `SHH_G2` | `sigma_local` | local defect stays above capture floor across congruence and restart losses |
| `SHH_G3` | `kappa_compact` | normalized near-failure families are precompact and congruence windows do not collapse |
| `SHH_G4` | `rho_rigidity` | bad local-obstruction countermodels are excluded |
| `SHH_G5` | `pattern_transfer` | rigid limit transfers to the simultaneous-prime endpoint class |
| `SHH_G6` | `eps_coh` | strict coherence / identification closure |
| `SHH_GM` | derived | final strict margin |

    ## Falsification Conditions

    - `repro/certificate_runtime.json` has any non-`PASS` gate.
    - `lane.active_lane != "manifold_constrained"`.
    - `all_pass != true`.
    - Any manifest hash mismatch under `repro/repro_manifest.json`.
    - A verified counterexample to any EG theorem statement used in the paper.
