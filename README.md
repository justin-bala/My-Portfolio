# Justin Ralph Bala
**Chemical Engineering — Polytechnique Montréal**

Chemical engineering student in the biofabrication / biomanufacturing stream. This page presents selected academic projects that reflect my approach to engineering analysis, modeling, and process understanding, with an emphasis on using simulation tools to study real process behavior.

---

## Projects

### Sugar Extraction & Evaporation Process

This academic team project focused on the process understanding, modeling, and simulation
of an industrial sugar extraction plant, with emphasis on mass and energy balances,
steady-state operation, and dynamic behavior of evaporator systems.

The work progressed from flowsheet development and plant-wide mass balances to steady-state and transient modeling of a multi-effect evaporator cascade, with the goal of building engineering tools that reflect real operating behavior.

---

#### Part I — Process Understanding & Process Flow Diagram (PFD)

Literature-based understanding of the sugar extraction process and development of a process flow diagram (PFD) from the plant description provided by the instructors. The PFD was developed individually.

<details>
<summary><strong>Sugar Plant Flowsheet (PFD)</strong></summary>

<p align="center">
  <img src="assets/sugar_PFD.png" width="900" alt="Sugar Plant Flowsheet">
</p>

</details>

---

#### Part II — Plant-Wide Mass Balance & Operator-Oriented Simulator

Development of a plant-wide mass balance and an operator-oriented Excel simulator (VBA/macros) allowing users to define a feed basis and explore operating parameters while preserving calculation integrity. 
I contributed primarily to the mass balance  implementation and simulator logic. Additional improvements to usability and input handling were implemented independently following the project.

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

Steady-state simulation of a five-effect evaporator cascade operating in series using Aspen HYSYS, including energy integration and sensitivity analysis. This portion of the project was completed individually.

<p align="center">
  <img src="assets/evap_cascade.png" width="700" alt="Five-effect evaporator cascade">
</p>

---

#### Part IV — Dynamic Evaporator Model

In this final phase, a single evaporator system was modeled dynamically to analyze transient behavior under disturbances, using a coupled system of four ordinary differential equations representing concentration, pressure, temperature, and liquid level.

**My contribution**
- Development and analysis of a dynamic evaporator model in Python
- Implementation of steady-state and transient simulations
- Interpretation of process behavior under operating disturbances

**Representative results**
- Time-dependent temperature, concentration, liquid level, and pressure profiles
- Transient responses to controlled step disturbances in operating conditions
- Comparison between steady-state predictions and dynamic behavior
- Comparison of different dynamic modeling approaches (nonlinear model, linearized model via Jacobian, and transfer-function representations)

<table>
  <tr>
    <td align="center">
      <img src="assets/RP.png" width="650"><br>
      <em>State variables at steady state</em>
    </td>
    <td align="center">
      <img src="assets/per_Tc.png" width="650"><br>
      <em>Effect of a 5% increase in heating jacket temperature</em>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="assets/per_deb_liq.png" width="650"><br>
      <em>Effect of a 10% increase in liquid feed flowrate</em>
    </td>
    <td align="center">
      <img src="assets/per_fv.png" width="650"><br>
      <em>Effect of a 5% decrease in vapor outlet flowrate</em>
    </td>
  </tr>
</table>

<details>
<summary><strong>Key findings</strong></summary>

<ul style="list-style-type: disc; padding-left: 1.2em;">
  <li>Linearized and transfer-function models produced identical responses, as expected, while deviations from the nonlinear model were observed for certain disturbances and state variables.</li>
  <li>An increase in liquid feed flow rate led to liquid accumulation, reduced evaporation, and a decrease in outlet concentration; only the nonlinear model consistently captured the expected physical behavior.</li>
  <li>An increase in heating jacket temperature enhanced evaporation, increased pressure and temperature, and resulted in a higher outlet concentration, making this disturbance the most favorable from an operational standpoint.</li>
  <li>A reduction in vapor outlet flow caused vapor accumulation, increased pressure and boiling temperature, and slowed evaporation, ultimately reducing outlet concentration.</li>
  <li>Dynamic simulations highlighted strong coupling between heat input, evaporation rate, pressure, and liquid inventory, revealing behaviors not observable through steady-state analysis alone.</li>
</ul>

</details>


---

## Skills & Tools

- Python (NumPy, SciPy, Matplotlib)
- Numerical methods for differential equations
- Process modeling & simulation
- Aspen HYSYS
- Engineering analysis & technical documentation

---

## Contact

- LinkedIn: [your LinkedIn link]
- GitHub: [your GitHub profile]
