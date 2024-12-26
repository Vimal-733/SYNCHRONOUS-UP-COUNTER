### SYNCHRONOUS-UP-COUNTER

**AIM:**

To implement 4 bit synchronous up counter and validate functionality.

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 bit synchronous UP Counter**

If we enable each J-K flip-flop to toggle based on whether or not all preceding flip-flop outputs (Q) are “high,” we can obtain the same counting sequence as the asynchronous circuit without the ripple effect, since each flip-flop in this circuit will be clocked at exactly the same time:

![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/d5db3fa0-e413-404c-b80e-b2f39d82e7e8)


![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/52cb61eb-d04b-442d-810c-31185a68410b)

Each flip-flop in this circuit will be clocked at exactly the same time.
The result is a four-bit synchronous “up” counter. Each of the higher-order flip-flops are made ready to toggle (both J and K inputs “high”) if the Q outputs of all previous flip-flops are “high.”
Otherwise, the J and K inputs for that flip-flop will both be “low,” placing it into the “latch” mode where it will maintain its present output state at the next clock pulse.
Since the first (LSB) flip-flop needs to toggle at every clock pulse, its J and K inputs are connected to Vcc or Vdd, where they will be “high” all the time.
The next flip-flop need only “recognize” that the first flip-flop’s Q output is high to be made ready to toggle, so no AND gate is needed.
However, the remaining flip-flops should be made ready to toggle only when all lower-order output bits are “high,” thus the need for AND gates.

**Procedure**

Step 1: Open Quartus II in your laptop.

Step 2: Write code to implement SR flipflop using Verilog and validating their functionality using their functional tables.

Step 3: Run compilation to check for errors.

Step 4: Open waveform output and load input values.

Step 5: Run simulation to get the output.

Step 6: Open in RTL viewers to get RTL diagram output.

**PROGRAM**

/* Program for flipflops and verify its truth table in quartus using Verilog programming. 

Developed by:A.VIMAL
RegisterNumber:24005922
*/

**RTL LOGIC UP COUNTER**
![WhatsApp Image 2024-12-26 at 21 32 18_ea76b682](https://github.com/user-attachments/assets/6cc17b6f-b529-4943-b4d5-0e7e497225bb)

**TIMING DIAGRAM FOR IP COUNTER**
![WhatsApp Image 2024-12-26 at 21 32 43_4694585b](https://github.com/user-attachments/assets/ae6b609d-e93c-4f63-a5ae-eb942f26f7af)

**TRUTH TABLE**
![WhatsApp Image 2024-12-26 at 21 16 20_b1b4ea9a](https://github.com/user-attachments/assets/359ca91b-7257-40f5-bfb2-a058d9a17fe0)

**RESULTS**
The observation of the simulation results and confirm the successful execution of the program.
