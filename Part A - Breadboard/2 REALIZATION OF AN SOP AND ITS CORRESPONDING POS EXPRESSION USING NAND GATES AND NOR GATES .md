**EXP NO: 2**				
**REALIZATION OF AN SOP AND ITS CORRESPONDING POS EXPRESSION USING NAND GATES AND NOR GATES** 

**OBJECTIVE:**

•	To design and implement the given SOP function F (x2, x1, x0) = Σm(0, 1, 4, 5, 7) using NAND logic and its corresponding POS expression using NOR gates 

**LEARNING OUTCOMES:**

•	Realize the given SOP or POS expression using universal gates 

**COMPONENTS/EQUIPMENTS REQUIRED:** 

![comp](https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%202/COMPREQ.png)

              
**THEORY:** 

Logic gates are connected to produce a specified output for certain specified combinations of input variables. With no storage involved, the resulting circuits are referred to as combinational logic. 
Logic minimization employs various techniques to achieve the simplest gate-level implementation of a logic function. Using Boolean laws, it is possible to minimize digital logic circuits. Since minimization 
with the use of Boolean laws is neither systematic nor suitable for computer implementation, a number of algorithms were proposed in order to overcome the implementation issue. Karnaugh proposed a technique 
for simplifying Boolean expressions using an elegant visual technique, which is actually a modified truth table intended to allow minimal sum-of products (SOP) and product- of-sums (POS) expressions to be 
obtained. Any Boolean expression can be represented in the following forms 

The Sum of Products Form (SOP)
Each product term consists of the product of literals (variables or their complements). When two or more product terms are summed by Boolean addition, the resulting expression is SOP 
Eg: AB+CD+ABC 
The Standard SOP Form 
A standard SOP expression is one in which all the variables in the domain appear in each product term (either in complemented or non-complemented form) in the expression 
Eg: 𝐴𝐵𝐶 + 𝐴′𝐵𝐶 + 𝐴𝐵𝐶′ 

The Product of Sums (POS) form 
A sum term consists of the Boolean addition of literals (variable or their complements). When two or more sum terms are multiplied, the resulting expression is a POS. 
Eg: (A+B) (B+C+D)

The Standard POS forms 
A standard POS expression is one in which all the variables in the domain appear in each sum term in the expression 
Eg: (A+B+C) (A’+B’+C) 

Boolean expressions and Truth tables 
All standard Boolean expression can be easily converted into truth table format using binary values for each term in the expression. 

Karnaugh Map 
The K map provides a systematic method for simplifying Boolean expressions and, if properly used, will produce the simplest SOP and POS expression possible, known as minimum expression. A Karnaugh map is 
similar to a truth table because it presents all of the possible values of input variables and the resulting output for each value. The K-Map for 2,3 and 4 variables is shown in the following figure

![kmap](https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%202/kmap.png)

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
3.	Verify the truth table for each input/ output combination for both SOP and POS circuits.

**CIRCUIT DIAGRAM** 

![ck1](https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20A%20-%20Breadboard/EXP%20NO%202/ck1.png)
  
SOP F1 = x1’ + x2x0
POS F2 = (x2 + x1’) (x1’ + x0)

NAND LOGIC FOR SOP - EQUATION AND CIRCUIT DIAGRAM

F1 = x1 + x2x0   = x1.(x2x0)

NOR LOGIC FOR POS  F2 = (x2 + x1) (x1 + x0) = (x2 + x1) + (x1 + x0) 
 
**MODEL QUESTIONS:**

1.	Realize the SOP expression: F(A,B,C)=AB’+A’CF using only NAND gates.
2.	Convert and implement the POS expression: F(A,B,C)=(A+B)(B’+C) using only NOR gates.
3.	Simplify the Boolean expression using Boolean algebra: F=AB+AB’+A’B and realize it using NAND gates only.
4.	Design a circuit for the function: F=(A+B’)(A’+C) using NOR gates only. Also, draw the logic diagram.

**VIVA QUESTIONS:**

1.	What is the difference between SOP and POS forms?
2.	Define NAND and NOR gates. Why are they called universal gates?
3.	How can you implement an AND, OR, and NOT gate using only NAND gates?
4.	Why do we prefer NAND or NOR gates in digital circuit design?
5.	How do you convert a Boolean function into its SOP and POS form?
6.	What is the advantage of using universal gates for implementing logic expressions?
7.	Explain De Morgan's Theorems and their application in gate-level realization.
8.	How does gate delay affect the performance of a logic circuit?
9.	What will be the output if you connect the inputs of a NAND gate together?
10.	In practical design, why is minimizing the number of gates used in a circuit important?

**INFERENCE:**

The SOP function F (x2, x1, x0) = Σm(0, 1, 4, 5, 7) was designed and implemented using NAND logic and its corresponding POS expression using NOR gates 

