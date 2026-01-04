# Justin Ralph Bala
**Chemical Engineering at Polytechnique Montréal**

I am a chemical engineering student in the biofabrication/ biomanufacturing stream. This page presents selected projects that reflect my approach to engineering analysis and problem-solving.
My academic projects emphasize using modeling and simulation as tools to understand process behavior

---

## Projects

### Sugar Extraction & Evaporation Process

This academic team project focused on the process understanding, modeling, and simulation of an industrial sugar extraction plant, with emphasis on mass andenergy balances, steady-state operation, and dynamic behavior of evaporator systems.

The work progressed from flowsheet development and plant-wide mass balances to steady-state and transient modeling of a multi-effect evaporator cascade, with the goal of building engineering tools that reflect real operating behavior.

#### Part I - Process Understanding and Process Flow Diagram (PFD)
Literature-based understanding of the sugar extraction process and development of a PFD using Visio from the plant description provided by professors. 

<details>
<summary><strong>Sugar Plant Flowsheet</strong></summary>

** **

![Sugar Plant Flowsheet](assets/sugar_PFD.png)
  
</details>

#### Part II - Plant-Wide Mass Balance & Operator-Oriented Simulator
Development of a plant-wide mass balance and an operator-oriented Excel simulator (VBA/macros) allowing users to define a feed basis and explore operating parameters while preserving calculation integrity.
The goal was to create a tool that reflects how process calculations would be used in practice.

<details>
<summary><strong>Simulator details</strong></summary>

- Feed-flow-based plant-wide mass balance  
- Automated flowrate propagation across all units  
- Parameter variation (air excess, inlet temperatures, etc.)  
- Input constraints and safeguards to prevent calculation errors  

</details>



#### Part III - Steady-State Modelling of an Evaporator Cascade
Steady-state simulation of a five-effect evaporator cascade in series using Aspen HYSYS, including energy integration and sensitivity analysis.

![Aspen HYSYS Simulation](assets/evap_cascade.png)

#### Part IV — Dynamic Evaporator Model

**My contribution**

- Development and analysis of a dynamic evaporator model in Python
- Implementation of steady-state and transient simulations
- Interpretation of process behavior under operating disturbances

**Representative results**

  - Time-dependent temperature, concentration, liquid level and pressure profiles
  - Comparison between steady-state and transient responses
  -  Comparison of different dynamic modeling approaches (nonlinear model, linearized model via Jacobian, and transfer-functions)

<table>
  <tr>
    <td align="center">
      <img src="assets/RP.png" width="800"><br>
      <em>State Variables at Steady-State</em>
    </td>
    <td align="center">
      <img src="assets/per_Tc.png" width="800"><br>
      <em>Effect on State Variables with a 5% increase on Heating Jacket Temperature</em>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="assets/per_deb_liq.png" width="800"><br>
      <em>Effect on State Variables with a 10% increase on Liquid Feed Flowrate</em>
    </td>
    <td align="center">
      <img src="assets/per_fv.png" width="800"><br>
      <em>Effect on State Variables with a 5% decrease on Vapor Outlet Flowrate</em>
    </td>
  </tr>
</table>

<details>
<summary><strong>Discussion</strong></summary>
  
- Thermal variables respond faster than concentration due to accumulation effects.
- Linearized and transfer-function models capture local behavior well but deviate under larger disturbances.
- Dynamic analysis highlights limitations of steady-state-only reasoning.
  
</details>

---

## Skills & Tools

- Python (NumPy, SciPy, Matplotlib)
- Numerical methods (ODEs, finite differences)
- Process modeling & simulation
- Engineering analysis & documentation

---

## Contact
- LinkedIn: [your link]
- GitHub: [your GitHub profile]
