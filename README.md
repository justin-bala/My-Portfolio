# Justin Ralph Bala
**Chemical Engineering — Polytechnique Montréal**

Chemical engineering student in the biofabrication / biomanufacturing stream. This page presents selected academic projects that reflect my approach to engineering analysis, modeling, and process understanding, with an emphasis on using simulation tools to study real process behavior.

---

## Projects

---

### Plant-Wide Modeling and Analysis of a Sugar Extraction Process

End-to-end modeling and analysis of an industrial sugar extraction plant, with emphasis on mass and energy balances, steady-state operation, and dynamic behavior of evaporator systems.

**Tools:** Excel (VBA), Aspen HYSYS, Python, MS Visio 

**Focus:** Process modeling · Energy analysis · Dynamic systems

<details>
  
<summary><strong>View project details</strong></summary>


#### Phase I — Process Understanding & Process Flow Diagram (PFD)

Development of a structured understanding of the sugar extraction process based on technical literature and the plant description provided.  
An industrial-style process flow diagram (PFD) was developed **individually** using MS Visio to represent major unit operations and material flows.

  <details>
    
  <summary><strong>Sugar Plant Flowsheet (PFD)</strong></summary>
  
  <p align="center">
    <img src="assets/sugar_PFD.png" width="900" alt="Sugar Plant Flowsheet">
  </p>
  
  </details>


#### Phase II — Plant-Wide Mass Balance & Operator-Oriented Simulator

Design and implementation of a **plant-wide mass balance** coupled with an **operator-oriented Excel simulator** (VBA/macros), allowing users to define a feed basis and explore operating conditions while preserving calculation integrity.

My primary contribution focused on the **mass balance formulation and simulator logic**, including flow propagation and numerical consistency.  
Additional improvements to usability, input handling, and safeguards were implemented **independently after the project**.

  <details>
    
  <summary><strong>Simulator features</strong></summary>
  
  <ul>
    <li>Feed-based plant-wide mass balance</li>
    <li>Automated flowrate propagation across interconnected process units</li>
    <li>Parameter variation (air excess, inlet temperatures, operating conditions)</li>
    <li>Input constraints and safeguards to prevent non-physical or unstable calculations</li>
  </ul>
  
  </details>


#### Phase III — Steady-State Modeling of an Evaporator Cascade

Steady-state simulation of a **five-effect evaporator cascade** operating in series using Aspen HYSYS.  
The model incorporated energy integration and was used to perform sensitivity analyses on key operating parameters. This phase was completed **individually**.

<p align="center">
  <img src="assets/evap_cascade.png" width="700" alt="Five-effect evaporator cascade">
</p>


#### Phase IV — Dynamic Modeling of an Evaporator System

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
    
  <summary><strong>Key technical observations</strong></summary>
  
  <ul>
    <li>Linearized and transfer-function models produced identical responses, as expected, while deviations from the nonlinear model were observed for certain disturbances and state variables.</li>
    <li>An increase in liquid feed flow led to liquid accumulation, reduced evaporation, and a decrease in outlet concentration; only the nonlinear model consistently captured the expected physical behavior.</li>
    <li>An increase in heating jacket temperature enhanced evaporation, increased pressure and temperature, and resulted in a higher outlet concentration, making this disturbance the most favorable from an operational standpoint.</li>
    <li>A reduction in vapor outlet flow caused vapor accumulation, increased pressure and boiling temperature, and slowed evaporation, ultimately reducing outlet concentration.</li>
    <li>Dynamic simulations highlighted strong coupling between heat input, evaporation rate, pressure, and liquid inventory, revealing behaviors not observable through steady-state analysis alone.</li>
  </ul>
  
  </details>

---

</details>

---

## Skills & Tools Demonstrated

- Python (NumPy, SciPy, Matplotlib)  
- Numerical solution of ordinary differential equations  
- Process modeling and simulation  
- Aspen HYSYS  
- Mass and energy balance implementation  
- Technical analysis and documentation  


---

## Contact

- LinkedIn: https://www.linkedin.com/in/justinralph-bala  
- GitHub: https://github.com/Justin-Bala

