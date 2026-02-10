# Justin Ralph Bala **Chemical Engineering — Polytechnique Montréal**
Chemical engineering student in the biofabrication / biomanufacturing stream. This page presents selected academic projects that reflect my approach to engineering analysis, modeling, and process understanding, with an emphasis on using simulation tools to study real process behavior. 

--- 
# Projects 
--- 
## Plant-Wide Modeling and Analysis of a Sugar Extraction Process

End-to-end modeling and analysis of an industrial sugar extraction plant, with emphasis on mass and energy balances, steady-state operation, and dynamic behavior of evaporator systems.

**Tools:** Excel (VBA), Aspen HYSYS, Python, MS Visio  
**Focus:** Process modeling · Energy analysis · Dynamic systems

<details>
<summary><em>View project details</em></summary>

### Phase I — Process Understanding & Process Flow Diagram (PFD)

Development of a structured understanding of the sugar extraction process based on technical literature and the plant description provided.  
An industrial-style process flow diagram (PFD) was developed **individually** using MS Visio to represent major unit operations and material flows.

<details>
<summary><em>Figure — Sugar Plant Flowsheet (PFD)</em></summary>

<p align="center">
  <img src="assets/sugar_PFD.png" width="900" alt="Sugar Plant Flowsheet">
</p>
</details>

### Phase II — Plant-Wide Mass Balance & Operator-Oriented Simulator

Design and implementation of a **plant-wide, feed-defined mass balance** in the form of an **operator-oriented Excel simulator** (VBA/macros). The tool allows users to vary operating conditions and observe their impact on the process while maintaining numerical consistency.

<em>I contributed primarily to the mass balance formulation and simulator logic, and later extended the tool with additional input handling and safeguards.</em>

<details>
<summary><em>Simulator Features</em></summary>

<ul>
  <li>Automatic propagation of flowrates across interconnected process units</li>
  <li>User-adjustable operating parameters with protected calculation cells</li>
  <li>Built-in checks to prevent non-physical operating conditions</li>
  <li>Designed for rapid “what-if” analysis rather than detailed optimization</li>
</ul>
</details>

### Phase III — Steady-State Modeling of an Evaporator Cascade

Steady-state simulation of a **five-effect evaporator cascade** operating in series using Aspen HYSYS.  
The model incorporated energy integration and was used to perform sensitivity analyses on key operating parameters. This phase was completed **individually**.

<p align="center">
  <img src="assets/evap_cascade.png" width="700" alt="Five-effect evaporator cascade">
</p>

### Phase IV — Dynamic Modeling of an Evaporator System

Dynamic modeling of a **single evaporator unit** to analyze transient behavior under operating disturbances.  
The system was represented by a coupled set of ordinary differential equations describing liquid concentration, pressure, temperature, and liquid level.

**My contribution**
- Development of a nonlinear dynamic evaporator model in Python
- Implementation of steady-state and transient simulations
- Linearization around steady state and derivation of transfer-function representations
- Interpretation of process behavior under controlled disturbances

**Representative results**
- Time-dependent profiles of temperature, concentration, liquid level, and pressure
- Transient responses to step changes in operating conditions
- Comparison between steady-state predictions and dynamic behavior
- Comparison of nonlinear, linearized, and transfer-function-based models

<table>
  <tr>
    <td align="center">
      <img src="assets/RP.png" width="750"><br>
      <em>State variables at steady state</em>
    </td>
    <td align="center">
      <img src="assets/per_Tc.png" width="750"><br>
      <em>Effect of a 5% increase in heating jacket temperature</em>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="assets/per_deb_liq.png" width="750"><br>
      <em>Effect of a 10% increase in liquid feed flowrate</em>
    </td>
    <td align="center">
      <img src="assets/per_fv.png" width="750"><br>
      <em>Effect of a 5% decrease in vapor outlet flowrate</em>
    </td>
  </tr>
</table>

</details>
