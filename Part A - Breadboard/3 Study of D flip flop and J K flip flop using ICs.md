**EXP NO: 3**

**STUDY OF D FLIP FLOP AND JK FLIP FLOPS USING ICS**

**OBJECTIVE:**

•	To familiarize with D and JK flip-flops using ICs 7474 and 7473

**LEARNING OUTCOMES:**

•	Identify and understand the functionality of D and JK flip-flops using ICs 7474 and 7473

**COMPONENTS/EQUIPMENTS REQUIRED:** 

![CER](https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%203/31.png)

**THEORY:** 

Digital electronic circuit is classified into combinational logic and sequential logic. Combinational logic output depends on the input levels, whereas sequential logic output

Depends on the stored levels and also the input levels.

 
The storage elements (flip-flops) are devices capable of storing one-bit binary information. The binary info stored in the memory elements at any given time defines the state of the Sequential circuit. 
The input and the present state of the memory element determine the output. The next state of the storage elements is also a function of external inputs and the present state.

![bd](https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%203/32.png)
**DESIGN:**

**Resistor Design:**

Let,

ID	= LED forward current in Amps (found in the LED datasheet)

VD	= LED forward voltage drop in Volts (found in the LED datasheet) VCC	
   = supply voltage

R	=(VCC-VD)/ID = (5-1.2)/10 = 380 Ω ≈ 330Ω 

**PROCEDURE:**

A. D Flip-Flop (using IC 7474)
 
 1.	Connect the IC 7474 on the breadboard and identify its pin configuration from the datasheet.
 2.	Connect Vcc (+5V) and Ground (0V) to the respective pins of the IC.
 3.	Connect the preset (PRE) and clear (CLR) inputs to logic HIGH (disable) unless required for testing.
 4.	Apply the clock signal from a function generator to the clock pin (CLK).
 5.	Connect the D input through logic switches (for 0/1 input selection).
 6.	Connect the Q and Q̅ outputs to LEDs or logic probes for observation.
 7.	Change the D input (0 or 1) and observe the output Q at the rising edge of the clock pulse.
 8.	Verify the operation with the truth table of the D flip-flop.

B. JK Flip-Flop (using IC 7476 / IC 7473)
 
 1.	Place the IC 7476 (dual JK flip-flop with preset and clear) on the breadboard.
 2.	Connect Vcc (+5V) and Ground (0V) to the IC.
 3.	Connect preset (PRE) and clear (CLR) to logic HIGH (inactive) unless testing their functions.
 4.	Apply a clock signal to the clock input pin.
 5.	Provide J and K inputs through logic switches.
 6.	Connect the Q and Q̅ outputs to LEDs or logic probes for observation.
 7.	Apply different combinations of J and K inputs (00, 01, 10, 11) and observe the output at the rising edge of the clock.
 8.	Verify the output with the truth table of the JK flip-flop.
    
     ○	J=0, K=0 → No change
   	
     ○	J=0, K=1 → Reset
   	
     ○	J=1, K=0 → Set
   	
     ○	J=1, K=1 → Toggle

C. Verification
   
   ●	Record input/output observations in the lab observation table.
   
   ●	Compare results with the theoretical truth tables of D and JK flip-flops.
   
   ●	Conclude the practical verification of flip-flop operation.

**CIRCUIT DIAGRAM** 

IC7474 D Flip-flop pin diagram and Truth table 
![IC74](https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%203/33.png)
 
IC7473 J-K Flip-flop pin diagram and truth table
![IC73](https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%203/34.png)
 
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
