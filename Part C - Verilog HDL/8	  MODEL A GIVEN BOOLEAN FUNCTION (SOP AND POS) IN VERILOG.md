**EXPERIMENT 8**

**MODEL A GIVEN BOOLEAN FUNCTION (SOP AND POS) IN VERILOG**

**OBJECTIVE:**

●	To model a given Boolean function (SOP and POS) in Verilog using F (x2, x1, x0) = Σm(0, 1, 4, 5, 7).  
	
		a.	Continuous assignment with logical operators 
		
		b.	Continuous assignment with conditional operators 

		c.	Using gate level primitives

**LEARNING OUTCOMES:**

After completing this experiment, the student will be able to:

●	Model the given Boolean function (SOP and POS) in Verilog using 

		a.	Continuous assignment with logical operators 
		
		b.	Continuous assignment with conditional operators 
		
		c.	Using gate level primitives

**SOFTWARE REQUIRED:**

●	ModelSim               

**THEORY:**

Logic gates are connected to produce a specified output for certain specified combinations of input variables. With no storage involved, the resulting circuits are referred to as combinational logic. Logic minimization employs various techniques to achieve the simplest gate-level implementation of a logic function. Using Boolean laws, it is possible to minimize digital logic circuits. Since minimization with the use of Boolean laws is neither systematic nor suitable for computer implementation, a number of algorithms were proposed in order to overcome the implementation issue. Karnaugh proposed a technique for simplifying Boolean expressions using an elegant visual technique, which is actually a modified truth table intended to allow minimal sum-of products (SOP) and product- of-sums (POS) expressions to be obtained. Any Boolean expression can be represented in the following forms 

**The Sum of Products Form (SOP)**

Each product term consists of the product of literals (variables or their complements). When two or more product terms are summed by Boolean addition, the resulting expression is SOP 

Eg: AB+CD+ABC 

**The Standard SOP Form :** 

A standard SOP expression is one in which all the variables in the domain appear in each product term (either in complemented or non-complemented form) in the expression 

Eg: 𝐴𝐵𝐶 + 𝐴′𝐵𝐶 + 𝐴𝐵𝐶′ 

**The Product of Sums (POS) form :** 

A sum term consists of the Boolean addition of  literals (variable or their complements). When two or more sum terms are multiplied, the resulting expression is a POS. 

Eg: (A+B) (B+C+D)

**The Standard POS forms :** 

A standard POS expression is one in which all the variables in the domain appear in each sum term in the expression  

Eg: (A+B+C) (A’+B’+C) 

**Boolean expressions and Truth tables** 

All standard Boolean expression can be easily converted into truth table format using binary values for each term in the expression. 

**Karnaugh Map**

The K map provides a systematic method for simplifying Boolean expressions and, if properly used, will produce the simplest SOP and POS expression possible, known as minimum expression. A Karnaugh map is similar to a truth table because it presents all of the possible values of input variables and the resulting output for each value. 

**DESIGN** 

<img src="https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20C%20-%20Verilog%20HDL/EXP%208/CKT.png" width ="600">


**VERILOG CODE:**

module sop_pos (  input  wire x2,x1,x0,    output wire F1,F2);

    wire x1n;
	
    assign x1n = ~x1;
	
    assign F1 = x1n | (x2&x0);   
	
    assign F2 = (x2 |x1n) & (x1n | x0);
	
endmodule

**b.	Continuous assignment with conditional operators**

module sop_pos (    input  wire x2,x1,x0,    output wire F1,F2);
	
	assign F1 = (~x1) ? 1'b1 : ((x2 & x0) ? 1'b1 : 1'b0);
	
	assign F2 = ((x2 | ~x1) & (~x1 | x0)) ? 1'b1 : 1'b0;
	
endmodule

**c.	Using gate level primitives**

module sop_pos_gatelevel(input x0, x1, x2, output F1, F2);

  	wire nx1, and1, or1, or2;
  
  	// For F1 = ~x1 + (x2 & x0)
  
  	not (nx1, x1);         // nx1 = ~x1
  
  	and (and1, x2, x0);    // and1 = x2 & x0
  
  	or  (F1, nx1, and1);   // F1 = nx1 | and1
  
  	// For F2 = (x2 + ~x1)(~x1 + x0)
  
  	or  (or1, x2, nx1);    // or1 = x2 | ~x1
  
  	or  (or2, nx1, x0);    // or2 = ~x1 | x0
  
  	and (F2, or1, or2);    // F2 = or1 & or2
  
endmodule

**PROCEDURE:**

1.	Start the Verilog Simulator / IDE

2.	Write Verilog Code for the given Boolean functions for each given operator format

3.	Save and Compile the Design Files

4.	Simulate the Design

5.	Observe Waveforms / Console Outputs

**MODEL QUESTIONS**

1.	Write the minimized SOP and POS expressions for F(x2,x1,x0)=Σm(0,1,4,5,7).

2.	Implement the given function in Verilog using continuous assignment with logical operators.

3.	Write Verilog code using continuous assignment with conditional operators (?:).

4.	Implement the same Boolean function in Verilog using gate-level modeling.


**VIVA QUESTIONS**

1.	What is the difference between SOP and POS forms of Boolean functions?

2.	Why is minimization of Boolean functions important before implementation?

3.	What is the difference between dataflow modeling and gate-level modeling in Verilog?

4.	Explain the use of the ?: conditional operator in Verilog.

5.	What is the difference between &, | (logical operators) and &&, || (logical AND/OR)?

6.	What are the advantages of using continuous assignment (assign) in Verilog?

7.	How does Verilog differentiate between bitwise and logical operators?

8.	Explain the use of gate-level primitives (and, or, not) in Verilog.

9.	What is the difference between simulation and synthesis in Verilog?

10.	Why do we usually verify Boolean expressions using truth tables before hardware implementation?

11.	Draw the logic circuit diagram corresponding to the minimized SOP expression.

12.	Draw the logic circuit diagram corresponding to the minimized POS expression.

13.	Compare SOP and POS forms – which uses fewer gates for this function?

**INFERENCE:**

●	The given Boolean function (SOP and POS) was successfully modeled in Verilog using continuous assignment with logical operators, continuous assignment with conditional operators, and gate-level primitives.

●	The truth tables were verified for each modeling method

