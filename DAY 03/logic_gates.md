
*GitHub link for workshop resources*
https://github.com/stevehoover/RISCV_MYTH_Workshop

Logic Gates :
<img width="1520" height="720" alt="WhatsApp Image 2026-06-03 at 10 45 49 AM (5)" src="https://github.com/user-attachments/assets/2b04dddf-85d1-4e7d-954d-18ab07a21bd7" />

Logic gates are the basic building blocks of digital
circuits. They take one or more binary inputs (0 or 1)
and produce a binary output. A NOT gate gives the
opposite value of the input. An AND gate gives 1 only
when all inputs are 1. An OR gate gives 1 if at least
one input is 1. An XOR gate gives 1 when the inputs
are different. NAND, NOR, and XNOR are the
opposite versions of AND, OR, and XOR respectively.
Truth tables are used to show the output for every
possible input combination.

Combinational Circuit :
<img width="1520" height="720" alt="WhatsApp Image 2026-06-03 at 10 45 49 AM (4)" src="https://github.com/user-attachments/assets/08391fef-1ed0-4903-9a8c-f33fc8efa5b4" />

A combinational circuit produces outputs based only
on the current input values. In the shown circuit, XOR,
AND, and OR gates are connected to form a full
adder. The inputs are A, B, and Cin (carry input),
while the outputs are S (sum) and Cout (carry
output). The output changes immediately when the
inputs change.

Adder :
<img width="1520" height="720" alt="WhatsApp Image 2026-06-03 at 10 45 49 AM (3)" src="https://github.com/user-attachments/assets/892cf364-89b0-4951-ae35-ce61bfd76dc3" />

An adder is a digital circuit used to perform binary
addition. A full adder adds two input bits and a carry
input, producing a sum and a carry output. Multiple
full adders can be connected together to add larger
binary numbers. The carry output from one stage
becomes the carry input for the next stage.

Boolean Operators :
<img width="1520" height="720" alt="WhatsApp Image 2026-06-03 at 10 45 49 AM (2)" src="https://github.com/user-attachments/assets/28a15b57-0a80-4d45-b327-758616f114cb" />

Boolean operators are used to perform logical
operations on binary values. Common operators
include NOT, AND, OR, XOR, NAND, NOR, and XNOR.
In Verilog, symbols such as ~, &, |, and ^ represent
these operations. These operators help describe
digital logic circuits in hardware design

Multiplexer (MUX) :
<img width="1520" height="720" alt="WhatsApp Image 2026-06-03 at 10 45 49 AM (1)" src="https://github.com/user-attachments/assets/56434590-e230-453e-b8f8-f418b2b104ba" />

A multiplexer, or MUX, is a circuit that selects one of
several input signals and sends it to a single output.
The selection is controlled by a select signal. In the
example, if the select signal S is 1, the output
becomes X1; otherwise, the output becomes X2. In
Verilog, this can be written using the ternary
operator

Chaining Ternary Operator :
<img width="1520" height="720" alt="WhatsApp Image 2026-06-03 at 10 45 49 AM" src="https://github.com/user-attachments/assets/3fd15b24-b079-4e8d-a293-0d039ce8003e" />

A ternary operator is used in Verilog to choose
between values based on conditions. Multiple ternary
operators can be connected together to select from
several inputs. This method works like a multiplexer,
where different select signals determine which input
appears at the output. The conditions are checked in
order, and the first true condition decides the output
value