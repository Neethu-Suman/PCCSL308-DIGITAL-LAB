**EXP NO:1**	

**STUDY OF BASIC DIGITAL ICS AND VERIFICATION OF BOOLEAN THEOREMS USING DIGITAL LOGIC GATES**

**OBJECTIVE:**

●	  To familiarize with the commonly used basic digital logic gate ICs such as AND, OR, NOT, NAND, NOR, and XOR gates.

●	  To understand the pin configuration and internal logic of standard digital ICs (7400, 7402, 7404, 7408, 7432, 7486).

●	  To verify fundamental Boolean algebra theorems using hardware implementation with logic gates.

**LEARNING OUTCOMES:**

●	  Identify and understand the functionality of basic digital logic gates 

●	  Interpret the pin configuration and operation of commonly used digital ICs such as 7400, 7402, 7404, 7408, 7432, and 7486

●	  Verify basic Boolean theorems experimentally using digital logic gates and validate their truth through logic circuits.

**COMPONENTS/EQUIPMENTS REQUIRED:**

![COMPONENTSREQUIRED](https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%201/COMPONENTS%20REQUIRED.png)


**THEORY:** 

**AND Gate:** 
The AND gate is a basic digital logic gate that outputs HIGH (1) only when all its inputs are HIGH. If any input is LOW (0), the output is LOW. It performs a logical multiplication.

**OR Gate:** 
The OR gate produces an output of HIGH (1) if at least one input is HIGH. The output is LOW only when all inputs are LOW. It performs logical addition.

**NOT Gate (Inverter):** 
This gate, also known as an inverter, produces an output that is the logical complement of the input. If the input is 1, the output is 0; if the input is 0, the output is 1.

**NAND Gate:** 
The NAND gate is the inverse of the AND gate. It gives a LOW (0) output only when all inputs are HIGH. In all other cases, the output is HIGH. It is a universal gate, meaning it can be used to construct any other gate.

**NOR Gate:** 
The NOR gate is the inverse of the OR gate. It gives a HIGH (1) output only when all inputs are LOW. Like NAND, it is also a universal gate.

**XOR Gate (Exclusive OR):**
The XOR gate outputs HIGH (1) only when the inputs are different (i.e., one is 0 and the other is 1). If both inputs are the same, the output is LOW. It is used in parity checking, arithmetic operations, etc.

**CIRCUIT DIAGRAM, TRUTH TABLE, AND PIN DIAGRAM OF GATES**

**AND GATE**

![add_gate](https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%201/add%20gate.png)

**OR GATE**

![or_gate](https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%201/or%20gate.png)

**NOT GATE**

![not_gate](https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%201/not%20gate.png)

**NAND GATE**

![nand_gate](https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%201/nand%20gate.png)
  
![nor_gate](https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%201/nor%20gate.png) 

![xor_gate](https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%201/xor%20gate.png)
    
**VERIFICATION OF BOOLEAN THEOREMS:** 

![t1](https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%201/theorem1.png)

![t2](https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%201/theorem2.png)

**DESIGN:**

**Resistor Design:**

Let,
ID	= LED forward current in Amps (found in the LED datasheet)

VD	= LED forward voltage drop in Volts (found in the LED datasheet) 

VCC	= supply voltage

R	=(VCC-VD)/ID = (5-1.2)/10 = 380 Ω ≈ 330Ω 

**PROCEDURE:**

A. Study of Basic Digital ICs
  
  1.	Identify the ICs to be used (e.g., 7400, 7402, 7408, 7432, 7486).

2.	Note the pin configuration of each IC from the datasheet.

3.	Insert the IC properly into the breadboard without bending pins.

4.	Provide power supply connections:

    ○	Vcc (+5V) → Pin 14 (for TTL ICs).

    ○	Ground (0V) → Pin 7.

5.	Connect input switches or wires to the input pins of the gate.

6.	Connect LED/logic probe to the output pins to observe the results.

7.	Verify the truth table of each gate by applying all possible inputs and recording the outputs.

B. Verification of Boolean Theorems

  1.	Choose a Boolean theorem to be verified (e.g., De Morgan’s theorem, Idempotent law, Absorption law).

2.	Express the theorem in two forms – Left-Hand Side (LHS) and Right-Hand Side (RHS).

    ○	Example: For De Morgan’s theorem, (AB)’ = A’ + B’.

3.	Construct LHS circuit using basic gates (AND → NOT).

4.	Construct RHS circuit using basic gates (NOT + OR).

5.	Apply all possible input combinations (00, 01, 10, 11 for two variables).

6.	Record outputs of LHS and RHS circuits in a truth table.

7.	Compare outputs of both sides; if they match for all inputs, the theorem is verified.

C. Tabulation & Observation

   ●	Prepare a truth table with input columns (A, B, …) and output columns (LHS, RHS).

●	Enter observed values for each input condition.

●	Ensure LHS = RHS for theorem verification.


**MODEL QUESTIONS:**

1.	Identify the IC numbers and pin configurations for basic logic gates (AND, OR, NOT, NAND, NOR, XOR, XNOR).
2.	Design and verify the Boolean identity A + A’B = A + B using logic gates.
3.	Construct the circuit to verify De Morgan’s First Theorem: (A·B)’ = A’ + B’.
4.	Implement and test the XOR function using only NAND gates.
5.	Draw the truth table and implement the expression (A + B)’ = A’·B’ using NOR gates only.

**VIVA QUESTIONS:**

1.	What is an Integrated Circuit (IC)?
 → An IC is a small electronic device made of semiconductor material that contains many logic gates or electronic components in a compact package.

2.	What is the difference between SSI, MSI, and LSI ICs?
 → SSI (Small Scale Integration): Few gates (1–10).
 → MSI (Medium Scale Integration): 10–100 gates (encoders, decoders).
 → LSI (Large Scale Integration): Hundreds to thousands of gates (microprocessors).

3.	What is the logic family used in basic digital ICs?
 → TTL (Transistor–Transistor Logic) and CMOS are the most common families.

4.	What is the IC number of basic gates?
 → IC 7400 → NAND gate, IC 7402 → NOR gate, IC 7408 → AND gate, IC 7432 → OR gate, IC 7486 → XOR gate.

5.	Why are NAND and NOR called universal gates?
 → Because any Boolean function can be implemented using only NAND or only NOR gates.
6.	State and verify the Idempotent Law.
 → A + A = A, A·A = A. Verified by using OR/AND gates.

7.	What is the Absorption Law?
 → A + AB = A, A(A + B) = A.

8.	What is the De Morgan’s Theorem?
 → (A·B)’ = A’ + B’, and (A + B)’ = A’·B’.

9.	How can you prove theorems using truth tables?
 → By comparing input-output combinations of both sides of the Boolean expression.

10.	What is the duality principle in Boolean algebra?
 → Every Boolean equation remains valid if we interchange + ↔ · and 0 ↔ 1 simultaneously.

11.	What is a truth table?
 → A table that lists all possible input combinations and their corresponding outputs.

12.	How can you implement an OR gate using NAND gates?
 → By using De Morgan’s theorem and connecting NAND gates appropriately.

13.	How can you implement an AND gate using only NOR gates?
 → By applying double negation and Boolean algebra transformations.

14.	What is the importance of verifying Boolean theorems in the lab?
 → To understand simplification of logic circuits, reduce hardware, and optimize design.

15.	How do you check whether a digital IC is working properly?
 → By applying known inputs (0 and 1), observing outputs, and comparing with the truth table.


**INFERENCE:**

The basic digital logic gate ICs (7400, 7402, 7404, 7408, 7432, 7486) were familiarized, and their truth table were verified. The Demorgan’s theorem was realized using basic gates, and the truth table was verified.


