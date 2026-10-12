# Dissipative Topological Protection of Peptide Backbone Wavefunctions

Theoretical simulation suite and multi-system parameter data mapping the emergence of long-lived amide-I vibrational phase coherence plateaus across distinct human amyloidogenic models under high-temperature physiological noise regimes.

## 🧬 Framework Context
This repository contains the open-source python execution validation tools accompanying the theoretical research submission:
**"Dissipative Topological Protection of Peptide Backbone Wavefunctions: A Comparative Non-Hermitian Structural Framework Across Pathological Proteopathies"** (Submitted for editorial review to *Protein Engineering, Design and Selection*, Oxford University Press).

The framework implements a Markovian open quantum system integration engine solving the Liouville-von Neumann Lindblad Master Equation across three independent disease models parameterized from high-resolution repositories:
* **System I (Amyloid-β 1-42):** Mapped to the central hydrophobic core segment (`PDB ID: 2LFM`)
* **System II (α-Synuclein):** Mapped across the amyloidogenic NAC region core (`PDB ID: 2N0A`)
* **System III (Human IAPP):** Mapped to the highly cytotoxic core domain (`PDB ID: 2L86`)

## 🛠️ Execution & Environment Setup
The simulation engine utilizes standard, open-source linear algebra and mathematical visualization toolsets. To install the required dependencies, execute via your terminal:
```bash
pip install numpy scipy matplotlib
```

To run the open-system trajectory integration loop and generate the multi-system comparison metrics file (`image_3CEggt.png`):
```bash
python simulation_engine.py
```

## 📊 Core Performance Metrics
Under an aggressive physiological dephasing noise baseline ($\gamma_{\phi} = 5.0 \text{ ps}^{-1}$ at $310\text{ K}$), standard classical configurations yield sub-picosecond phase collapse. Incorporating asymmetric solvent shielding profiles drives the backbones near non-Hermitian Exceptional Points, establishing a protected subspace:

| Target System Parameter Context | Coherence Amplitude (t = 10.0 ps) | Asymptotic Phase Survival Rate |
| :--- | :--- | :--- |
| **Classical Thermal Control (Isotropic)** | 0.000 | 0.00% |
| **System I (Amyloid-β 1-42 DTP Space)** | 0.441 | 88.2% |
| **System II (α-Synuclein NAC DTP Space)** | 0.432 | 86.4% |
| **System III (Human IAPP Core DTP Space)** | 0.448 | 89.6% |

## ⚖️ Open Science License & Attribution
This software architecture is distributed under the MIT License. All structural models, matrix coefficients, and data parsing equations are original derivations developed for academic peer-review verification.
