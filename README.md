# Lab-2: Basic Circuits
* Hannah Markwell 
* Alexis Puckett

January 25, 2024

PROJECT SUMMARY 

This lab allowed for a couple of overall objectives and knowledge to be learned and obtained. For this lab, the idea of Kirchhoff’s voltage law (KVL) and Kirchhoff’s current law (KCL) and using Thevenin and superposition theorems on the circuits that were constructed were the objectives that were tested and learned. In order to test these objectives, a series of differing circuits were constructed and measured. First, the act of soldering was introduced. This technique was demonstrated by constructing a simple series circuit and soldering cables and resistors. Soldering would allow us to connect the DC power supply and the multimeter to gain accurate measurements. For KCL, the current drop across resistors in a parallel circuit was measured using the DMM. And for KVL, we measure the voltage drop across varying resistors in the same circuit. When it came to Thevenin’s Theorem we had to make a series of calculations in order to determine the voltage and resistance with a load. 

Our series circuit findings prove that KVL holds true because the sum of the voltages in the circuits is equal to zero. In our findings with the parallel circuit without R5, we saw that the KCL holds true because the sum of the currents at a junction is equal to zero. We can also see that the Thevenin Theorem is true and can help aid in reducing the components in circuits in order to simplify the circuits that are presented. 

DESIGN/METHODS 

Part One: Resistors in Series 

For this lab we needed a Fluke Digital Multimeter True RMS (DMM), a DC power supply, a soldering station and piece of solder, and resistors with resistances 1, 2.2, 5.1, 4.7, 6.8, 15, 220 k&Omega;.

We first created a simple circuit with three resistors in series with a DC Power Supply (DCPS). Below is a schematic of this circuit along with a picture of the completed solder circuit board.  



In our solder circuit board, the black wire was accidentally soldered to positive, so red was soldered to negative to fix our mistake. 

We verified the resistor values in the circuit before connecting the circuit to the DCPS using the DMM. The table below shows the measured resistor values compared to their expected values: 

R1 Measured = 0.989k&Omega;, Expected = 1k&Omega;

R2 Measured = 2.16k&Omega;, Expected = 2.2k&Omega;

R3 Measured = 5.01k&Omega;, Expected = 5.1k&Omega; 

Req Measured= 8.17k&Omega;, Expected = 8.3k&Omega;

We then connected the series circuit to the 10V from the DCPS and measured voltage across the resistors and the current flowing through the circuit to see if our findings align with Kirchoff’s Voltage Law. Because the circuit is in series, the current was consistent throughout the entire circuit.  

Part Two: Resistors in Parallel 

We then created a more complex circuit with resistors in parallel to test Kirchoff’s Current Law and Thevenin’s Theorem in which R5 is the load.  

<p align="center">
  <img src="https://github.com/hrma240/Lab-2/blob/main/Adobe%20Scan%20Jan%2025%2C%202024%20(1).jpg">
</p>

We are missing a real-life picture of this circuit, but this circuit with the load removed is documented later in our report. We built this circuit on a regular breadboard and connected it to the DCPS supplying 12V. We verified that the DCPS was within 0.1V of the expected 12V to ensure accuracy in our measurements. We used the DMM to do so and found that the measured value was 12.01V, so it was within this range. 

Next, we used the DMM once again to verify the resistor values. Below are the values we measured compared to the expected resistor values. 

R1 Measured = 4.603k&Omega;, Expected = 4.7k&Omega; 

R2 Measured = 6.77k&Omega;, Expected = 6.8k&Omega;

R3 Measured =14.73k&Omega;, Expected = 15k&Omega; 

R4 Measured= 219.6k&Omega;, Expected=220k&Omega;

R5 Measured= RL=2.18k&Omega;, Expected= 2.2k&Omega;

We used the DMM to measure the voltage drop across R5 and the current through R5, before removing R5 from the circuit entirely. These measurements are the voltage drop across the load (VL) and the current through the load (IL). Below is the schematic with R5 removed and pictures of the bread board.  

With R5, or the load, removed from the circuit, we measured currents I1, I2, and I3 as seen in the schematic. We used the DMM to do so by placing it in series with R1, R2, and R4 respectively. Additionally, we measured the voltage drop across each resistor using the DMM. We used the actual resistances we measured before connecting this circuit to DCPS to calculate the currents I1, I2, and I3 and the voltage drop across each resistor using Ohm’s law.  

Finally, using Thevenin’s Theorem, we calculated the Thevenin resistance and voltage, the Norton current, and the voltage and resistance of the load to compare these values to the measured values of VL and IL.  

Results:


Series Circuit Findings:
|  Voltage Drop Resistor|  Voltage (V)|
|:---:|:---:|
|1 |1.21V|
| 2 |2.65V|
| 3 |6.14V|

I = 1.21mA

KVL holds true in this series circuit because Vr1+Vr2+Vr3=Vs. 1.21V+2.65V+6.14V=10V. And the current we measured through the circuit I=1.21mA aligns with Ohms law in which I=V/Req. 1.21mA=10V/8.3kOhms. 

Parallel Circuit Findings:

V5 or VL = 3.6V
I5 or IL = 1.68mA

Remove R5
|  |  Measured|  Calculated|
|:---|:---:|:---:|
|I1   |.51mA |.49mA|
|I2     | .44mA |.445mA|
|I3     | .05mA |.031mA|

|  Voltage|  Measured Magnitude|  Calculated Voltage|
|:---|:---:|:---:|
|V1   |2.28V |2.29V|
|V2     | 3.064V|2.97V|
|V3     | 6.65V |6.48V|
|V4     | 9.71V |9.8V|

Thevenin:
|  |  Calculated|
|:---:|:---:|
|VTH |9.71V|
| RTH |24.53 kOhms|
| IN |.39 mA|
| VL ||
| IL ||

DISCUSSION QUESTIONS 

Discussion Question 1: How much power does each resistor dissipate? Each branch? Total power? Is the power in equal to the power out? 

We can use the equation P=IV with the above measurements to calculate the power dissipated by each resistor. 

|  Resistor|  Power Dissipated (W)|
|:---:|:---:|
|1 |.0011628W|
| 2 |.00134816W|
| 3 |.002926W|
| 4 |.00048W|

The total power of the circuit can be calculated by P= V^2/Req= 144V/24530Ohms, which ends up equaling around 0.00589W. The total power in is equal to the total power out because the total power in is the calculated total power, while the total power out is the sum of the power dissipated by each resistor, which also equals 0.059W. Since the total power in is equal to the total power out, power is conserved in this circuit. 

Discussion Question 2: Does ITH = IL? 

CONCLUSION 

In this lab, we learned that Kirchhoff’s Current Law (KCL) and Kirchhoff’s Voltage Law (KVL) as well as the Thevenin Theorem hold true. We found these true by creating a series circuit and a parallel circuit and taking measurements across the resistors to see these drops and conducting a series of calculations to determine the voltages for the theorem. These measured and calculated test results have allowed us to see KCL and KVL ideas in place as well as see the theorem in place.  

In addition to this, through the action of soldering, we have learned how to solder and what safety measures to take in order to perform this act correctly and safely. Soldering has shown us how to ensure that resistors, capacitors, cables, etc are held in place on a loose breadboard. Doing this correctly helped allow us to take precise and accurate measurements using the multimeter as well as send voltage through the circuit and have current run through it. 
