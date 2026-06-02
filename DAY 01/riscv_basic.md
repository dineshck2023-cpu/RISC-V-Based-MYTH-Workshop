# INTRODUCTION TO RISC-V INSTRUCTION SET ARCHITECTURE:
RISC-V is an open-source instruction set architecture used to design modern processors. In this project, the complete flow of RISC-V processor development is studied from software level to hardware implementation. The process begins with generating RISC-V instructions from a program, followed by implementing the processor architecture using hardware design techniques. The designed processor is then converted into logic circuits and finally transformed into a physical chip layout for fabrication. This project helps in understanding the overall flow of processor design, including architecture, implementation, and physical realization of a RISC-V based CPU.

<img width="1520" height="720" alt="WhatsApp Image 2026-06-02 at 6 53 03 PM (10)" src="https://github.com/user-attachments/assets/131ca29d-9798-4301-a13e-461421348421" />

•A computer system mainly has three parts: application software, system software, and hardware. Application software includes programs we use daily such as Word, PowerPoint, Excel, Firefox, and VirtualBox. These applications help users do tasks like writing documents, browsing the internet, or creating presentations. System software acts like a bridge between the applications and the hardware. It includes operating systems such as Windows, Linux, and macOS, which manage the computer and allow applications to run properly. Programming languages like C, C++, Java, and VB are converted into machine-understandable instructions using tools such as a compiler and assembler. The compiler changes the program into lower-level instructions, and the assembler converts them into binary code (0s and 1s). Finally, the hardware executes these instructions. Hardware includes physical parts and electronic circuits inside the computer chip. In simple terms, application software helps the user, system software controls and translates commands, and hardware performs the actual work.

<img width="1520" height="720" alt="WhatsApp Image 2026-06-02 at 6 53 03 PM (9)" src="https://github.com/user-attachments/assets/da2b0759-5d43-4232-bded-f95d7bf17212" />

<img width="1520" height="720" alt="WhatsApp Image 2026-06-02 at 6 53 03 PM (8)" src="https://github.com/user-attachments/assets/2e216f32-9ff8-4b79-a6e4-c0186f8741e5" />

Part 1 – RISC-V Instruction Set Architecture (ISA)

This stage focuses on understanding the instruction set of the processor. The RISC-V ISA defines how the CPU communicates using instructions such as arithmetic, memory access, and logical operations. Assembly instructions are converted into binary machine code that the processor can understand and execute. This part mainly explains the basic architecture and working flow of the processor instructions.

Part 2 – RTL and Synthesis of RISC-V CPU Core

In this stage, the processor is designed using RTL (Register Transfer Level) coding, usually written in Verilog. The RTL describes how data moves inside the CPU and how different hardware blocks function together. After writing the RTL code, synthesis is performed to convert the design into a gate-level netlist made of logic gates and flip-flops.
Part 3 – Physical Design Implementation

This stage converts the synthesized netlist into an actual hardware layout. Different electronic components are placed and connected on the chip to create the final processor hardware. Physical design includes placement, routing, and optimization to ensure the chip works correctly and efficiently in real hardware form.


LAB 01
  
Steps to Run the Program in Ubuntu

1. Open Terminal
Press:
Ctrl + Alt + T
2. Go to Home Directory
cd
3. Create C File Using Leafpad
leafpad sum1ton.c
4. Type the Program
#include <stdio.h>

int main()
{
    int i, sum = 0, n = 100;

    for(i = 1; i <= n; ++i)
    {
        sum += i;
    }

    printf("Sum of numbers from 1 to %d is %d", n, sum);

    return 0;
}


5. Save the File
Click File → Save
Close Leafpad
6. Compile the Program
gcc sum1ton.c
7. Run the Program
./a.out
8. Output
Sum of numbers from 1 to 100 is 5050

<img width="1520" height="720" alt="WhatsApp Image 2026-06-02 at 6 53 03 PM (6)" src="https://github.com/user-attachments/assets/b4191fb7-137e-41a4-b025-8f5c6d681719" />
LAB CONTINUE 
Commands with comments
# Display the C program
cat sum1ton.c

# Compile the program for RISC-V architecture
riscv64-unknown-elf-gcc -O1 -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c

# List the generated object file
ls -ltr sum1ton.o

# Display assembly/disassembly code of object file
riscv64-unknown-elf-objdump -d sum1ton.o

# View assembly output page by page
riscv64-unknown-elf-objdump -d sum1ton.o | less

# Compile with fast optimization
riscv64-unknown-elf-gcc -Ofast -mabi=lp64 -march=rv64i -o sum1ton.o sum1ton.c
Next continue:
<img width="1520" height="720" alt="WhatsApp Image 2026-06-02 at 6 53 03 PM (5)" src="https://github.com/user-attachments/assets/a121b5df-1e79-4181-afa3-77ecb1205061" />

<img width="1520" height="720" alt="WhatsApp Image 2026-06-02 at 6 53 03 PM (4)" src="https://github.com/user-attachments/assets/caf764a9-2908-4823-88d6-e87a29cb0b56" />
<img width="1520" height="720" alt="WhatsApp Image 2026-06-02 at 6 53 03 PM (3)" src="https://github.com/user-attachments/assets/8d4207e7-8a2c-4ce8-820c-11d036632008" />
<img width="1520" height="720" alt="WhatsApp Image 2026-06-02 at 6 53 03 PM (2)" src="https://github.com/user-attachments/assets/3eca9a23-905d-466e-a173-459d872f3738" />
<img width="1520" height="720" alt="WhatsApp Image 2026-06-02 at 6 53 03 PM (1)" src="https://github.com/user-attachments/assets/ceaad01e-9149-479a-a9d7-7afdaecfc083" />
<img width="1520" height="720" alt="WhatsApp Image 2026-06-02 at 6 53 03 PM" src="https://github.com/user-attachments/assets/85855982-fb72-466e-ae91-b6ccea3a9e88" />
