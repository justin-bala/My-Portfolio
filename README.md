# Justin Ralph Bala
**Chemical Engineering — Polytechnique Montréal**

Chemical engineering student in the biofabrication / biomanufacturing stream.
This page presents selected academic projects that reflect my approach to engineering
analysis, modeling, and process understanding, with an emphasis on using simulation
tools to study real process behavior.

---

## Projects

### Sugar Extraction & Evaporation Process

This academic team project focused on the process understanding, modeling, and simulation
of an industrial sugar extraction plant, with emphasis on mass and energy balances,
steady-state operation, and dynamic behavior of evaporator systems.

The work progressed from flowsheet development and plant-wide mass balances to
steady-state and transient modeling of a multi-effect evaporator cascade, with the goal
of building engineering tools that reflect real operating behavior.

---

#### Part I — Process Understanding & Process Flow Diagram (PFD)

Literature-based understanding of the sugar extraction process and development of a
process flow diagram (PFD) from the plant description provided by the instructors.

<details>
<summary><strong>Sugar Plant Flowsheet (PFD)</strong></summary>

<p align="center">
  <img src="assets/sugar_PFD.png" width="900" alt="Sugar Plant Flowsheet">
</p>

</details>

---

#### Part II — Plant-Wide Mass Balance & Operator-Oriented Simulator

Development of a plant-wide mass balance and an operator-oriented Excel simulator
(VBA/macros) allowing users to define a feed basis and explore operating parameters
while preserving calculation integrity.

<details>
<summary><strong>Simulator details</strong></summary>

<ul style="list-style-type: disc; padding-left: 1.2em;">
  <li>Feed-flow-based plant-wide mass balance</li>
  <li>Automated flowrate propagation across all process units</li>
  <li>Parameter variation (air excess, inlet temperatures, etc.)</li>
  <li>Input constraints and safeguards to prevent calculation errors</li>
</ul>

</details>

---

#### Part III — Steady-State Modeling of an Evaporator Cascade

Steady-state simulation of a five-effect evaporator cascade operating in series using
Aspen HYSYS, including energy integration and sensitivity analysis.

<p align="center">
  <img src="assets/evap_cascade.png" width="700" alt="Five-effect evaporator cascade">
</p>

---

#### Part IV — Dynamic Evaporator Model

**My contribution**
- Development and analysis of a dynamic evaporator model in Python
- Implementation of steady-state and transient simulations
- Comparison of different dynamic modeling approaches (nonlinear model, linearized model via Jacobian, and transfer-function representations)
- Interpretation of process behavior under operating disturbances

**Representative results**
- Time-dependent temperature, concentration, liquid level, and pressure profiles
- Comparison between steady-state and transient responses
- Evaluation of model fidelity under different disturbance magnitudes

<table>
  <tr>
    <td align="center">
      <img src="assets/RP.png" width="550"><br>
      <em>State variables at steady state</em>
    </td>
    <td align="center">
      <img src="assets/per_Tc.png" width="550"><br>
      <em>Effect of a 5% increase in heating jacket temperature</em>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="assets/per_deb_liq.png" width="550"><br>
      <em>Effect of a 10% increase in liquid feed flowrate</em>
    </td>
    <td align="center">
      <img src="assets/per_fv.png" width="550"><br>
      <em>Effect of a 5% decrease in vapor outlet flowrate</em>
    </td>
  </tr>
</table>

<details>
<summary><strong>Discussion</strong></summary>

<ul style="list-style-type: disc; padding-left: 1.2em;">
  <li>Thermal variables respond faster than concentration due to accumulation effects.</li>
  <li>Linearized and transfer-function models capture local behavior but deviate under larger disturbances.</li>
  <li>Dynamic analysis highlights limitations of steady-state-only reasoning.</li>
</ul>

</details>

---

## Skills & Tools

- Python (NumPy, SciPy, Matplotlib)
- Numerical methods for differential equations
- Process modeling & simulation
- Engineering analysis & technical documentation

---

## Contact

- LinkedIn: [your LinkedIn link]
- GitHub: [your GitHub profile]
