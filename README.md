# Analog-Hackathon-Data-Encryption
2 bit random number generation under data encryption using Synopsys Custom Compiler in 32nm CMOS Technology
## Table Of Contents
- [Abstract](###Abstract)
- [Circuit Details](###Circuit%20Details)
- [Circuit Diagram](###Circuit%20Diagram)
- [Circuit Waveform](###Circuit%20Waveform)
- [Tool Used](###Tool%20Used)
- [Netlist Genereted](###Netlist%20Generated)
- [Author](###Author)
- [Acknowledgements](###Acknowledgements)
- [References](###References)

### Abstract
This is the implementation of 2-bit Random
number generator in which initial inputs are given
and output will be in random order which will be
helpful for verification engineers to generate random
stimulus for Unit Under Test(UUT) and also used
in data encryption.In this circuit 2-bit shift registers
are used and output from those two flip-flops are
feedback to input of first flip-flop thus it generates
random number.This is implemented using CMOS
technology in Synopsys Custom Design tool.
### Circuit Details
D flip-flops are used to store the previous output
and new output will be based on present input and
previous output which are suitable for using in storing devices such as registers,counters,even memory
can also be implemented. This is the implementation
of 2-bit Random number generator in which initial
inputs are given and output will be in random
order which will be helpful for verification engineers to generate random stimulus for Unit Under
Test(UUT)and also used in data encryption.So,here
two D flip-flops are used to construct shift registers
but output from those two flip-flops are feedback
as input to first flip-flop and initial input is given
which in turn creates random number.Here,I have
contructed D-FF,INVERTER and XNOR module
in CMOS Technology and further it is designed
in structural model(Top-Down approach),Giving inputs like clk and clk1 which are in 180 degree of
phase difference,i.e.,on the high level of clk data
from first flip-flop is read and at level high of
clk1 data from seconf ff is read.Now when resetn
is low initial value 00 is set to ff and further it
changes according to LUT(XOR) and Encrypted got
as output and also 2-bit Random Number is generated.This is implemented using CMOS Technology
in Synopsys Custom Design tool under the Cloud
Based Analog IC Design Hackathon conducted by VSD(VLSI SYSTEM DESIGN) and IIT HYDERABAD in collaboration with Synopsys.
### Circuit Diagram
![ANALOGHACKATHONFINAL](https://user-images.githubusercontent.com/60102705/155479716-6907f7aa-1b87-4f3e-b580-10ad83c9cd8f.png)
### Circuit Waveform
![analoghackwf](https://user-images.githubusercontent.com/60102705/155479921-05219dc6-5437-4dff-b597-7b42c136cc78.png)
### Tool Used
#### Synopsys Custom Compiler
![Screenshot (113)](https://user-images.githubusercontent.com/60102705/155481268-c8e95b0e-ff57-41a5-8a6b-50459eaa7b87.png)

The Synopsys Custom Compiler™ design environment is a modern solution for full-custom analog, custom digital, and mixed-signal IC design. As the heart of the Synopsys Custom Design Platform, Custom Compiler provides design entry, simulation management and analysis, and custom layout editing features. It delivers industry-leading productivity, performance, and ease-of-use while remaining easy to adopt for users of legacy tools.
### Netlist Generated
#### Summary
Tool : Custom Compiler

Version             : S-2021.09

Library             : sidhant_lib

Cell                : Top_Module

View                : schematic

Working Directory   : /home/sidhant1922/Desktop/analog_ic_hackathon

Open Mode           : Edit Mode

Scope               : From Current

Hierarchy Levels    : 1

CountBy             : LCV

Library    :     Cell   :       View      :    Count   

sidhant_lib  :   xnor_gate :    schematic  :   4   

sidhant_lib   :  D_ff       :   schematic   :  2   

sidhant_lib   : inverter    :  schematic    : 1   

Total                 :                      7        
#### Netlist
Find Netlist here:[NetlistAnalog.txt](https://github.com/sidhantp1906/Analog-Hackathon-Data-Encryption-/files/8130734/NetlistAnalog.txt)
### Author
Sidhant Priyadarshi, Student, KLE Technological University, Karnataka, 580031
### Acknowledgements
[1]. https://analog.hackathoniith.in/

[2]. https://www.synopsys.com/

[3]. https://www.vlsisystemdesign.com/
### References
[1] Max Maxfield. Linear Feedback Shift
Registers.
https://www.eetimes.com/tutorial-linear-feedback-shift-registers-lfsrs-part-3

[2]Cadence PCB Solutions. CMOS Design and
circuit simulation tasks .
https://resources.pcb.cadence.com/blog/2020-cmos-vlsi-design-and-circuit-simulation-task
