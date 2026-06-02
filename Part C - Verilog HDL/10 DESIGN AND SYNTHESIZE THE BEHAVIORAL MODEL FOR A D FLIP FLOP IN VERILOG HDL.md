**EXPERIMENT 10**

**DESIGN AND SYNTHESIZE THE BEHAVIORAL MODEL FOR A D FLIP FLOP IN VERILOG HDL**

**OBJECTIVE:**

●	To design and synthesize a behavioral model of a D flip-flop using Verilog HDL.

●	To understand the working of synchronous sequential circuits.

●	To simulate and verify the truth table and timing diagram of a D flip-flop.

**LEARNING OUTCOMES :**

After performing this experiment, the student will be able to:

1.	Understand the working principle of a D flip-flop.

2.	Model sequential circuits in Verilog using behavioral constructs (always block).

3.	Differentiate between blocking (=) and non-blocking (<=) assignments.

4.	Verify the functionality of a flip-flop using simulation tools.

**THEORY:**

A flip-flop is a fundamental building block of sequential logic circuits. Unlike combinational circuits, sequential circuits depend not only on the present inputs but also on the previous state. Flip-flops are edge-triggered devices that store one bit of data and are widely used in registers, counters, and memory elements.

D Flip-Flop (Data/Delay Flip-Flop)

●	The D flip-flop eliminates the ambiguity of the SR flip-flop (where S = R = 1 is invalid).

●	It has only one input, D (Data), apart from the clock (CLK) and optional reset/set signals.

●	On the triggering edge of the clock (usually rising edge), the output Q takes the value of D.

●	Thus, the next state of the flip-flop is always equal to the value of D.

Applications of D Flip-Flop

●	Data storage element in registers and memory.

●	Used in shift registers and counters.

●	Synchronization of asynchronous signals.

●	Fundamental component in digital system design and FPGA-based systems.

**DESIGN**
 
**VERILOG CODE:**

module dfp(output reg Q,Qn,input wire Clock,Reset,Preset,D,EN);

  always @(posedge Clock or negedge Reset or negedge Preset)

  if(!Reset)
    
    begin
       
      Q <= 1'b0;
      
      Qn <= 1'b1;
    
    end

 else if(!Preset)
    
    begin
    
      Q <= 1'b1;
      
      Qn <= 1'b0;
   
    end

else 

 if (EN)
 
   begin
   
       Q <=D;
       
       Qn <=~D;
   
   end

endmodule	

PROCEDURE:
1.	Write the Verilog code in the HDL tool.
2.	Compile and check for syntax errors.
3.	Run the simulation using testbench.
4.	Observe waveforms and verify that Q follows D on the rising edge of the clock.
5.	Perform synthesis and check resource utilization.

Model Viva Questions:
1.	What is the difference between latch and flip-flop?
 → Latch is level-triggered, flip-flop is edge-triggered.

2.	Why is it called a D flip-flop?
 → Because it transfers the value of the Data input (D) to output Q on clock edge.

3.	What is the excitation table of a D flip-flop?
 → Q(next) = D, irrespective of present state.

4.	Why are non-blocking assignments (<=) used in sequential circuits?
 → To avoid race conditions and ensure correct synchronous updates.

5.	What is setup time and hold time in flip-flops?
 → Setup time: Minimum time input D must be stable before clock edge.
 → Hold time: Minimum time input D must remain stable after clock edge.

6.	Difference between synchronous and asynchronous reset?
 → Synchronous reset acts only on clock edge; asynchronous reset overrides clock.

INFERENCE:
●	The behavioral model of a D flip-flop was successfully designed, simulated, and synthesized using Verilog HDL.

●	From the simulation waveforms, it is verified that the output Q follows input D only at the rising edge of the clock.

●	This experiment demonstrates the modeling of sequential circuits and the importance of clocking in digital systems.

