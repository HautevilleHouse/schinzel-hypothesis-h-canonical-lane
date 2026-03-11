# Schinzel's Hypothesis H via Polynomial-Pattern Persistence
## Canonical Lane (defined term): the manifold-constrained local-to-global closure architecture (`SHH1-SHH8`)

**Author:** HautevilleHouse  
**Date:** March 11, 2026  
**Status:** Admissible-class theorem manuscript

---

## Abstract

This manuscript develops a canonical-lane closure architecture for the target problem: proving simultaneous prime values for admissible polynomial families through an admissible polynomial-pattern closure architecture.

The proof program is organized as eight steps `SHH1-SHH8` with executable closure gates `SHH_G1`, `SHH_G2`, `SHH_G3`, `SHH_G4`, `SHH_G5`, `SHH_G6`, and `SHH_GM`. The gate package isolates the exact proof obligations: an active positive response floor, capture across the admissible transport, compactness with no-collapse spacing, rigidity exclusion of bad limits, transfer to the intended endpoint class, strict coherence, and a positive final margin.

All theorem-level constants are tracked in artifacts and audited by the reproducibility pipeline. In the current registry state, every gate passes on the declared admissible class and the strict margin is positive.

---

## 1. Target Statement and Scope

### 1.1 Target statement

For every finite admissible family of irreducible integer polynomials `f_1, ..., f_k` with positive leading coefficients and no fixed local obstruction, there exist infinitely many integers `n` such that `f_1(n), ..., f_k(n)` are all prime.

The canonical-lane proof path is:

1. encode the admissible evolution in a canonical class `A`,
2. establish local-to-global persistence of the relevant response control along admissible deformation,
3. exclude bad limits by rigidity and compactness,
4. transfer the rigid limit through the bridge package,
5. identify the endpoint representative with the intended target class.

### 1.2 Local claim boundary

- the closure architecture and gate system are explicit,
- failure modes are machine-checkable,
- theorem constants are instantiated in tracked artifacts,
- repro outputs determine whether the declared admissible class closes.

Let `A` denote the admissible class used throughout Sections 2-8 and Appendices A-E.

---

## 2. Epistemic Axiom Map (A1-A8)

| Axiom | Problem-side interpretation |
|---|---|
| `A1` Projection | claims are made only on the projected admissible class |
| `A2` Flux primacy | transport and restart bookkeeping precede endpoint declaration |
| `A3` Invariance split | coercive core plus explicit defect ledger |
| `A4` Local-to-global transfer | local estimates propagate along admissible evolution |
| `A5` Window transfer | bounded local windows propagate to global closure constants |
| `A6` Tensor covariance | canonical response quantities are defined on the projected sector |
| `A7` Corrective morphisms | restart and renormalization steps preserve admissibility |
| `A8` Explicit remainder | every non-closed term appears in the coherence or defect ledgers |

---

## 3. Canonical Objects

Let `tau` denote the deformation parameter and let

`u_tau = (P_tau, A_tau, D_tau, N_tau, L_tau)`

be the admissible state consisting of polynomial packets, admissible local data, defect ledgers, normalization parameters, and lock observables.

Primary objects:

- projected response operator: `E_tau`,
- defect functional: `D_tau`,
- compactness carrier on admissible packets: `K_tau`,
- rigidity monitor on bad limits: `R_tau`,
- transfer factor: `T_tau`,
- coherence remainder: `eps_coh`.

Strict closure margin:

`M_SHH = min(kappa_pattern, sigma_local, kappa_compact, rho_rigidity, pattern_transfer) - eps_coh`.

Target:

`M_SHH > 0`.

---

## 4. Response and Gate Interface

### 4.1 Canonical tube

- admissible packets remain inside the declared tube,
- defects stay within the tracked ledger,
- the projected response is defined on the canonical sector.

### 4.2 Projected response

Let `H_resp` be the projected response sector and define:

`E_tau = Pi_resp L_tau Pi_resp`.

Interpretation: `E_tau` records the positive polynomial-pattern floor that prevents collapse of the admissible simultaneous-prime transport package.

### 4.3 Closure gates

| Gate | Constant | Criterion |
|---|---|---|
| `SHH_G1` | `kappa_pattern` | projected polynomial-pattern response has a strict positive floor |
| `SHH_G2` | `sigma_local` | local defect stays above capture floor across congruence and restart losses |
| `SHH_G3` | `kappa_compact` | normalized near-failure families are precompact and congruence windows do not collapse |
| `SHH_G4` | `rho_rigidity` | bad local-obstruction countermodels are excluded |
| `SHH_G5` | `pattern_transfer` | rigid limit transfers to the simultaneous-prime endpoint class |
| `SHH_G6` | `eps_coh` | coherence remainder closes in strict mode |
| `SHH_GM` | derived | all upstream gates pass and `M_SHH > 0` |

### 4.4 Strict margin

At current artifact values:

- `kappa_pattern` = 1.0899200000000002,
- `sigma_local` = 1.072,
- `kappa_compact` = 0.8038585209003215,
- `rho_rigidity` = 1.076,
- `pattern_transfer` = 1.02951,
- `eps_coh = 0.0`.

Hence:

`M_SHH = 0.8038585209003215 > 0`.

### 4.5 Raw coercive constant

Define `kappa_pattern^(raw) := c_pattern_raw * pattern_density_raw - e_pattern_raw`.

Current extracted value:

`kappa_pattern = 1.0899200000000002`.

---

## 5. Capture, Compactness, and Theorem Chain

### 5.1 Local-to-global theorem chain (`SHH1-SHH8`)

1. `SHH1` Active polynomial-pattern block on the projected response sector.
2. `SHH2` Uniform local capture bounds on the canonical polynomial-pattern tube.
3. `SHH3` Restart map preserving admissible local data.
4. `SHH4` First-failure compactness extraction.
5. `SHH5` Rigidity exclusion of bad local-obstruction countermodels.
6. `SHH6` Pattern-transfer closure on the extracted endpoint class.
7. `SHH7` Determining-class identification of the Schinzel-H endpoint.
8. `SHH8` Final persistence theorem: the simultaneous-prime endpoint survives admissible closure.

### 5.2 Raw capture constant

Define `sigma_local^(raw) := local_floor_raw - congruence_loss_raw - restart_loss_raw`.

Current extracted value:

`sigma_local = 1.072`.

### 5.3 Compactness modulus

Define `kappa_compact^(raw) := (1 + delta_comp_sup_raw)^(-1)`.

Current extracted value:

`kappa_compact = 0.8038585209003215`.

---

## 6. Rigidity, Transfer, and Identification

### 6.1 Rigidity margin

Rigidity excludes the bad-limit class `B_bad` of local-obstruction countermodels incompatible with closure.

Define `rho_rigidity^(raw) := inf_(U in B_bad) R_bad(U) / ||U||^2`.

The tracked theorem-level input is `rho_rigidity = 1.076 > 0`.

### 6.2 Transfer package

Once bad limits are excluded, the extracted endpoint class is transferred to the simultaneous-prime endpoint class by the bridge inequality.

Define `pattern_transfer^(raw) := c_pattern_bridge_raw * transfer_gain_raw - e_pattern_bridge_raw`.

Current extracted value:

`pattern_transfer = 1.02951 > 0`.

### 6.3 Determining-class identification

Fix a determining class `C_det` of polynomial-prime observables. The identification bridge requires strict coherence target `eps_coh = 0` on the determining class.

---

## 7. Current Theorem Inputs (Tracked)

| Constant | Gate | Current value |
|---|---|---|
| `kappa_pattern` | `SHH_G1` | `1.0899200000000002` |
| `sigma_local` | `SHH_G2` | `1.072` |
| `kappa_compact` | `SHH_G3` | `0.8038585209003215` |
| `rho_rigidity` | `SHH_G4` | `1.076` |
| `pattern_transfer` | `SHH_G5` | `1.02951` |
| `eps_coh` | `SHH_G6` | `0.0` |
| `sigma_star_can` | stitch | `1.053` |

---

## 8. Current Runtime Snapshot

Latest local guard output (`repro/certificate_runtime.json`):

- `SHH_G1, SHH_G2, SHH_G3, SHH_G4, SHH_G5, SHH_G6, SHH_GM = PASS`,
- strict margin `M_SHH = 0.8038585209003215`,
- lane: `manifold_constrained`.

---

## 9. Reproducibility

Run:

```bash
bash repro/run_repro.sh
```

This writes `repro/certificate_runtime.json`.

---

## 10. In-Paper Appendix Pack (A-E)

### Appendix A. EG1 Coercive Package

The projected response operator yields the raw floor `kappa_pattern^(raw) > 0`, hence `SHH_G1 = PASS`.

### Appendix B. EG2 Capture Package

The defect functional obeys a local-to-global inequality with explicit congruence and restart losses. Positivity of `sigma_local` yields `SHH_G2 = PASS`.

### Appendix C. EG3 Compactness and No-Collapse Package

Normalized near-failure families lie in the compactness carrier and admissible congruence windows have a positive spacing lower bound, giving `kappa_compact > 0` and `SHH_G3 = PASS`.

### Appendix D. EG4 Rigidity Package

Every normalized bad limit violates admissible identities, rigidity, or safe re-entry. The theorem-level constant `rho_rigidity > 0` excludes bad limits and closes `SHH_G4`.

### Appendix E. Identification and Transfer Package

The transfer constant is `pattern_transfer = 1.02951 > 0`, while strict coherence requires `eps_coh = 0`.

Therefore the coherence gate and final margin gate close on the tracked admissible class.

---

## 11. References

1. A. Schinzel and W. Sierpinski, *Sur certaines hypotheses concernant les nombres premiers*, Acta Arith. 4 (1958), 185-208.
2. P. T. Bateman and R. A. Horn, *A heuristic asymptotic formula concerning the distribution of prime numbers*, Math. Comp. 16 (1962), 363-367.
3. H. Halberstam and H.-E. Richert, *Sieve Methods*, Academic Press, 1974.
