# Common-Source-Amplifier-Analysis

Parametric Sweep Analysis of Common Source Amplifier

This is the Common Source amplifier, where the gate is fed with an AC signal having a DC voltage of 700 mV, an AC magnitude of 5V, and 1 GHz frequency. A bias resistor of 100 ohms is connected to the drain of the MOSFET on one end and a DC source is connected on the other end of resistor. 

<img width="402" height="277" alt="image" src="https://github.com/user-attachments/assets/5d8d70ca-fc89-47c7-888e-269d251183da" />

The output is obtained as follows: 

<img width="755" height="353" alt="image" src="https://github.com/user-attachments/assets/c850b1ec-25db-4c2b-9c70-d8be990f324a" />

To perform parametric sweep analysis of the CS Amplifier, total width of the MOSFET is taken as parameter and the variable assigned to it is Wn. Before simulating, set the initial value of the design variable ‘Wn’ as 1u. To perform the parametric sweep for different values of ‘Wn’, go to ‘Tools’ and click on ‘Parametric Analysis’. Then sweep the variable ‘Wn’ from 1u to 5u in steps of 10.

From this, we can see different values of Vout for different values of Vin.

<img width="940" height="441" alt="image" src="https://github.com/user-attachments/assets/2839728c-81b7-4a26-97fb-60d8c7229dee" />

Cascode Common Source Amplifier

The cascode common source amplifier has 2 input ports: Vbias, Vin, 2 inout ports: vdd, gnd and an output port: Vout. For this cellview, a symbol is created.

<img width="310" height="355" alt="image" src="https://github.com/user-attachments/assets/76607108-4fe1-42af-b458-d8382ac9b0ee" />

In the testbench circuit, the following sources are connected as shown. 

<img width="592" height="425" alt="image" src="https://github.com/user-attachments/assets/da2bfe0c-13a6-4aa2-bb29-78d3a44624d3" />

DC analysis was done by taking the AC source as the component parameter and AC analysis was done from 100Hz to 1GHz. Moderate mode of transient analysis is selected. 3 responses are obtained as shown below after running the simulation.

<img width="940" height="377" alt="image" src="https://github.com/user-attachments/assets/f33ffe99-936a-42a2-be44-608a60c995d8" />

