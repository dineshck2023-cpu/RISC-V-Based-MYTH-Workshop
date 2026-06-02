Assembly language (ASM)

<img width="1520" height="720" alt="WhatsApp Image 2026-06-02 at 8 44 24 PM (1)" src="https://github.com/user-attachments/assets/f35d8bef-23ad-4639-b228-7cd77d5af4d2" />


The flowchart explains a simple program that is first written in C language and then rewritten in Assembly (ASM) language. The program starts by setting two registers, a3 and a4, to zero. Another register, a2, is loaded with the value 10, which acts as the loop limit or counter. Inside the loop, the value of a3 is added to a4, so a4 keeps storing the running total. After that, a3 is increased by 1. The program then checks whether a3 is still less than a2. If the condition is true, the loop repeats again. If the condition becomes false, the final value stored in a4 is moved to a0, which is used as the return value, and the program ends. In simple terms, the program calculates the sum of numbers from 0 to 9 using Assembly language instructions.

<img width="1520" height="720" alt="WhatsApp Image 2026-06-02 at 8 44 24 PM" src="https://github.com/user-attachments/assets/a1dd6ba6-55d0-49d6-b611-ee99dfebe201" />


EXAMPLE LAB:
1.Open the terminal in Ubuntu/Linux.


2.Type the following command and press Enter:


leafpad 1to9_custom.c &

3.The following C program will appear in Leafpad:
#include <stdio.h>

extern int load(int x, int y);

int main() {
        int result = 0;
        int count = 9;
        result = load(0x0, count+1);
        printf("Sum of number from 1 to %d is %d\n", count, result);
}

4.Again open the terminal and type:
leafpad load.S &

5.The following Assembly program will appear in Leafpad:
.section .text
.global load
.type load, @function

load:

    add     a4, a0, zero      // Initialize sum register a4 with 0
    add     a2, a0, a1        // Store count value in register a2
    add     a3, a0, zero      // Initialize loop counter a3 with 0

loop:
    add     a4, a3, a4        // Add counter value to sum
    addi    a3, a3, 1         // Increment counter by 1
    blt     a3, a2, loop      // Repeat loop if a3 < a2

    add     a0, a4, zero      // Move final result to a0
    ret                       // Return result

THEN CONTINUE:
<img width="1520" height="720" alt="WhatsApp Image 2026-06-02 at 8 44 23 PM (2)" src="https://github.com/user-attachments/assets/a64c72b9-a8d8-405a-919a-ce9e9fb6b3d3" />

<img width="1520" height="720" alt="WhatsApp Image 2026-06-02 at 8 44 23 PM (1)" src="https://github.com/user-attachments/assets/8e47bd1c-4f54-4e52-8287-0d288b238242" />

<img width="1520" height="720" alt="WhatsApp Image 2026-06-02 at 8 44 23 PM" src="https://github.com/user-attachments/assets/f5cf1c66-aace-4156-aeb4-58a8123035c8" />

<img width="1520" height="720" alt="WhatsApp Image 2026-06-02 at 8 44 22 PM" src="https://github.com/user-attachments/assets/ea794a3b-25fd-4dd1-91b3-746e5165f88f" />



1. Use the following command to display the C program file contents:

cat 1to9_custom.c

2. The C program will be displayed on the terminal screen.

3. Use the following command to display the Assembly program file contents:

cat load.S

4. The Assembly program with comments will appear on the terminal screen.
5. Type the following command to clean the terminal screen:

clear

6. Use the following command to show the files in the folder:

ls

7. Compile the C and Assembly programs using the following command:

riscv64-unknown-elf-gcc -Ofast -mabi=lp64 -march=rv64i -o 1to9_custom.o 1to9_custom.c load.S

8. Execute the generated object file using Spike simulator:

spike pk 1to9_custom.o

9. The output will be displayed as:

Sum of number from 1 to 9 is 45

10. Use the following command to view the disassembled object code:

riscv64-unknown-elf-objdump -d 1to9_custom.o | less

 LAB VERIFICATION:
Step 1: Open Home Directory
cd
Step 2: Clone the GitHub Repository
git clone https://github.com/kunalg123/riscv_workshop_collaterals.git



Step 3: Enter into Repository Folder

cd riscv_workshop_collaterals

Step 4: List the Files

ls -ltr

Step 5: Move to Labs Directory

cd labs

Step 6: List Files in Labs Folder

ls -ltr

Step 7: Open PicoRV32 Verilog File

vim picorv32.v


Step 8: View PicoRV32 File

less picorv32.v

Step 9: Open Testbench File

vim testbench.v

Step 10: Open Shell Script

vim rv32im.sh

Step 11: Give Execute Permission

chmod 777 rv32im.sh

Step 12: Run the Shell Script

./rv32im.sh

Step 13: Open Custom C File

vim 1to9_custom.c

Step 14: Run the Script Again

./rv32im.sh

Step 15: List Generated Files

ls -ltr

Step 16: Open Firmware HEX File

vim firmware.hex

Step 17: Open Firmware32 HEX File

vim firmware32.hex

Step 18: Open Testbench File Again

vim testbench.v
