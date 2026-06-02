
# CONTENTS 
<img width="1520" height="720" alt="WhatsApp Image 2026-06-02 at 6 53 03 PM (7)" src="https://github.com/user-attachments/assets/febddaea-2894-4e55-a2c8-badf5388cd0e" />

Pseudo Instructions

Pseudo instructions are shortcut commands used in RISC-V assembly language to make programming easier and simpler. These instructions are not directly executed by the processor. Instead, the assembler converts them into real machine instructions. They help programmers write readable and shorter code.

Base Integer Instructions – RV64I

RV64I is the basic 64-bit instruction set of the RISC-V processor. It contains fundamental operations such as addition, subtraction, loading and storing data, branching, and logical operations. It forms the core foundation of the processor and allows the CPU to perform normal integer calculations and data handling.




Multiply Extension – RV64M

RV64M is an extension that adds multiplication, division, and remainder operations to the processor. Without this extension, the processor can only perform basic arithmetic operations. It improves the processor’s ability to handle mathematical calculations efficiently.

Single and Double Precision Floating Point – RV64F & RV64D

RV64F and RV64D are floating-point extensions used for decimal number calculations. RV64F handles single-precision 32-bit floating-point numbers, while RV64D handles double-precision 64-bit floating-point numbers with higher accuracy. These extensions allow the processor to perform precise decimal arithmetic operations.

Application Binary Interface (ABI)

ABI is a set of rules that defines how programs and functions communicate with each other. It specifies how data is passed between functions, how return values are stored, and which registers are used during execution. ABI ensures compatibility between software, compilers, and the operating system.

Memory Allocation and Stack Pointer

Memory allocation is the process of reserving memory space for variables and program data. The stack pointer (sp) is a special register that points to the top of stack memory. The stack stores temporary data, function information, and local variables during program execution. The stack grows and shrinks as functions are called and completed.


Floating Point Addition

Floating-point addition is the process of adding decimal numbers in the processor. RISC-V uses floating-point registers and special instructions to perform these operations accurately. It allows the processor to handle decimal arithmetic efficiently and precisely.

Next continue 
<img width="1520" height="720" alt="WhatsApp Image 2026-06-02 at 7 19 39 PM (2)" src="https://github.com/user-attachments/assets/c983aae8-86ce-4910-bb81-e91922a4d0e6" />

<img width="1520" height="535" alt="WhatsApp Image 2026-06-02 at 7 19 39 PM (1)" src="https://github.com/user-attachments/assets/6e571441-d948-46cc-a9b6-d21f5bb6c1f5" />

<img width="1520" height="720" alt="WhatsApp Image 2026-06-02 at 7 19 39 PM" src="https://github.com/user-attachments/assets/b871a4db-70d4-4e9e-ad8b-7eb016c94ff5" />

A computer stores and processes data using binary numbers made of only 0s and 1s. The smallest unit of data is called a bit. A group of 8 bits forms a byte. Larger groups are used to handle bigger numbers, such as a word which is 32 bits (4 bytes) and a doubleword which is 64 bits (8 bytes). In a 64-bit number, the leftmost bit is called the MSB (Most Significant Bit) because it has the highest value, while the rightmost bit is called the LSB (Least Significant Bit) because it has the lowest value. Processors like RISC-V use these binary values to perform operations such as addition, multiplication, and division for both integers and floating-point numbers. A 64-bit doubleword can represent very large unsigned values ranging from 0 to 2 ^64 - 1.
 Example program:
<img width="1520" height="720" alt="WhatsApp Image 2026-06-02 at 7 19 38 PM (2)" src="https://github.com/user-attachments/assets/fbfe6dbe-12cb-4362-b842-f3698d16c40e" />

<img width="1520" height="720" alt="WhatsApp Image 2026-06-02 at 7 19 38 PM (1)" src="https://github.com/user-attachments/assets/1a57d27c-c475-4301-8bce-ffef2ceffd67" />

<img width="1520" height="720" alt="WhatsApp Image 2026-06-02 at 7 19 38 PM" src="https://github.com/user-attachments/assets/a18a20b8-1422-41d5-be3a-fb2c5d5391dd" />

<img width="1520" height="720" alt="WhatsApp Image 2026-06-02 at 7 19 37 PM" src="https://github.com/user-attachments/assets/0547ed3f-db64-4763-a924-c65c9eb9b806" />
