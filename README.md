# VSDIAT_Advanced_Physical_Design
Introduction: 

Electronic board ex. Arduino board.
In the center of the electronic board is chip.

![image](https://github.com/gauravh-03/VSDIAT_Advanced_Physical_Design/assets/165159967/c3bd773f-87eb-4660-9080-ca0669a075c8)

This is an Arduino board.

![image](https://github.com/gauravh-03/VSDIAT_Advanced_Physical_Design/assets/165159967/ea6a2294-6518-4705-a930-8b2cd903de34)

This is the chip present in the Arduino board.

The chip is present in the center of the package.
The outside connections are passed into the chip by wires pounds.

Some important components are:

1. Pads - used to send signals inside the chip from outside and vice-versa.

2. Core - holds all the digital logic.

3. Die - it is the entire size of the chip.

A typical chip consists of various parts such as: SPI ,SRAM ,RISCV SOC ,PLL, adc0, adc1 and dac.
The PLL,adc0,adc1,dac and SRAM are foundry Ip's.
The RISCV SOC and SPI are the Macros.

Foundry- A foundry is a place where chips get manufactured.

RISCV INSTRUCTION SET ARCHITECTURE(ISA):

ISA - it is a way to talk to the computer.
When we need to run a certain C programme on a particular layout we must compile the C pragramme in its assembly language programme, the RISCV assembly proggramme is later converted into machine language programme(binary code).
We must implement the RISCV programme in some RTL(ex.picorv32 cpu core)

Application software(apps) to hardware-

The application software is coverted into the system software which is the converted into the hardware.
The system software contains three major components:
1. Operating system
2. Compiler
3. Assembler
The operating system handles various functions such as -
1. Handle IO operations
2. Allocate memory
3. Low level system functions

The output of the OS are small functions such as C,C++,VB,JAVA,etc.
These are compiled into instructions.
The assembler coverts the instructions into the binary code(machine language programme).
The instructions acts as an abstract interface.

ASIC design:

ASIC design requires three important elements:
1. RTL designs
2. EDA tools
3. PDK data

An opensource ASIC design requires opensource RTL designs, opensource EDA tools and opensource PDK data.
Some opensource RTL design sites are Librecores.org, Opencores.org, and Github.com.
Some opensource EDA tools are Qflow, Openroad, and Openlane.

PDK(Process Design Kit):
It is a collection of files used to model a fabrication process for the EDA tools used to design an IC.

Simplified RTL to GDSII flow:

The major processes invovled are :
1. Synthesis
2. Floor/Power planning
3. Placement
4. Clock Tree Synthesis
5. Routing
6. Sign off

Synthesis: Converts RTL to a circuit  out of components from the standard cell library.

FP+PP:
Macro floor planning - define dimensions, pin locations and rows definition.
Power planning - the power network is constructed.

Placement: place the cells on the power plan rows, aligned with the sites.

CTS: create a clock distribution network.

Routing: implement the interconnect using the available metal layers.

Sign off: once done with routing,we construct the final layout, which undergoes physical verfication and timing verification.

Openlane started out as an open source flow for a true open source tape out experiment.

striVe SoC family:
1. striVe   - Sky130 SCL + Synthesized 1 Kbytes SRAM
2. striVe2  - Sky130 SCL + 1 Kbytes OpenRAM block
3. striVe2a - striVe2 with a single chip core module
4. striVe3  - OSU SCL + Synthesized 1 Kbytes SRAM
5. striVe5  - Sky130 SCL + 8*1 Kbytes OpenRAM banks
6. striVe6  - striVe2 with DFT

Main goal of OpenLane : Produce a clean*GDSII with no human intervention.

*clean means: 
1. No LVS violations
2. No DRC violations
3. No timing violations

![image](https://github.com/gauravh-03/VSDIAT_Advanced_Physical_Design/assets/165159967/68d01b3a-99d6-4605-80d4-c46cb8d409da)
OPENLANE ASIC FLOW CHART







