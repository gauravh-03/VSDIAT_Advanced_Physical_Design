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




