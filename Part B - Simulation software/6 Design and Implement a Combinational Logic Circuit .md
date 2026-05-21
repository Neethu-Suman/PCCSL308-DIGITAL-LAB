**EXP NO:6**

**DESIGN AND IMPLEMENT A COMBINATIONAL LOGIC CIRCUIT**

**OBJECTIVE:**

●	To design and simulate the following combinational logic circuit for arbitrary functions 

1.	Binary to Gray code converters.
2.	Half adder
3.	Full adder
4.	Half subtractor
5.	Full subtractor
   
**LEARNING OUTCOMES:**

●	Design and simulate the combinational logic circuit using circuit simulation software

**SOFTWARE REQUIRED:** 

circuitverse.org

**THEORY:** 

**Binary to Gray code converter**

By putting the MSB of 1 below the axis and the MSB of 1 above the axis and reflecting the (n-1) bit code about an axis after 2n-1 rows, we can obtain the n-bit gray code. Let b0, b1, b2, and b3 be the bits representing the binary numbers, where b0 is the LSB and b3 is the MSB, and let g0, g1, g2, and g3 be the bits representing the gray code of the binary numbers, where g0 is the LSB and g3 is the MSB.
To find the corresponding digital circuit, the K-Map technique is used, where each of the gray code bits serves as output and all the binary bits serve as input. 
Using the K-map method to design the logical circuit for the conversion of binary to gray code:
            
               
g3= b3	g2= b2b3’+b3b2’=b2⊕b3	g1=b2b1’+b1b2’=b1⊕b2        g0=b0b1’+b1b0’=b0⊕b1

**Half Adder:**

Half adders perform a simple binary addition of 2 bits, producing 2 outputs, the sum bit (S) and carry bit (C). The half adder is shown in the block diagram in the following figure
 

**Full Adder:**

A Full Adder is an adder that adds three inputs and produces two outputs. The first two inputs are A and B, and the third input is an input carry as C-IN. The output carry is designated as C-OUT, and the 
normal output is designated as S (SUM). The full adder is shown in the block diagram in the following figure
 
**Half Subtractor:**

Half subtractors perform a simple binary subtraction of 2 bits, producing 2 outputs, the difference and borrow. The half subtractor is shown in the block diagram in the following figure
 
Full Subtractor:

Full Subtractor is a subtractor that subtracts three inputs and produces two outputs. The first two inputs are A and B, and the third input is an input borrow as B-IN. The output borrow is designated as B-OUT and the normal output is designated as D which is Difference. The full subtractor is shown in the block diagram in following figure.
 
**PROCEDURE:**

1.	Add the input, output, and gates from the circuit elements according to the circuit diagram.
2.	Connect the circuit as per the logic diagram.
3.	Add a flag to each input and output.
4.	Verify the truth table and analyse the waveform for each input/ output combination for all the given five combinational circuits
   
**CIRCUIT DIAGRAM:**

**Binary to Gray code converter**
 
**Half Adder:**
**Truth Table:**
 
Using AOI Logic:  S = A’B + AB’ C =AB
 

**Full Adder:**
**Truth Table:**

 
**Using AOI Logic**

 

 

Half Subtractor:
Truth Table:
 
Using AOI Logic  	d=A’B+AB’ 	b=A’B    
   
Full Subtractor:
Truth Table:
 
Using AOI Logic
   
 
EXPECTED OUTPUT:

Binary to Gray code converter

 


Half Adder:
 

Full Adder:
 

Half Subtractor:

 


Full Subtractor:
 

MODEL QUESTIONS:

1.	Design and simulate a 3-bit Binary to Gray code converter using logic gates.
2.	Design and simulate a 4-bit Gray to Binary code converter using logic gates.
3.	Design and simulate a Full Adder using two Half Adders and an OR gate.
4.	Design and simulate a Full Adder using NAND gates only.
5.	Design and simulate a Full Subtractor using NAND gates only.
6.	Design and simulate a half adder and half subtractor using NAND gates only.

VIVA QUESTIONS:

1.	What is the key difference between Binary code and Gray code? Why is Gray code used?
2.	What are the outputs of a Half Adder? Can it handle carry from previous stages? Why/why not?
3.	How does a Full Adder differ from a Half Adder?
4.	Explain how a Full Adder can be implemented using two Half Adders.
5.	What are the outputs of a Half Subtractor? Define the borrow.
6.	How do you implement a Full Subtractor using basic logic gates?
7.	What logic gates are used in designing a Binary to Gray code converter?
8.	Can you use XOR gates to implement a Binary to Gray code converter? Justify.
9.	Why are combinational circuits different from sequential circuits? Give one key difference.
10.	What real-world applications use Gray code and full adders/subtractors?

INFERENCE:

The Binary to Gray code converter, Half Adder, Full Adder, Half Subtractor, and Full Subtractor circuits were designed using basic logic gates and simulated using circuit simulation software


