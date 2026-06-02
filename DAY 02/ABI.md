APPLICATION BINARY INTERFACE ( ABI )
An Application Binary Interface (ABI) is the low-level connection between compiled software and the computer system. It defines how machine-level programs interact with the operating system, processor, and hardware. The concept is shown using assembly instructions, operating systems, standard libraries, and processor architectures such as x86, ARM, and RISC-V.

<img width="1520" height="720" alt="WhatsApp Image 2026-06-02 at 8 31 00 PM (2)" src="https://github.com/user-attachments/assets/6e8a6f67-d53f-484f-99b8-6fa0e84b5785" />


The explanation starts from a compiled program containing assembly instructions. These instructions follow ABI rules so the processor knows how to execute them correctly. The ABI specifies things like:

how function calls are made,

which CPU registers store arguments and return values,

how the stack and memory are organized,

how programs request operating system services through system calls.


The flow begins with an application program, such as an email app, which uses APIs from programming languages and libraries. Those libraries communicate with the operating system using system calls. The ABI defines the binary-level rules for this communication.

The operating system then interacts with the processor through the Instruction Set Architecture (ISA), such as RISC-V, ARM, or x86. Beneath that is the actual hardware implementation. Different processors may be designed for high performance or low power, but if they follow the same ABI and ISA rules, the same compiled program can still run correctly.

In simple terms:

API helps programmers write software.

ABI helps compiled software run correctly on a system.
ISA defines the CPU instructions understood by the processor.
The main idea is that the ABI acts as a stable bridge between software and hardware, ensuring compatibility at the machine-code level.

<img width="1520" height="720" alt="WhatsApp Image 2026-06-02 at 8 31 00 PM" src="https://github.com/user-attachments/assets/ad4bcd00-b763-40a3-a8c5-b0c2178ea9fd" />

<img width="1520" height="720" alt="WhatsApp Image 2026-06-02 at 8 31 00 PM (1)" src="https://github.com/user-attachments/assets/bf151a34-6c35-4015-9b00-d8f27cdf38f2" />

A computer works using binary numbers, which are made of only 0s and 1s called bits. More bits can represent more values. For example, 2 bits can store 4 values, 3 bits can store 8 values, and 4 bits can store 16 values. In computers, 8 bits make 1 byte, 4 bytes make 1 word, and 8 bytes make 1 doubleword. The processor performs two main types of calculations: integer operations for whole numbers and floating-point operations for decimal numbers.

The processor also contains small and very fast storage locations called registers, which are used during calculations and program execution. In RISC-V, there are 32 registers named x0 to x31, and each has a specific purpose. For example, x0 always stores 0, x1 stores the return address after a function call, x2 acts as the stack pointer, and some registers are used for temporary values or passing function arguments. Functions also follow rules about saving and restoring register values, known as caller-saved and callee-saved registers.

<img width="1520" height="720" alt="WhatsApp Image 2026-06-02 at 8 30 59 PM" src="https://github.com/user-attachments/assets/01393b66-103d-4986-9d6d-cc43ebfd198e" />


