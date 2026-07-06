# nanofluidic-ion-transport-poster
Research poster presented at Ben-Gurion University, detailing analytical and numerical COMSOL modeling of gate-voltage-controlled ion transport in dielectric-embedded nanochannels.

# Electrostatic Gating of Nanochannels Embedded by a Dielectric Material

## Research Poster Presentation
**Fluid Mechanics Laboratory (FML), Ben-Gurion University of the Negev** 
**Authors:** Nave Markovich and Prof. Yoav Green

🏆 *Supported by the Israel Science Foundation (ISF) via grants 337/20 and 1953/20.*

---

### 📊 Poster Overview
This repository hosts the research poster detailing our comprehensive analytical and numerical framework for gate-voltage-controlled ($V_{\text{gate}}$) ion transport within dielectric-embedded nanochannels. By investigating the coupled interplay between electrostatics in the surrounding dielectric shell and electrokinetics inside the fluidic channel, we elucidate how external gating modulates internal potential fields, ionic charge distribution, and conductance.

---

### 🔍 View Research Poster

<img width="3402" height="4536" alt="Poster" src="https://github.com/user-attachments/assets/24058e1b-3584-41d9-b969-c1a5a7117618" />


---

### 🔬 Core Methodology & Governing Equations
Our study evaluates a steady-state, convection-less symmetric binary electrolyte ($D_{\pm} = D$ and $z_{\pm} = \pm z$) described by non-dimensional **Poisson-Boltzmann equations**:[cite: 3]

$$\frac{2\epsilon^{2}}{r}(r\phi_{m})_{r} = -(e^{-\phi} - e^{\phi})$$

Where $\epsilon$ represents the non-dimensional Debye length:

$$\epsilon = \frac{\tilde{\lambda}_D}{\tilde{a}_{\text{in}}} = \frac{1}{\tilde{a}_{\text{in}}}\sqrt{\frac{\tilde{\varepsilon}_0\varepsilon_r R \tilde{T}}{2\tilde{F}^2 z^2 \tilde{c}_0}}$$

Analytical models were developed under a finite-gate boundary condition $\phi(a_{\text{out}}) = V_g$ split into two structural branches:
* **Model-1:** Valid over low-to-moderate high-voltage regimes ($-100 \le V_g \le V_{\text{crit}}$).
* **Model-2:** Valid over the highly positive high-voltage regime ($V_{\text{crit}} < V_g \le 100$).
---

### 📈 Key Results & Findings (Validated via COMSOL)
Analytical models (solid/dashed lines) demonstrate exceptional agreement when validated against numerical **COMSOL Multiphysics** simulations (markers):

* **Potential Distribution:** Modulating $V_g$ successfully shifts internal electrostatic fields across both positive and negative voltage ranges.
* **Charge Inversion & Suppressed Conductance:** High positive gate voltages strongly suppress ion transport, decreasing the excess counterion concentration and reducing effective conductance by several orders of magnitude. The rise in $|Q_{\text{in}}|$ at extreme voltages suggests charge inversion.
* **Electrostatic Selectivity:** At low surface charge densities, increasing $|V_g|$ allows the gate voltage to overcome surface-charge-dominated responses, steering the nanochannel toward gate-induced electrostatic selectivity.

## 📂 Software & Tools Used
* **COMSOL Multiphysics** (Finite Element numerical simulations)
* **Wolfram Mathematica / MATLAB** (Analytical modeling and data plotting)
