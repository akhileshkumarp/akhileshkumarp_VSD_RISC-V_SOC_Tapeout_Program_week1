Day1:

Introduction to Verilog design and synthesis.

Introduction to open-source simulator iverilog     
2-SKY130RTL D1SK1 L1 Introduction to iverilog design test bench
Simulator: It is a tool/program which detects the changes in the inputs and forms changes in the output.
given below a look of a basic simulator block diagram.
[![Day1_1](../week1_assets/Day1_1.png)](../week1_assets/Day1_1.png)
given bleow the flow of iverilog and gtkwave.
[![Day1_2](../week1_assets/Day1_2.png)](../week1_assets/Day1_2.png)

LABS: 
Labs using Iverilog and GTKWave.
3-SKY130RTL D1SK2 L1 Lab1 introduction to lab
step1: clone repo files for labs by command: git clone https://github.com/kunalg123/sky130RTLDesignAndSynthesisWorkshop.git
[![Day1_repo_clone](../week1_assets/Day1_repo_clone.png)](../week1_assets/Day1_repo_clone.png)

[![Day1_repo_contents](../week1_assets/Day1_repo_contents.png)](../week1_assets/Day1_repo_contents.png)

4-SKY130RTL D1SK2 L2 Lab2 Introduction iverilog gtkwave part1
Simulate a good_mux using iverlog and view and analyze the waveform using gtkwave tool.
[![Day1_intro_to_iverilog_gtkwave_part1](../week1_assets/Day1_intro_to_iverilog_gtkwave_part1.png)](../week1_assets/Day1_intro_to_iverilog_gtkwave_part1.png)

5-SKY130RTL D1SK2 L3 Lab2 Introduction iverilog gtkwave part2
[![Day1_mux_codes](../week1_assets/Day1_mux_codes.png)](../week1_assets/Day1_mux_codes.png)

Introduction to Yosys and logic synthesis
6-SKY130RTL D1SK3 L1 Introduction to yosys
Synthesizer: used to convert RTL logic to netlist.
[![Day1_Yosys_structure](../week1_assets/Day1_Yosys_structure.png)](../week1_assets/Day1_Yosys_structure.png)
Verify the synthesis by simulation of netlist with the tb, match the results of both behavioural and netlist simulation runs with the same testbench code. 

7-SKY130RTL D1SK3 L2 introduction to logic synthesis part1
RTL is written in verlog HDL.
we need a digital circuit made of hardware circuit. 
The key is synthesis, design is converted to the gate level netlist. 
A .lib is a collectiono of logic modules such as AND, OR, XOR with different speed or types.
Why need different flavours of gates: 
Because of the setup and hold issues.

8-SKY130RTL D1SK3 L3 introduction to logic synthesis part2
Need to guide the synthsize to select the best logical cells that is ideal for the logic circuit.
balance between power performance and are. 
the guidance can be given to the synthesis tool in the form of constraints file. 

Labs using Yosys and Sky130PDKs
9-SKY130RTL D1SK4 L1 Lab3 Yosys 1 good mux Part1
read .lib 
read verilog 
synth -top module_name
[![Day1_yosys_synthesis_start](../week1_assets/Day1_yosys_synthesis_start.png)](../week1_assets/Day1_yosys_synthesis_start.png)
[![Day1_yosys_mux_synth_done](../week1_assets/Day1_yosys_mux_synth_done.png)](../week1_assets/Day1_yosys_mux_synth_done.png)
[![Day1_yosys_abc_report](../week1_assets/Day1_yosys_abc_report.png)](../week1_assets/Day1_yosys_abc_report.png)
[![Day1_yosys_show](../week1_assets/Day1_yosys_show.png)](../week1_assets/Day1_yosys_show.png)

10-SKY130RTL D1SK4 L2 Lab3 Yosys 1 good mux Part2
Analyse the synthesized image. 

11-SKY130RTL D1SK4 L3 Lab3 Yosys 1 good mux Part3
[![Day1_yosys_output_netlist](../week1_assets/Day1_yosys_output_netlist.png)](../week1_assets/Day1_yosys_output_netlist.png)