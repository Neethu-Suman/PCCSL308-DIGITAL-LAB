**EXP NO: 3**

**STUDY OF D FLIP FLOP AND JK FLIP FLOPS USING ICS**

**OBJECTIVE:**

•	To familiarize with D and JK flip-flops using ICs 7474 and 7473

**LEARNING OUTCOMES:**

•	Identify and understand the functionality of D and JK flip-flops using ICs 7474 and 7473

**COMPONENTS/EQUIPMENTS REQUIRED:** 



**THEORY:** 

Digital electronic circuit is classified into combinational logic and sequential logic. Combinational logic output depends on the input levels, whereas sequential logic output

Depends on the stored levels and also the input levels.

 
The storage elements (flip-flops) are devices capable of storing one-bit binary information. The binary info stored in the memory elements at any given time defines the state of the Sequential circuit. 
The input and the present state of the memory element determine the output. The next state of the storage elements is also a function of external inputs and the present state.

**DESIGN:**

**Resistor Design:**

Let,

ID	= LED forward current in Amps (found in the LED datasheet)

VD	= LED forward voltage drop in Volts (found in the LED datasheet) VCC	
   = supply voltage

R	=(VCC-VD)/ID = (5-1.2)/10 = 380 Ω ≈ 330Ω 

**PROCEDURE:**

1.	Wire the circuit as per the diagram on the breadboard.
2.	Apply various input combinations and observe the output for each one.
3.	Verify the truth table for each input/ output combination for both D and JK flip-flops

**CIRCUIT DIAGRAM** 

IC7474 D Flip-flop pin diagram and Truth table 

 
X Either LOW or HIGH Logic Level
↑ Positive-going transition of the clock.
Q0 The output logic level of Q before the indicated input conditions were established.

IC7473 J-K Flip-flop pin diagram and truth table
 
**MODEL QUESTIONS**

1.	Realize a 1-bit data storage using a D flip-flop (IC 7474) and verify its truth table.
2.	Design and verify the truth table of a JK flip-flop (IC 7473) in toggle mode.
3.	Demonstrate the operation of D flip-flop as a delay element using IC 7474.
4.	Construct a T flip-flop using JK flip-flop (IC 7473) and verify its toggling behavior.
5.	Realize a 2-bit binary counter using JK flip-flops (IC 7473) and observe the output sequence.

**VIVA QUESTIONS**

1.	What is the main difference between a D flip-flop and a JK flip-flop?
2.	What is the function of the ‘clock’ input in flip-flops like 7474 and 7473?
3.	How does the D flip-flop avoid the indeterminate state found in an SR flip-flop?
4.	Explain the toggle mode of a JK flip-flop. When does toggling occur?
5.	What are the preset and clear inputs in IC 7474 used for? Are they active high or low?
6.	Why are flip-flops considered edge-triggered devices? Which edge is used in IC 7474?
7.	Can a JK flip-flop be used as a T flip-flop? How?
8.	What is the role of master-slave configuration in IC 7473?
9.	What will be the output of a JK flip-flop when both J and K are 1? Explain with the help of clock pulses.
10.	What are the possible applications of D and JK flip-flops in digital circuits?

**INFERENCE:**

The familiarization of D and JK flip-flops using ICs 7474 and 7473 was done, and the truth table was verified.
