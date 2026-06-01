**EXPERIMENT 9**

**MODEL MUX, DEMUX, ENCODER, DECODER AND A 7-SEGMENT DISPLAY DECODER IN VERILOG**

**OBJECTIVE:**

●	To model a 4:1 MUX, 1:4 DEMUX, 4 to 2 encoder, and 2 to 4 decoder and a 7-Segment Display Decoder in Verilog using 

    a.	continuous assignment with logical operators 

    b.	continuous assignment with conditional operators

**LEARNING OUTCOMES:**

After completing this experiment, the student will be able to:

●	Model a 4:1 MUX, 1:4 DEMUX, 4 to 2 encoder, and 2 to 4 decoder, and a 7-Segment Display Decoder in Verilog using 

       a.	continuous assignment with logical operators 
 
       b.	continuous assignment with conditional operators

**SOFTWARE REQUIRED:** 

●	ModelSim                                

**THEORY:** 

In digital design, combinational circuits form the backbone of data selection, encoding, and display systems. Using Verilog HDL, these circuits can be modeled at the gate level, dataflow level (continuous assignment), or behavioral level. In this experiment, we focus on continuous assignment using two methods:

●	Logical operators (&, |, ~)

●	Conditional operators (?:)

Basic Circuits

 a) 4:1 Multiplexer (MUX)

   ●	A multiplexer selects one input out of many and forwards it to the output based on select lines.

   ●	For a 4:1 MUX, 4 inputs (I0–I3) are controlled by 2 select lines (S1, S0).

   ●	Boolean expression: Y = S̄₁S̄₀I₀ + S̄₁S₀I₁ + S₁S̄₀I₂ + S₁S₀I₃

   ●	In Verilog: Can be modeled with logical operators (&, |, ~) or conditional operator (assign Y = (S==2’b00)? I0 : (S==2’b01)? I1 : ...).

b) 1:4 Demultiplexer (DEMUX)

   ●	A demultiplexer routes one input to one of several outputs based on select lines.

   ●	For 1:4 DEMUX, a single input D is sent to one of 4 outputs (Y0–Y3) using select lines S1, S0.

   ●	Boolean equations: Y₀ = D S̄₁ S̄₀    Y₁ = D S̄₁ S₀   Y₂ = D S₁ S̄₀   Y₃ = D S₁ S₀ 

c) 4-to-2 Encoder
 
   ●	An encoder converts active input lines into a coded binary output.

   ●	A 4-to-2 encoder maps 4 inputs into 2-bit outputs.

   ●	Example: If I2=1, then Output = 10.

   ●	Boolean equations:Y₁ = I₂ + I₃   Y₀ = I₁ + I₃ 

d) 2-to-4 Decoder
 
   ●	A decoder performs the opposite function of an encoder.

   ●	It converts n inputs into 2^n unique outputs.

   ●	For 2 inputs (A, B), 4 outputs are generated:

      Y₀ = ĀB̄       Y₁ = ĀB      Y₂ = AB̄     Y₃ = AB
 
e) 7-Segment Display Decoder

   ●	A 7-segment display uses 7 LEDs (a–g) to display numbers (0–9).
 
   ●	A BCD to 7-segment decoder takes 4-bit input (0–9) and lights up appropriate segments

 ●	Example: To display "0", segments a, b, c, d, e, f = 1, and g = 0.

 ●	Boolean equations can be written for each segment (a–g) and coded in Verilog.

Applications

 ●	MUX/DEMUX: Data routing in communication and computer systems.

 ●	Encoder/Decoder: Priority systems, data compression, memory addressing.7-Segment Decoder: Display units in calculators, digital clocks, embedded systems.

**CIRCUIT DIAGRAM AND VERILOG CODE**

**4:1 MUX**
 
<img src ="https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20C%20-%20Verilog%20HDL/EXP%209/ck1.png">

**1:4 DEMUX**

<img src ="https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20C%20-%20Verilog%20HDL/EXP%209/ckt2.png">

**4:2 ENCODER**
<img src="https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20C%20-%20Verilog%20HDL/EXP%209/ck3.png">

