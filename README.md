# JKFLIPFLOP-USING-IF-ELSE

**AIM:** 

To implement  JK flipflop using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**JK Flip-Flop**

JK flip-flop is the modified version of SR flip-flop. It operates with only positive clock transitions or negative clock transitions. The circuit diagram of JK flip-flop is shown in the following figure.

<img width="554" height="366" alt="Screenshot 2025-12-10 184031" src="https://github.com/user-attachments/assets/90445503-33d7-4e0c-a51b-2d1f0c1dbd90" />

This circuit has two inputs J & K and two outputs Qtt & Qtt’. The operation of JK flip-flop is similar to SR flip-flop. Here, we considered the inputs of SR flip-flop as S = J Qtt’ and R = KQtt in order to utilize the modified SR flip-flop for 4 combinations of inputs. The following table shows the state table of JK flip-flop.

<img width="493" height="334" alt="Screenshot 2025-12-10 185658" src="https://github.com/user-attachments/assets/46be245e-29b1-4244-af33-1db9b768005f" />

 Here, Qtt & Qt+1t+1 are present state & next state respectively. So, JK flip-flop can be used for one of these four functions such as Hold, Reset, Set & Complement of present state based on the input conditions, when positive transition of clock signal is applied. The following table shows the characteristic table of JK flip-flop. Present Inputs Present State Next State
 
 <img width="353" height="288" alt="Screenshot 2025-12-10 185503" src="https://github.com/user-attachments/assets/c439a9f7-c0bb-463c-87a0-970286e62b2b" />

By using three variable K-Map, we can get the simplified expression for next state, Qt+1t+1. Three variable K-Map for next state, Qt+1t+1 is shown in the following figure.
 
<img width="553" height="320" alt="Screenshot 2025-12-10 184310" src="https://github.com/user-attachments/assets/0197c7e6-e25b-4a11-9177-3518f8e3c02a" />

The maximum possible groupings of adjacent ones are already shown in the figure. Therefore, the simplified expression for next state Qt+1t+1 is Q(t+1)=JQ(t)′+K′Q(t)Q(t+1)=JQ(t)′+K′Q(t)

**Procedure**

1.Type the program in Quartus software.
2.Compile and run the program.
3.Generate the RTL schematic and save the logic diagram.
4.Create nodes for inputs and outputs to generate the timing diagram.
5.For different input combinations generate the timing diagram.

**PROGRAM**
```
module LabExercise5 (J,K,Qt,Y);
input J,K,Qt;
output Y;
assign Y = J & ~Qt | ~K & Qt;
endmodule
```

**RTL LOGIC FOR FLIPFLOPS**

<img width="1920" height="1080" alt="Screenshot (61)" src="https://github.com/user-attachments/assets/3f94088f-d85c-40f0-abe3-fec4c8f49d7d" />

**TIMING DIGRAMS FOR FLIP FLOPS**

<img width="1920" height="1080" alt="Screenshot (62)" src="https://github.com/user-attachments/assets/56a8a6a2-7c45-4288-b5a1-1f5a4cd0224e" />

**RESULTS**

This Program was excecuted successfully
