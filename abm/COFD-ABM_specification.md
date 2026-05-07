# COFD-ABM: Agent-Based Model Specification

*Extracted from Appendix B of the CFD main paper.*
*Status: Preliminary specification — pending implementation and empirical validation.*

---

## Overview

The Coupled Functional Differentiation Agent-Based Model (COFD-ABM) instantiates the four-loop CGM computationally. This document provides a specification sufficient for implementation.

## B.1 Agent Types

### Type I — Individual Agents

| Property | Description |
|----------|-------------|
| **State** | `{biological state b_k, cognitive load c_k, affective state e_k, motivational stack m_k, internalization vector I_k = (I_{k,1}, …, I_{k,7})}` |
| **Actions** | Respond to exposure (update `I_k`); make decisions in choice tasks based on current internalization and active group logic |
| **Group membership** | Each individual belongs to one or more groups (family, work team, friend network) |

### Type II — Group Agents

| Property | Description |
|----------|-------------|
| **State** | `{member set M_g, active relational logic S_g, situational cue vector u_g}` |
| **Actions** | (a) Compute `u_g` from environment and membership; (b) probabilistically update `S_g` per softmax equation; (c) mediate individual decisions according to `S_g`; (d) reconcile multi-logic activation per status arbitration, narrative reframing, or logic stratification |

### Type III — Subsystem Agents

| Property | Description |
|----------|-------------|
| **State** | `{output O_i, code C_i, programs P_i, resource state R_i}` |
| **Actions** | (a) Receive inputs from coupled subsystems and from individual decisions; (b) apply programs `P_i` to inputs to produce `O_i`; (c) propagate `O_i` to coupled subsystems through `Γ`; (d) update channels through which exposure `E` reaches individuals |

## B.2 Environment

The environment includes:

- **Coupling matrix `Γ`**: initialized empirically from historical estimation; updated per equation A.4
- **Resource vector `R(t)`**
- **Exogenous shock generator** producing `ε_i(t)`
- **Buffering vector `B(t)`**

## B.3 Time Step (One Tick)

1. Subsystems generate outputs `O_i(t)` given current inputs and program rules.
2. Outputs propagate through `Γ` to other subsystems and through channels to individuals (updating exposure `E_{k,i}`).
3. Groups update situational cues `u_g`.
4. Groups probabilistically update active relational logic `S_g`.
5. Individuals update internalization `I_{k,i}` per internalization equation.
6. Individuals make decisions, mediated by their group's `S_g`, weighted by their `I_k`.
7. Decisions aggregate (per channel-specific aggregation functions) into next-period subsystem inputs.
8. The buffering vector `B(t)` updates per institutional design rules.
9. The coupling matrix `Γ` evolves slowly per coupling update equation.
10. **Loop 4 (slow):** Periodically (per `Δ` ticks), the social-scientific subsystem updates `K_t` and modifies programs `P_i` per performative reflection equation.

## B.4 Calibration Parameters

| Parameter | Symbol | Range | Notes |
|-----------|--------|-------|-------|
| Learning-rate constant | `α` | 0.01–0.10 per tick | Lower for adult learning, higher during sensitive periods |
| Logic-switching inverse temperature | `β` | 1–5 | Higher β → more deterministic responsiveness to cues |
| Coupling-influence rate | `δ` | 0.05–0.30 | Estimable from impulse-response analysis on historical data |
| Coupling-formation rate | `η` | 0.001–0.01 | Slow |
| Buffering effectiveness | `μ` | 0.1–0.5 | Policy-dependent; higher with effective regulation |
| Loop-4 uptake rate | `φ` | ~0.01 | Slow |

## B.5 Expected Emergent Outcomes

Validation criteria for the ABM include the following emergent outcomes (each corresponding to a proposition in §5):

| Scenario | Expected Outcome | Validates |
|----------|-----------------|-----------|
| Sustained increase of `η` without buffering | `λ_max(Γ)` rises; crisis-synchronization frequency rises super-linearly | P3, P7 |
| Sustained asymmetric coupling from one subsystem to another | Terminology drift in the colonized subsystem develops | P4 |
| Platform-equivalent acceleration of Loops 1, 2, and 4 | Individual decision latency declines; platform-prediction accuracy rises | P9 |
| Externally imposed resource shock to small groups | MP displaces EM | P1 |
| Threat plus homogeneity condition | CS displaces both AR and MP | P12 |

## B.6 Implementation Notes

- A reference implementation should use an **event-driven simulator** rather than a fixed-time-step simulator, because the time scales of the four loops differ by orders of magnitude (Loop 4 is ~10⁴ times slower than Loop 1 on platform-mediated environments).
- **Multi-scale temporal integration** is essential.
- Standard ABM platforms (**NetLogo**, **Mesa**, **RepastHPC**) are adequate for prototype implementation.
- Scaling to populations larger than 10⁵ requires **distributed computation**.

## Core Equations (Summary)

**Internalization (Loop 1):**

$$I_{k,i,t+1} = I_{k,i,t} + \alpha \cdot w(d_k) \cdot E_{k,i,t} \cdot r_{k,i,t} \cdot \frac{1}{1 + c_{k,t}} \cdot (I_{\max,i} - I_{k,i,t})$$

**Logic Switching:**

$$P(S_{g,t+1} = S \mid u_{g,t}) = \frac{\exp(\beta \cdot v_S^\top u_{g,t})}{\sum_{S'} \exp(\beta \cdot v_{S'}^\top u_{g,t})}$$

**Cross-Subsystem Coupling:**

$$O_{i,t+1} = (1 - \delta) O_{i,t} + \delta \sum_j \gamma_{ji,t} O_{j,t} + \varepsilon_{i,t}$$

**Coupling Matrix Update:**

$$\Gamma_{t+1} = \Gamma_t + \eta \cdot \Delta\Gamma_t - \mu \cdot \text{diag}(B_t)$$

**Performative Reflection (Loop 4):**

$$\text{Programs}_{i,t+\Delta} = \text{Programs}_{i,t} + \varphi \cdot K_t \cdot \psi_i$$
