<div align="center">

# Coupled Functional Differentiation (CFD)

### A Mechanism-Based, Formalized, and Falsifiable Theory of the Multi-Level Human Social System

[![License: GPL v3](https://img.shields.io/badge/License-GPL_v3-blue.svg)](LICENSE)
[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC_BY--NC_4.0-lightgrey.svg)](LICENSE-DOCS) 

[![Status: Preprint](https://img.shields.io/badge/Status-Preprint-orange.svg)](#disclaimer)

</div>

> [!IMPORTANT]
> **Disclaimer:** This is an independent working paper/preprint. It has not undergone peer review, and all claims are provisional and subject to revision based on future empirical testing and community critique. This preliminary framework is submitted for open community feedback and pending empirical validation.


<div align="center">

## Executive Summary

Modern societies exhibit a paradox: their functionally differentiated subsystems (law, economy, politics, science, religion, aesthetics, media) display pronounced operational autonomy — a judge does not optimize for profit, a peer reviewer does not campaign for votes — yet these same subsystems are bound together by increasingly tight, fast, and consequential interdependencies. Financial shocks reshape political legitimation in days; algorithmic media selection rewrites political discourse in hours; legal classifications gate economic credit. Existing theories tend to resolve this tension by either collapsing the differentiation (reductionism) or cataloguing it without explaining the coupling (descriptive pluralism).

This paper proposes a third option. It specifies a single **Core Generative Mechanism (CGM)**: functionally differentiated subsystems, each operating under a distinctive binary code and programs, engage in *selective and asymmetric structural coupling* through identifiable communication channels. This coupling simultaneously produces coordination across subsystems and tension between codes. Both outputs feed back onto individual cognition (through internalization) and onto small-group dynamics (through situationally triggered switching among Fiske's four relational logics).

The **ego** — the layered biological-cognitive-affective-motivational complex of the individual, organized around survival, recognition, and status, with affective valence on an approach/avoidance (love/fear) axis — is the locus where the four loops of this mechanism meet. The aggregate institutional layer functions as a **Social Operating System**: ideology and religion serve as the categorical glue allowing millions of unacquainted egos to coordinate; the legal subsystem replaces personal revenge with formal procedure; money operates as a "religion of trust." At the global scale, the joint operation of these loops constitutes a **modern Leviathan** — a globally coupled multi-system network following the canonical loop: money → technology → ideology → education → ego → system → money.

From the single CGM, we derive the conditions for subsystem colonization, small-group logic flipping, globally synchronized crises, and surveillance-capitalist erosion of reflective autonomy. The theory is formalized through a system of difference equations, specified computationally through an Agent-Based Model (COFD-ABM), and yields **sixteen directional, falsifiable propositions** including an explicit falsification criterion.

</div>

## Core Generative Mechanism

> Functionally differentiated subsystems, each operating under a distinctive binary code and a set of programs, engage in selective and asymmetric structural coupling through identifiable communication channels. This coupling produces, simultaneously: (i) coordination across subsystems sufficient for joint operation, and (ii) tension between codes that propagates through the channels. Both outputs feed back onto individual cognition through internalization and onto small-group dynamics through situationally triggered switching among four relational logics.

## The Four Loops

| Loop | Direction | Mechanism | Key Concept |
|------|-----------|-----------|-------------|
| **Loop 1** | Macro → Micro | Internalization | Subsystem codes deposited into ego via schooling, media, contracts, platforms |
| **Loop 2** | Micro → Macro | Aggregation | Individual decisions, filtered through group logic, aggregate via markets, elections, science |
| **Loop 3** | Meso ↔ Meso | Horizontal coupling | Coordination and tension across subsystems via institutional bridges (contracts, taxes, algorithms) |
| **Loop 4** | System → System | Self-reflection | Social-scientific knowledge changes the system it describes (performativity) |

## 16 Propositions at a Glance

| # | Short Title | Level | Loop |
|---|-------------|-------|------|
| P1 | Resource scarcity displaces EM → MP | Group | 2 |
| P2 | Complex emotions vary more cross-culturally than basic | Individual | 1 |
| P3 | Tight coupling → synchronized crises | System | 3 |
| P4 | Colonization signatures detectable via NLP | System | 3 |
| P5 | Loop 2 severing → elite-population divergence | System | 2 |
| P6 | Developmental windows accelerate internalization | Individual | 1 |
| P7 | Coupling speed → systemic volatility | System | 3 |
| P8 | Status cues activate Authority Ranking | Group | 2 |
| P9 | Platform mediation erodes reflective autonomy | Platform | 1–4 |
| P10 | Economy-politics coupling: stability vs. capture | System | 3 |
| P11 | Code-switching overload → anomie | Individual | 1 |
| P12 | Threat + homogeneity activates Communal Sharing | Group | 2 |
| P13 | Training in theory shifts behavior toward theory | Loop 4 | 4 |
| P14 | Buffering reduces contagion non-linearly | System | 3 |
| P15 | Coleman-boat time-constant asymmetry | Individual | 1–2 |
| P16 | **Falsification criterion** | System | All |



## Repository Structure

```
Coupled-Functional-Differentiation/
├── README.md                              ← You are here
├── README_he.md                           ← Hebrew summary (RTL)
├── LICENSE                                ← GPL-3.0 License for code
├── LICENSE-DOCS                           ← CC BY-NC 4.0 License for docs
├── CITATION.cff                           ← Citation metadata
├── paper/
│   ├── CFD_main_paper.md                  ← Full paper (Markdown)
│   ├── CFD_main_paper.tex                 ← Full paper (LaTeX source)
│   └── references.bib                     ← BibTeX bibliography
├── abm/
│   └── COFD-ABM_specification.md          ← Agent-Based Model spec
├── propositions/
│   └── 16_propositions.md                 ← Extended proposition table
├── translations/
│   ├── hebrew/                            ← Original Hebrew documents
│   │   ├── Coupled_Human_Systems_Hebrew.md
│   │   ├── Humanity_Crossroads_Hebrew.md
│   │   └── Theory_Human_System_Hebrew.md
│   └── english/                           ← Full English translations
│       ├── Coupled_Human_Systems.md
│       ├── Humanity_Crossroads.md
│       └── Theory_Human_System.md
├── figures/                               ← Placeholder for diagrams
│   └── README.md
└── docs/
    └── comparison_with_rival_theories.md  ← Comparison with 4 rival traditions
```

## Building the PDF

The LaTeX source can be compiled to PDF:

```bash
cd paper/
pdflatex CFD_main_paper.tex
bibtex CFD_main_paper
pdflatex CFD_main_paper.tex
pdflatex CFD_main_paper.tex
```

Requires a standard LaTeX distribution (TeX Live, MiKTeX) with packages: `amsmath`, `amssymb`, `booktabs`, `longtable`, `natbib`, `hyperref`, `geometry`, `setspace`, `microtype`.

## How to Cite

```bibtex
@misc{Schwartz2026CFD,
  author       = {Schwartz, Liran M.},
  title        = {Coupled Functional Differentiation: A Mechanism-Based Theory
                  of the Multi-Level Human System},
  year         = {2026},
  version      = {v2.0},
  note         = {Working paper / preprint. Not peer-reviewed.},
  url          = {https://github.com/LiranOG/Coupled-Functional-Differentiation}
}
```

Or in prose:

> Schwartz, L. M. (2026). *Coupled Functional Differentiation: A Mechanism-Based Theory of the Multi-Level Human System* (v2.0). Working paper / preprint.

## Contributing

This is an open preprint. Contributions, critiques, and empirical tests are welcome:

1. **Theoretical critique:** Open an issue describing where the CGM or its derivations fail.
2. **Empirical testing:** If you test any of the 16 propositions, please share results via issue or PR.
3. **Formalization:** Improvements to the equation system or ABM specification are welcome.
4. **Translation:** Corrections to the Hebrew-English translations are appreciated.

## License

This repository uses a dual-license model:

| Component | License | Applies To |
|-----------|---------|------------|
| Source code | [GPL-3.0](https://www.gnu.org/licenses/gpl-3.0) | All `.py`, `.cpp`, `.js`, and other executable files |
| Documentation & theory | [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/) | Paper, ABM specification, propositions, translations, and comparison documents |

## Author

**Liran M. Schwartz**
Independent Researcher, Haifa, Israel
ORCID: [0009-0008-8035-1308](https://orcid.org/0009-0008-8035-1308)
