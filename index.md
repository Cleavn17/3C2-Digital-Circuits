# Digital Circuits

* Read the quesiton thoroughly
* Expected to get one guranteed quesiton on quantum circuits in the first question subsections
* Practise all the tutorials

For exam:
* Question 1a:
  * Will generally be cuboidal
  * Normally in centimeter

## Past Paper Analysis

**(!)** means its repeated 

**2023-2024**

* Question 1
  * a) Sketch Diagram and find current (semiconductors)
  * b) CMOS to drive LED
  * c) Solve BJT circuit to find load Resistor **(!)**
  * d) Mosfet question **(!)**
  * e) CMOS logic to implment boolean function
  
* Question 2
  * a) BJT to drive LED (buffer circuit) **(!)**
  * b) Design the circuit **(!)**
  
* Question 3
  * a) Find the model of the MOSFET transistor and draw transfer characteristic graph **(!)**
  * b) Find an experission for Output Voltage **(!)**
  * c) Calculate Power **(!)**
  
* Question 4 **(! but different values)**
  * a) CMOS inverter, find the transfer characteristic **(!)**
  * b) Relationship between channel width, then steady state current, then **(!)** find power **(!)**
  * c) Design a circuit to fit a description **(!)**

**2022-2023**

* Question 1
  * a) Doping concentration and doping type (semiconductors)
  * b) Diode model behvaiour and ratio of saturation currents
  * c) Solve BJT circuit to find load Resistor **(!)**
  * d) Mosfet question **(!)**
  * e) CMOS logic to find the boolean function **(! but different circuit)**
  
* Question 2
  * a) BJT to drive LED (buffer circuit) **(!)**
  * b) Design the circuit **(!)**
  
* Question 3
  * a) Find the model of the MOSFET transistor and draw transfer characteristic graph **(!)**
  * b) Find an experission for Output Voltage **(!)**
  * c) Calculate Power **(!)**
  
* Question 4 **(! but different values)**
  * a) CMOS inverter, find the transfer characteristic **(!)**
  * b) Relationship between channel width, then steady state current, then  find power **(!)**
  * c) Design a circuit to fit a description **(!)**
  
**2021-2022**

* Question 1
  * a) Doping concentration and doping type (semiconductors) **(!)**
  * b) Diode model behvaiour and current and doping concentration
  * c) Solve BJT circuit with load capacitor
  * d) Mosfet question **(!)**
  * e) CMOS logic to find the boolean function **(! but different circuit)**
  
* Question 2
  * a) BJT inverter and state 
  * b) Calculate the voltage min input High
  * c) Derive the fanout of the transistor
  * d) Calculate base resistance
  
* Question 3
  * a) BJT, find the voltages 
  * b) Calculate Quiescent Current
  
* Question 4 **(! but different circuit)**
  * a) CMOS inverter, find the transfer characteristic **(!)**
  * b) Relationship between channel width, then steady state current, then find power **(!)**
  * c) Design a circuit to fit a description **(!)**
  

## Question 1a
* If in the question electric field is there then the current to calculate is drift current.

### Law of Mass Action 

$n_{o}$$p_{o}$ = $n_{i}^{2}$
 
where:
* $n_{o}$ is the concentration of free electrons 
* $p_{o}$ is the concentration of holes
* $n_{i}$ is the intrinsic carrier concentration

For intrinsic silicon at room temperature:

* $n_{o}$ = $p_{o}$ ~ 1.5 x $10^{10}$ $cm^{-3}$
* $n_{i}^{2}$ ~ 2.25 x $10^{20}$

### Law of Mass Action: N-type

The law of mass action still applies

$n_{o}$$p_{o}$ = $n_{i}^{2}$

For n-type, the concentration of free electrons is much higher than for intrinsic silicon
due to doping, hence:

$n_{o}$ = $N_{d}$ >> $n_{i}$

$p_{o}$ = $n_{i}^{2}$/$N_{d}$ << $n_{i}$

if $N_{d}$ ~ 1 x $10^{13}$ $cm^{-3}$ and $n_{i}$ ~ 1.5 x $10^{10}$ $cm^{-3}$, $p_{o}$ is approximately 700 times smaller than $n_{o}$.

### Law of Mass Action: P-type

The law of mass action still applies

$n_{o}$$p_{o}$ = $n_{i}^{2}$

For p-type, the concentration of holes is much higher than for intrinsic silicon
due to doping, hence:

$p_{o}$ = $N_{a}$ >> $n_{i}$

$n_{o}$ = $n_{i}^{2}$/$N_{a}$ << $n_{i}$

if $N_{a}$ ~ 1 x $10^{13}$ $cm^{-3}$ and $n_{i}$ ~ 1.5 x $10^{10}$ $cm^{-3}$, $n_{o}$ is approximately 700 times smaller than $p_{o}$.

### Quantifying the Electron Drift Current
#### Charge flux Density ($J^{drift}$)
The average charge flow per unit area in the direction on the field

For electrons: 
$J^{drift}_{n}$ = -nq$\mu_{n}$E

where:
* n is the density of electrons
* q is the charge on the electron(negative)
* $\mu_{n}$ is the mobility of the electron
* E is the electric field.

> **Note**: The sign of the carrier is already present so just need to put the value of q in. Not sure yet

### Quantifying the Hole Drift Current
#### Charge flux Density ($J^{drift}$)
The average charge flow per unit area in the direction on the field

For electrons: 
$J^{drift}_{p}$ = pq$\mu_{p}$E

where:
* p is the density of holes
* q is the charge on the electron(positive)
* $\mu_{n}$ is the mobility of the hole
* E is the electric field.

> **Note**: The sign of the carrier is already present so just need to put the value of q in. Not sure yet

### Combined Drift Current

THe drift current ($I^{drift}$) is the charge flux density ($J^{drift}$) integrated over the area **A**. 

The total drift current ($I^{drift}$) has two components:
* Net movement of electrons $I^{drift}_{n}$
* Net movement of holes $I^{drift}_{p}$

moving in opposite directions

```math
I^{drift} = I^{drift}_n + I^{drift}_p \\
= J^{drift}_nA + J^{drift}_pA \\
= -n(-q)(\mu_n)EA + p(q)(\mu_p)EA \\
= AEq(n\mu_n + p\mu_p)
```

> NOTE: The above statements for drift current and current flux density is only valid for unifrom electron density inside a semiconductor.   

### Different types

if it is mentioned that it is p type or n type do normally by finding drift current. 

If it is intrinsic Silicon do the below

**Intrinsic Silicon**

n = p = $n_{i}^{2}$

If its not either then just do  