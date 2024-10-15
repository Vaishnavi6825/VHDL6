# VHDL6
A Multiplexer (MUX) is a combinational circuit that selects one of several input signals and forwards the selected input to a single output line. <br>
A 4x1 multiplexer has four input data lines, two select lines, and one output.  <br>
Inputs:  <br>
D0, D1, D2, D3: The four input data lines.  <br>
S1, S0: Two select lines used to select one of the four input data lines.  <br>
Output:  <br>
Y: The output data line that represents the selected input. <br>

`Aim`: <br>

To design and simulate a 4x1 multiplexer using Verilog HDL and verify its functionality through simulation.

`Apparatus Required:`

-Xilinx Vivado (or any Verilog simulator).<br>
-PC/Laptop with required software tools.<br>

`Code Implementation:`

``module mux_4to1(input [3:0] d, input [1:0] sel, output y);
  assign y = (sel == 2'b00) ? d[0] :
             (sel == 2'b01) ? d[1] :
             (sel == 2'b10) ? d[2] :
             d[3];
endmodule``

![WhatsApp Image 2024-10-15 at 18 16 36_fde7bb14](https://github.com/user-attachments/assets/b4173d46-3dc2-470e-afd3-ff9029d8f5f6)

`Output Waveform:`

![WhatsApp Image 2024-10-15 at 18 16 02_337ed5fd](https://github.com/user-attachments/assets/fdea35b3-4a85-4303-b824-992d5de1a457)

`Result:`

The 4x1 multiplexer was successfully designed and simulated using Verilog HDL.<br>
The output matched the expected behavior based on the truth table of a 4x1 multiplexer, with the correct input being selected for each combination of the select lines.<br>


