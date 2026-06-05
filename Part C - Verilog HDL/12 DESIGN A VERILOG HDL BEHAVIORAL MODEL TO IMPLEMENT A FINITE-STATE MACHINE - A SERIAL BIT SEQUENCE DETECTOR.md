**EXPERIMENT 12**

**DESIGN A VERILOG HDL BEHAVIORAL MODEL TO IMPLEMENT A FINITE-STATE MACHINE - A SERIAL BIT SEQUENCE DETECTOR**
 
**OBJECTIVE:**

To design and implement a Finite-State Machine (FSM) in Verilog HDL that detects a specific serial bit sequence, using behavioral modeling, and to verify its functionality through simulation.

**LEARNING OUTCOMES:**

After completing this experiment, students will be able to:

1.	Understand the concept of Finite-State Machines (FSMs) and their classification.

2.	Design a sequence detector using the Mealy or Moore FSM model.

3.	Implement FSMs using behavioral modeling constructs in Verilog HDL.

4.	Simulate and verify the correct detection of a given bit sequence.

5.	Understand state transitions and waveform verification in simulation.

**THEORY:**

A Finite-State Machine (FSM) is a sequential logic circuit that moves between a finite number of states based on input signals and a clock. It is widely used in control systems, digital communication, and sequence recognition applications.

FSMs are classified into two types:

**1.Moore Machine** – Output depends only on the current state.
**2.	Mealy Machine** – Output depends on the current state and the current input.

A serial bit sequence detector identifies a specific sequence of bits (for example, “1011”) from a serial input stream. Each input bit is processed on every clock pulse, and the FSM transitions through 
states representing how much of the target sequence has been matched so far.

In Verilog, FSMs are typically implemented using three processes:

**1.	State Register:** Stores the current state.

**2.	Next-State Logic:** Determines the next state based on the current state and input.

**3.	Output Logic:** Determines the output based on the current state (and input for Mealy type).

**DESIGN**

<img src="https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20C%20-%20Verilog%20HDL/EXP%2012/d1.png" width ="600">
 
<img src="https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20C%20-%20Verilog%20HDL/EXP%2012/d2.png" width ="600">
VERILOG CODE:
      


PROCEDURE:
1.	Open the Verilog design software (e.g., Xilinx Vivado / ModelSim / Quartus II).

2.	Create a new project and add a Verilog module named sequence_detector.

3.	Write the Verilog HDL code for the FSM (either Moore or Mealy) that detects a given bit sequence, e.g., “1011”.

4.	Define the different states and their transitions based on the input sequence.

5.	Include clk, reset, and input bit signals in the design.

6.	Save the code and compile to check for syntax errors.

7.	Create a testbench file to generate clock, reset, and input signals.

8.	Simulate the design and observe the waveform.

9.	Verify that the output signal (y) goes high whenever the target sequence appears in the input stream.

10.	Synthesize the design and verify hardware resource utilization.

MODEL VIVA QUESTIONS WITH ANSWERS:
1.	Q: What is a Finite-State Machine (FSM)?
 A: An FSM is a sequential circuit that transitions between a finite number of states based on inputs and produces outputs depending on its current state.

2.	Q: What are the two main types of FSMs?
 A: The two types are Moore Machine and Mealy Machine.

○	Moore: Output depends only on the current state.

○	Mealy: Output depends on the current state and input.

3.	Q: What is a sequence detector?
 A: A sequence detector is a circuit that identifies a specific sequence of bits (e.g., “1011”) from a serial input stream.

4.	Q: What is the difference between Moore and Mealy sequence detectors?

 A:

○	In a Moore detector, the output is associated with states, so the output changes only on state transitions.

○	In a Mealy detector, the output can change immediately with the input, resulting in faster detection.

5.	Q: Why do we use state diagrams in FSM design?
 A: State diagrams visually represent all possible states, transitions, and outputs, helping in systematic FSM design.

6.	Q: What is the role of the clock in FSM?
 A: The clock synchronizes state transitions, ensuring all changes occur at defined intervals.

7.	Q: How is the reset signal used in FSM?
 A: The reset initializes the FSM to its starting (idle) state before operation begins.

8.	Q: How can overlapping sequences be detected in FSM?
 A: Overlapping sequences are detected by designing the FSM to reuse previous matched bits as part of the next sequence.

9.	Q: What is the advantage of using behavioral modeling for FSMs?
 A: Behavioral modeling simplifies design by allowing the use of high-level constructs like if-else and case statements, making code more readable and maintainable.

10.	Q: Give some practical applications of FSMs.
 A: FSMs are used in traffic light controllers, vending machines, sequence detectors, communication protocols, and control systems.

INFERENCE:
The Finite-State Machine (FSM) for detecting a specific serial bit sequence was successfully designed, simulated, and synthesized using Verilog HDL. The output waveform confirmed that the FSM correctly identified the given sequence and demonstrated proper state transitions


2.	Mealy Machine – Output depends on the current state and the current input.

A serial bit sequence detector identifies a specific sequence of bits (for example, “1011”) from a serial input stream. Each input bit is processed on every clock pulse, and the FSM transitions through 
