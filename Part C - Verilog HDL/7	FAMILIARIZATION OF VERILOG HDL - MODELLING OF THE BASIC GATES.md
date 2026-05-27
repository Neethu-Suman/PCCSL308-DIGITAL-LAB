**EXP NO:7**	

**FAMILIARIZATION OF VERILOG HDL - MODELLING OF THE BASIC GATES**

**OBJECTIVE:**

To familiarize Verilog HDL - Modelling of the basic gates using 
1.	Gate level modelling
2.	Behavioral modelling 
3.	Structural modelling 
4.	Dataflow modelling  

**LEARNING OUTCOMES:**

After completing this experiment, the student will be able to:
•	Implement basic gates using the following four Verilog modeling methods 
1.	Gate level modelling
2.	Behavioral modelling 
3.	Structural modelling 
4.	Dataflow modelling  

**SOFTWARE REQUIRED:** 

ModelSim

**THEORY:**

**AND Gate:** 
The AND gate is a basic digital logic gate that outputs HIGH (1) only when all its inputs are HIGH. If any input is LOW (0), the output is LOW. It performs a logical multiplication.

**OR Gate:** 
The OR gate produces an output of HIGH (1) if at least one input is HIGH. The output is LOW only when all inputs are LOW. It performs logical addition.

**NOT Gate (Inverter):** 
This gate, also known as an inverter, produces an output that is the logical complement of the input. If the input is 1, the output is 0; if the input is 0, the output is 1.

**CIRCUIT DIAGRAM:**

**AND GATE**

<img src ="https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%201/add%20gate.png">
 
**OR GATE**

<img src ="https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%201/or%20gate.png">
 
**NOT GATE**

<img src ="https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%201/not%20gate.png">

**VERILOG CODE:**

**1. Gate-Level Modeling**

module gates_gatelevel (    input  wire A, B,    output wire Y_and, Y_or, Y_not);
    and g1(Y_and, A, B);   // AND gate
    or  g2(Y_or,  A, B);   // OR gate
    not g3(Y_not, A);      // NOT gate (only one input)
endmodule

**2. Behavioral Modeling**

module gates_behavioral ( input  wire A, B,     output reg  Y_and, Y_or, Y_not);
    always @ (A or B) begin
        Y_and = A & B;   // AND operation
        Y_or  = A | B;   // OR operation
        Y_not = ~A;      // NOT operation
    end
endmodule

**3. Structural Modeling**

// Submodules
module and_gate(output Y, input A, B);
    assign Y = A & B;
endmodule

module or_gate(output Y, input A, B);
    assign Y = A | B;
endmodule

module not_gate(output Y, input A);
    assign Y = ~A;
endmodule

// Structural Top Module
module gates_structural ( input  wire A, B,   output wire Y_and, Y_or, Y_not
);
    and_gate u1(Y_and, A, B);
    or_gate  u2(Y_or,  A, B);
    not_gate u3(Y_not, A);
endmodule

**4. Dataflow Modeling**

module gates_dataflow (
    input  wire A, B,
    output wire Y_and, Y_or, Y_not
);
    assign Y_and = A & B;   // AND gate
    assign Y_or  = A | B;   // OR gate
    assign Y_not = ~A;      // NOT gate
endmodule

**PROCEDURE:**

1.	Start the Verilog Simulator / IDE
2.	Write Verilog Code for Basic Gates for each modeling
3.	Save and Compile the Design Files
4.	Simulate the Design
5.	Observe Waveforms / Console Outputs

OUTPUT:

1.	Gate level modelling









2.	Behavioral modelling 









3.	Structural modelling 










4.	Dataflow modelling  










MODEL QUESTIONS:

1.	Write a Verilog program for AND, OR, and NOT gates using Gate-level modeling.
2.	Write a Verilog program for AND, OR, and NOT gates using Behavioral modeling.
3.	Write a Verilog program for AND, OR, and NOT gates using Structural modeling.
4.	Write a Verilog program for AND, OR, and NOT gates using Dataflow modeling.
5.	Write a Verilog program for a 2-input XOR gate using all four modeling styles.
6.	Write a testbench in Verilog to verify the outputs of AND, OR, and NOT gates.

VIVA QUESTIONS:

1.	What is Verilog HDL and why is it used?
2.	What is the difference between Behavioral, Dataflow, Gate-level, and Structural modeling?
3.	Which modeling style is closest to actual hardware gates?
4.	Which modeling style is most commonly used in large digital system design? Why?
5.	Can we mix different modeling styles in the same Verilog project?
6.	What is the difference between assign (used in Dataflow) and always (used in Behavioral)?
7.	What is the purpose of structural modeling in Verilog?
8.	Why do we need testbenches in Verilog simulations?
9.	How does Verilog differ from VHDL?
10.	Compare Gate-level modeling and Structural modeling in Verilog.
11.	What happens if we don’t declare reg type in Behavioral modeling?

INFERENCE:
Modeled AND, OR, NOT gates in the following four Verilog modeling methods, and their truth tables were verified.
1.	Gate level modelling
2.	Behavioral modelling 
3.	Structural modelling 
4.	Dataflow modelling  


