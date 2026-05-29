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

![sop](https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20B%20-%20Simulation%20software/EXP%205/sop.png)

![pos](https://github.com/Neethu-Suman/PCCSL308-DIGITAL-LAB/blob/main/Part%20B%20-%20Simulation%20software/EXP%205/pos.png)
 
**MODEL QUESTIONS:**

1.	Convert the given function F(x2, x1, x0) = Σm(0, 1, 4, 5, 7) into SOP and POS canonical forms and simulate it
2.	Realize the SOP expression: F(A,B,C)=AB’+A’CF using only NAND gates.
3.	Convert and implement the POS expression: F(A,B,C)=(A+B)(B’+C) using only NOR gates.
4.	Simplify the Boolean expression using Boolean algebra: F=AB+AB’+A’B and realize it using NAND gates only.
5.	Design a circuit for the function: F=(A+B’)(A’+C) using NOR gates only. Also, draw the logic diagram.

**VIVA QUESTIONS:**

1.	What is the given Boolean function to implement?

    F(x2,x1,x0)=Σm(0,1,4,5,7)F(x_2, x_1, x_0) = \Sigma m(0, 1, 4, 5, 7)F(x2,x1,x0)=Σm(0,1,4,5,7)

2.	What does Σm(0, 1, 4, 5, 7) represent?

    It represents the minterms where the function output is 1 — these are the combinations for which the output of F is HIGH (1).
  	
3.	What is an SOP expression?

    SOP (Sum of Products) is a form where logical AND terms (products) are ORed together to form the Boolean function.
  	
4.	What is a POS expression?

    POS (Product of Sums) is a form where logical OR terms (sums) are ANDed together to form the Boolean function.
  	
5.	How do you find the POS form from the given minterms?

    Find the maxterms (where output is 0). For F = Σm(0, 1, 4, 5, 7), the maxterms are at indices not included: 2, 3, 6 → F = ΠM(2, 3, 6)
  	
6.	What is a universal gate?

    A universal gate is a gate that can be used to implement any Boolean function. NAND and NOR gates are universal.
  	
7.  What tool can be used to simulate the given circuit?

    Tools like CircuitVerse, Logisim, Multisim, or Proteus can be used for digital simulation.

8.	How do you verify the logic circuit is working correctly?

    By comparing the output waveform or simulation result with the expected truth table of the function.

9.	What is a waveform in digital logic simulation?

    A graphical representation of the logic levels (0 or 1) of signals over time.

10.	How many input combinations are possible for a 3-variable Boolean function?

    23=82^3 = 823=8 combinations.

11.	What is the importance of truth tables in circuit design?

    Truth tables help verify whether the circuit output matches the expected logic function for all possible input combinations.


**INFERENCE:**
The SOP function F (x2, x1, x0) = Σm(0, 1, 4, 5, 7) was designed and implemented using NAND logic and its corresponding POS expression using NOR gates. The two circuits were simulated using the circuit simulation software



