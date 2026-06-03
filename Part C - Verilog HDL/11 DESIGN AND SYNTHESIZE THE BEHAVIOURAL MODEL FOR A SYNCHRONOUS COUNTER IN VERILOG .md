EXPERIMENT 11
DESIGN AND SYNTHESIZE THE BEHAVIOURAL MODEL FOR A SYNCHRONOUS COUNTER IN VERILOG 

OBJECTIVE:
To design and synthesize a behavioural model of a synchronous counter using Verilog HDL and verify its functionality through simulation.
LEARNING OUTCOMES:
After completing this experiment, students will be able to:
1.	Understand the concept of synchronous counters and their working principle.

2.	Develop Verilog code using behavioural modelling techniques.

3.	Simulate and verify the functionality of a synchronous counter.

4.	Synthesize the design and observe the hardware resource utilization.

THEORY:
A synchronous counter is a type of counter in which all flip-flops are triggered simultaneously by the same clock signal. This eliminates propagation delay problems associated with asynchronous (ripple) counters, leading to faster operation.
Counters are used for counting purposes in digital systems such as timers, frequency dividers, and digital clocks.
A synchronous counter can be up, down, or up/down type depending on the counting sequence. In a behavioural model, the counter is described using high-level constructs such as always blocks and conditional statements instead of gate-level connections.




DESIGN
 
VERILOG CODE:
2bit up counter
module counter_2bit_up(output reg[1:0] 
CNT, input wire Clock, Reset);
reg[1:0] current_state, next_state;
parameter C0 = 2'b00, C1 = 2'b01, 
C2 = 2'b10, C3 = 2'b11;
always @(posedge Clock or negedge Reset)
    begin: STATE_MEMORY
	if(!Reset)
	    current_state <= C0;
        else
	    current_state <= next_state;
    end
always @(current_state)
begin: NEXT_STATE_LOGIC
    case (current_state)
    C0:  next_state = C1;
    C1:  next_state = C2; 
    C2:  next_state = C3; 
    C3:  next_state = C0; 
    default : next_state = C0;
    endcase
end
always @(current_state)
 begin: OUTPUT_LOGIC
   case (current_state)
       C0 :CNT = 2'b00;
       C1 :CNT = 2'b01;
       C2 :CNT = 2'b10;
       C3 :CNT = 2'b11;
       default :CNT =2'b00;
   endcase
 end
endmodule

      
2bit down counter
module counter_2bit_down(output reg[1:0] CNT, input wire Clock, Reset);
reg[1:0] current_state, next_state;
parameter C0 = 2'b00, C1 = 2'b01, C2 = 2'b10, C3 = 2'b11;
always @(posedge Clock or negedge Reset)
    begin: STATE_MEMORY
	if(!Reset)
	    current_state <= C0;
        else
	    current_state <= next_state;
    end
always @(current_state)
begin: NEXT_STATE_LOGIC
    case (current_state)
    C0: next_state =C3;
    C1: next_state =C0;
    C2: next_state =C1;
    C3: next_state =C2;
    default : next_state = C0;
    endcase
end

always @(current_state)
 begin: OUTPUT_LOGIC
   case (current_state)
       C0 :CNT = 2'b00;
       C1 :CNT = 2'b01;
       C2 :CNT = 2'b10;
       C3 :CNT = 2'b11;
       default :CNT =2'b00;
   endcase
 end
endmodule
    
 
PROCEDURE:
1.	Open the Verilog design tool (such as Xilinx Vivado / ModelSim / Quartus II).

2.	Create a new project and add a new Verilog module named sync_counter.

3.	Write the Verilog code for a 4-bit synchronous counter using behavioural modelling.

4.	Save and compile the code to check for syntax errors.

5.	Create a testbench module to provide clock and reset signals.

6.	Simulate the design and observe the waveform of the output count.

7.	Verify that the counter increments correctly on every positive edge of the clock.

8.	Synthesize the design and verify the resource utilization report.
Model Viva Questions:
1.	Q: What is a synchronous counter?
 A: A synchronous counter is a counter in which all flip-flops are triggered simultaneously by the same clock signal.

2.	Q: How is a synchronous counter different from an asynchronous counter?
 A: In a synchronous counter, all flip-flops receive the clock at the same time, while in an asynchronous counter, the clock is passed from one flip-flop to the next, causing propagation delay.

3.	Q: What is behavioural modelling in Verilog?
 A: Behavioural modelling describes the circuit’s functionality using high-level constructs like always blocks, if-else, and case statements rather than gate-level connections.

4.	Q: Which Verilog construct is used for sequential logic?
 A: The always block triggered by posedge or negedge of the clock signal is used to describe sequential logic.

5.	Q: What is the purpose of the reset signal in a counter?
 A: The reset signal initializes the counter to a known state, usually zero, regardless of the clock input.

6.	Q: What happens when a 4-bit counter reaches its maximum count (1111)?
 A: After reaching 1111 (15 in decimal), the counter rolls over to 0000 and starts counting again.

7.	Q: How can you convert an up-counter into a down-counter?
 A: Replace the increment operation (count <= count + 1;) with a decrement operation (count <= count - 1;) in the Verilog code.

8.	Q: What is the difference between blocking and non-blocking assignments?
 A:

○	Blocking (=): Executes statements sequentially.

○	Non-blocking (<=): Executes all assignments simultaneously, suitable for sequential logic.

9.	Q: Why do we use posedge clk in the always block?
 A: It ensures that the counter updates only on the positive edge of the clock, mimicking the triggering behavior of flip-flops.

10.	Q: Give some applications of counters.
 A: Counters are used in timers, digital clocks, frequency dividers, event counters, and control systems.


INFERENCE:
The behavioural model of a synchronous counter was successfully designed, simulated, and synthesized using Verilog HDL. The output waveform verified that the counter increments synchronously with the clock signal, demonstrating correct functionality and timing behavior.
