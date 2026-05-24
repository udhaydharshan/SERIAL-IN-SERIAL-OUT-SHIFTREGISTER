<img width="814" height="532" alt="image" src="https://github.com/user-attachments/assets/aaca5303-495c-43dc-b205-f7ab090fe582" /># SERIAL-IN-SERIAL-OUT-SHIFTREGISTER

**AIM:**

To implement  SISO Shift Register using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**SISO shift Register**

A Serial-In Serial-Out shift register is a sequential logic circuit that allows data to be shifted in and out one bit at a time in a serial manner. It consists of a cascade of flip-flops connected in series, forming a chain. The input data is applied to the first flip-flop in the chain, and as the clock pulses, the data propagates through the flip-flops, ultimately appearing at the output.

The logic circuit provided below demonstrates a serial-in serial-out (SISO) shift register. It comprises four D flip-flops that are interconnected in a sequential manner. These flip-flops operate synchronously with one another, as they all receive the same clock signal.

![image](https://github.com/naavaneetha/SERIAL-IN-SERIAL-OUT-SHIFTREGISTER/assets/154305477/e81c4072-37f9-46c6-8145-566764b74c3a)

Figure 01 4 Bit SISO Register

The synchronous nature of the flip-flops ensures that the shifting of data occurs in a coordinated manner. When the clock signal rises, the input data is sampled and stored in the first flip-flop. On subsequent clock pulses, the stored data propagates through the flip-flops, moving from one flip-flop to the next.
Each D flip-flop in the circuit has a Data (D) input, a Clock (CLK) input, and an output (Q). The D input represents the data to be loaded into the flip-flop, while the CLK input is connected to the common clock signal. The output (Q) of each flip-flop is connected to the D input of the next flip-flop, forming a cascade.

**Procedure**

/* write all the steps invloved */

**PROGRAM**
```
/* Program for flipflops and verify its truth table in quartus using Verilog programming.
Developed by: UDHAYDHARSHAN S
RegisterNumber: 212225230286
*/
module deexp2(a,b,c,d,f1,w,x,y,z,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1=((~b&~d)| (~a&b&d)| (a&b&~c));
assign f2=((~y&z)|(x&y)|(w&y));
endmodule

```
RTL realization
<img width="814" height="532" alt="Screenshot 2026-05-24 220749" src="https://github.com/user-attachments/assets/146169c9-17c1-4873-843e-a35261949547" />

**RTL LOGIC FOR SISO Shift Register**
<img width="1365" height="498" alt="Screenshot 2026-05-24 220601" src="https://github.com/user-attachments/assets/aa830144-31ea-4d21-a038-e61739d77864" />


**TIMING DIGRAMS FOR SISO Shift Register**
<img width="938" height="402" alt="image" src="https://github.com/user-attachments/assets/d1404354-9c42-4dd7-aee8-daa0210b6273" />

**RESULTS**
