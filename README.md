# Justin Ralph Bala
**Chemical Engineering at Polytechnique Montréal**

I am a chemical engineering student in the biofabrication/ biomanufacturing stream. This page presents selected projects that reflect my approach to engineering analysis and problem-solving.
My academic projects emphasize using modeling and simulation as tools to understand process behavior

---

## Projects

### Sugar Extraction & Evaporation Process

This academic team project involved the process understanding, modeling, and simulation of an industrial sugar extraction plant, with a focus on mass and energy balances, steady-state operation, and dynamic behavior of evaporator systems.

The work progressed from process analysis and process flow diagram (PFD) development, through plant-wide mass balance implementation, to steady-state and transient modeling of a multi-effect evaporator cascade.
The objective was not only to obtain numerical results, but to build engineering tools and models that reflect real operating behavior and can be used for analysis and decision-making.

#### Part I - Process Understanding and Process Flow Diagram (PFD)
The first part of the project focused on the understand the overall sugar extraction process through literature review, then a PFD was developed using Visio from the plant description provided by professors. 
![Sugar Plant Flowsheet](assets/sugar_PFD.pdf)

#### Part II - Plant-Wide Mass Balance & Operator-Oriented Simulator
Using the developed flowsheet, mass balances were calculated across the entire plant, linking all major units and process streams.
To operationalize these calculations, a plant-wide simulator was developed in Excel using VBA and macros.

The simulator allows users to:
    - define a basis flowrate of the primary feed
    - automatically compute flowrates throughout all downstream equipment
    - modify operating parameters such as air excess, inlet temperatures, and other process conditions

The goal was to create a tool that reflects how process calculations would be used in practice.
#### Part III - Steady-State Modelling of an Evaporator Cascade
In the third phase, the evaporation section of the plant was modeled in more detail.
A five-effect evaporator cascade operating in series was simulated at steady state using Aspen HYSYS.

![Aspen HYSYS Simulation](assets/evap_cascade.png)

#### Part IV - Dynamic Evaporator Model
Finally, the evaporator system was modeled dynamically to study transient behavior under operating disturbances.

**What I did**
- Developed and analyzed a dynamic evaporator model in Python
- Implemented steady-state and transient simulations
- Interpreted process behavior under changing operating conditions

**Key results**
- Time-dependent temperature and concentration profiles
- Comparison between steady-state and dynamic behavior

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


</details>
---

### Thermal Cable Model
**Context:** Academic team project (Numerical Modeling)  
**Focus:** Heat transfer, finite-difference methods

**What I did**
- Implemented a finite-difference thermal model in Python
- Simulated transient temperature evolution in a cable
- Studied the effect of material properties and boundary conditions

**Key results**
- Radial temperature profiles
- Sensitivity to thermal parameters

**Links**
- 📄 Report (PDF)
- 📊 Results & figures
- 💻 Code

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
