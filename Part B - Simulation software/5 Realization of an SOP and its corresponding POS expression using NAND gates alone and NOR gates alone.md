**EXP NO:5**	

**REALIZATION OF A SOP AND ITS CORRESPONDING POS EXPRESSION USING NAND GATES AND NOR GATES**

**OBJECTIVE:**

  ●	To realize a SOP using NAND gates only and its corresponding POS using NOR gates only 
      F (x2, x1, x0) = Σm(0, 1, 4, 5, 7).  using circuit simulation software 

**LEARNING OUTCOMES:**

  ●	Realize a SOP function using NAND gates only and its corresponding POS using NOR gates only
  
**SOFTWARE REQUIRED:**

circuitverse.org

**THEORY:** 

Logic gates are connected to produce a specified output for certain specified combinations of input variables. With no storage involved, the resulting circuits are referred to as combinational logic. Logic minimization employs various techniques to achieve the simplest gate-level implementation of a logic function. Using Boolean laws, it is possible to minimize digital logic circuits. Since minimization with the use of Boolean laws is neither systematic nor suitable for computer implementation, a number of algorithms were proposed in order to overcome the implementation issue. Karnaugh proposed a technique for simplifying Boolean expressions using an elegant visual technique, which is actually a modified truth table intended to allow minimal sum-of products (SOP) and product- of-sums (POS) expressions to be obtained. Any Boolean expression can be represented in the following forms 

**The Sum of Products Form (SOP)**

Each product term consists of the product of literals (variables or their complements). When two or more product terms are summed by Boolean addition, the resulting expression is SOP 

Eg: AB+CD+ABC 

**The Standard SOP Form**

A standard SOP expression is one in which all the variables in the domain appear in each product term (either in complemented or non-complemented form) in the expression 

Eg: 𝐴𝐵𝐶 + 𝐴′𝐵𝐶 + 𝐴𝐵𝐶′ 

**The Product of Sums (POS) form**

A sum term consists of the Boolean addition of literals (variable or their complements). When two or more sum terms are multiplied, the resulting expression is a POS. 

Eg: (A+B) (B+C+D)

**The Standard POS forms**

A standard POS expression is one in which all the variables in the domain appear in each sum term in the expression 

Eg: (A+B+C) (A’+B’+C) 

**Boolean expressions and Truth tables** 

All standard Boolean expression can be easily converted into truth table format using binary values for each term in the expression. 

**Karnaugh Map** 

The K map provides a systematic method for simplifying Boolean expressions and, if properly used, will produce the simplest SOP and POS expression possible, known as minimum expression. A Karnaugh map is similar to a truth table because it presents all of the possible values of input variables and the resulting output for each value. The K-Map for 2,3 and 4 variables is shown in the following figure

![KM](https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%202/kmap.png)

**PROCEDURE:**
1.	Add the input, output, and gates from the circuit elements according to the circuit diagram.
2.	Connect the circuit as per the logic diagram.
3.	Add a flag to each input and output.
4.	Verify the truth table and analyse the waveform for each input/ output combination for both NAND-only and NOR gate-only circuits of SOP format and POS format of the given function

**CIRCUIT DIAGRAM**

![CD](https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20B%20-%20Simulation%20software/EXP%205/ck1.png)

![CD1](https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20B%20-%20Simulation%20software/EXP%205/CK2.png)

![CD2](https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20B%20-%20Simulation%20software/EXP%205/CK3.png)

**EXPECTED OUTPUT:**
 
**MODEL QUESTIONS:**

1.	Convert the given function F(x2, x1, x0) = Σm(0, 1, 4, 5, 7) into SOP and POS canonical forms and simulate it
2.	Realize the SOP expression: F(A,B,C)=AB’+A’CF using only NAND gates.
3.	Convert and implement the POS expression: F(A,B,C)=(A+B)(B’+C) using only NOR gates.
4.	Simplify the Boolean expression using Boolean algebra: F=AB+AB’+A’B and realize it using NAND gates only.
5.	Design a circuit for the function: F=(A+B’)(A’+C) using NOR gates only. Also, draw the logic diagram.

**VIVA QUESTIONS:**

1.	What is a minterm and a maxterm? How are they used in SOP and POS expressions?
2.	Why do we implement logic circuits using only NAND or only NOR gates?
3.	What does a universal gate mean?
4.	How is De Morgan's Theorem used in designing NAND or NOR-only logic?
5.	What are the steps to design a Boolean function using NAND gates only?
6.	Can every Boolean function be implemented using only NAND or only NOR gates? Explain.
7.	How do you verify that the output of your simulated circuit matches the truth table?
8.	What is the main difference between SOP and POS implementations in hardware?
9.	Which gate configuration is more efficient for hardware implementation—NAND or NOR? Why?
10.	What did you observe during the simulation? Did the SOP-NAND and POS-NOR circuits produce the same output?

**INFERENCE:**
The SOP function F (x2, x1, x0) = Σm(0, 1, 4, 5, 7) was designed and implemented using NAND logic and its corresponding POS expression using NOR gates. The two circuits were simulated using the circuit simulation software



