**EXP NO:4**	

**FAMILIARIZATION WITH THE WORKING OF CIRCUIT SIMULATION SOFTWARE**

**OBJECTIVE:**

●	To familiarize with the working of circuit simulation software (circuitverse.org)

●	To realize basic logic gates (AND, OR, NOT, NAND, NOR, XNOR, and XOR gates) and analyze their waveforms

●	To design and simulate logic circuits using circuit simulation software to verify the fundamental theorems of Boolean algebra using basic logic gates.

**LEARNING OUTCOMES:**

1.	Understand the purpose and basic functionality of circuit simulation software

2.	Construct and simulate basic digital logic gates (AND, OR, NOT, NAND, NOR, XOR, XNOR) using the simulation software.

3.	Observe and analyze the input-output waveforms of basic logic gates.

4.	Validate the truth tables of logic gates through simulation.

5.	Develop familiarity with digital circuit design using simulation tools, which is essential before hardware implementation.

**SOFTWARE REQUIRED:**

circuitverse.org

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

Circuit simulation software provides a virtual platform for designing, building, and testing electronic circuits without physically assembling them. It is a vital tool for engineers, students, and hobbyists 
to understand circuit behavior before implementing it in real hardware.

Key Features:

●	Drag-and-drop component-based design

●	Real-time simulation of circuits

●	Visualization tools (waveforms, timing diagrams, truth tables)

●	Debugging support for logic errors

●	No physical components required, minimizing cost and risk

Benefits:

●	Safe environment for trial and error

●	Faster learning and prototyping

●	Reduces hardware costs

●	Enhances understanding of theoretical concepts through practical application

Popular circuit simulators include:

●	Multisim – Industry-standard simulator with analog/digital support

●	Proteus – Widely used for microcontroller simulation

●	LTspice – Focused on analog simulations

●	Logisim – Educational tool for digital circuits

●	CircuitVerse – Online, open-source digital logic simulator

CircuitVerse – An Open Source Digital Logic Simulator

CircuitVerse is a free, online platform designed for learning and teaching digital logic circuits. It is widely used in academic environments due to its simplicity, accessibility, and educational tools.

Key Features:

●	Browser-based: No installation needed

●	Real-time simulation of logic circuits

●	Components include:

  ○	Basic gates (AND, OR, NOT, etc.)

  ○	Flip-flops, multiplexers, decoders

  ○	Clocks, input/output devices, LEDs

●	Sub-circuit support for modular design

●	Timing diagram viewer for waveform analysis

●	Truth table generator

●	Collaboration and project sharing features

Educational Advantages:

●	Ideal for students new to digital electronics

●	Interactive learning: simulate and immediately see results

●	Encourages experimentation and creative circuit design

●	Useful for assignments, lab experiments, and project prototyping

Common Applications in CircuitVerse:

●	Designing and testing combinational circuits (adders, encoders, decoders)

●	Sequential circuits (flip-flops, counters, registers)

●	Verifying logic gate truth tables

●	Analyzing timing behavior using waveforms

**CIRCUIT DIAGRAM, TRUTH TABLE, AND PIN DIAGRAM OF GATES**

**AND GATE**

<img src ="https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%201/add%20gate.png" width = "400">

**OR GATE**

<img src ="https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%201/or%20gate.png" width = "400">

**NOT GATE**

<img src ="https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%201/not%20gate.png" width = "400">

**NAND GATE**

<img src ="https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%201/nand%20gate.png" width = "400">
  
<img src ="https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%201/nor%20gate.png" width = "400"> 

<img src ="https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%201/xor%20gate.png" width = "400">
    
**VERIFICATION OF BOOLEAN THEOREMS:** 

<img src ="https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%201/theorem1.png" width = "400">

<img src ="https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%201/theorem2.png" width = "400">

**PROCEDURE:**

1.	Add the input, output, and gates from the circuit elements according to the circuit diagram.
2.	Connect the circuit as per the logic diagram.
3.	Add flag to each input and output.
4.	Verify the truth table and analyse the waveform for each input/ output combination for the gates and the Boolean theorem

**EXPECTED OUTPUT:**

**CIRCUIT DIAGRAM**

**AND GATE**

<img src ="https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20B%20-%20Simulation%20software/EXP%204/1%20AND%20gate.png" width = "400">

**OR GATE**

<img src ="https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20B%20-%20Simulation%20software/EXP%204/2%20OR%20GATE.png" width = "400">

**NOT GATE**

<img src ="https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20B%20-%20Simulation%20software/EXP%204/3%20NOT%20GATE.png" width = "400">

**XOR GATE**

<img src ="https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20B%20-%20Simulation%20software/EXP%204/4%20XOR%20GATE.png" width = "400">

**NAND GATE**

<img src ="https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20B%20-%20Simulation%20software/EXP%204/5%20NAND%20gate.png" width = "400">

**NOR GATE**

<img src ="https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20B%20-%20Simulation%20software/EXP%204/6%20NOR%20GATE.png" width = "400">

**NXOR GATE**

<img src ="https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20B%20-%20Simulation%20software/EXP%204/7%20NXOR%20GATE.png" width = "400">

Realize a given Boolean function using basic gates and verify the waveform with the truth table.

To design and implement the given SOP function F (x2, x1, x0) = Σm(0, 1, 4, 5, 7). Using basic gate

<img src ="https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20B%20-%20Simulation%20software/EXP%204/tt.png" width = "400">

**K map simplification**

<img src ="https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20B%20-%20Simulation%20software/EXP%204/kmap.png" width = "400">


**MODEL QUESTIONS:**
1.	Design and simulate a logic circuit for the expression:
F=A⋅(B+C′) using CircuitVerse and observe the output waveform.
2.	Verify De Morgan’s Theorem using logic gates: using CircuitVerse simulation. Capture the waveform and explain the result.
3.	Construct the truth table and waveform for the XOR gate using basic logic gates in CircuitVerse.
4.	Simulate and analyze the waveform of the circuit: F (A+B)′⋅C using CircuitVerse.
5.	Design a circuit to demonstrate the associative law of Boolean algebra:
A+(B+C)=(A+B)+C using logic gates and verify it using simulation.

**VIVA QUESTIONS:**
1.	What is CircuitVerse, and what are its primary uses?
2.	Explain the working of the XOR gate using basic gates.
3.	What are the fundamental theorems of Boolean algebra? Name any two.
4.	What is the significance of waveform analysis in logic circuit simulation?
5.	How can De Morgan’s Theorems be verified using logic gates in a circuit simulator?
6.	What is the difference between combinational and sequential circuits?
7.	Name any five basic digital ICs and their functions.
8.	What is the significance of verifying Boolean theorems using logic gates?
9.	State and verify the Boolean identity A + A = A using logic gates.
10.	How can you implement an XOR gate using only NAND gates?

**INFERENCE:**
The circuit simulation software (Circuitverse.org) was familiarized. The basic digital logic gates (AND, OR, NOT, NAND, NOR, XNOR, and XOR gates) were simulated using circuit simulation software, their truth table were verified, and their waveforms were analyzed. The Demorgan’s theorem was successfully verified by designing and simulating logic circuits using basic gates in circuit simulation software


