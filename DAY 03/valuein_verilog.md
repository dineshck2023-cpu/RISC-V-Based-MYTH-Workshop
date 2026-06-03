VALUES IN VERILOG :

<img width="1520" height="720" alt="WhatsApp Image 2026-06-03 at 11 40 48 AM" src="https://github.com/user-attachments/assets/0278895f-c59d-45a1-b12d-29f3f986c869" />


In Verilog, numbers are written using a special
format that shows the size, number system, and
value. For example, 16'hF0 means a 16-bit
hexadecimal value. Here, 16 represents the number
of bits, h represents hexadecimal format, and F0 is
the actual value. This helps the simulator know
exactly how many bits are being used.
Verilog also supports special values. '0 means all bits
are set to 0, with the width determined by the
context. 'X means all bits are "don't care" values,
which can be either 0 or 1. For example, 16'd5
represents the decimal value 5 stored in a 16-bit
number, while 5'b00XX1 represents a 5-bit binary
value where the middle bits are don't-care bits.
If a number is written simply as 1, Verilog treats it as
a 32-bit signed value by default. During simulation, if
the width of a value does not match the width of a
signal, the simulator may automatically add zeros
(zero-extension) or remove extra bits (truncation).
The simulator used here works with 2-state
simulation, meaning signals can only be 0 or 1, and it
does not use unknown X states during simulation.