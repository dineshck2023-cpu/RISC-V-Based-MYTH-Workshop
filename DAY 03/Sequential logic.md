SEQUENTIAL LOGIC :
<img width="1520" height="720" alt="WhatsApp Image 2026-06-03 at 11 29 46 AM" src="https://github.com/user-attachments/assets/b23bbea2-9ba5-4262-b572-b00c4c5512a5" />

Sequential logic is a type of digital logic that works
based on a clock signal. Unlike combinational logic,
its output depends not only on the current inputs but
also on previous states stored in memory elements
such as flip-flops. A D flip-flop updates its current
state to the next state whenever a rising edge of the
clock occurs. A reset signal is also used to place the
circuit into a known starting state, ensuring correct
operation when the system begins
<img width="1520" height="720" alt="WhatsApp Image 2026-06-03 at 11 29 45 AM (2)" src="https://github.com/user-attachments/assets/1592bd22-5592-4f46-b0e5-e27e53d3242e" />


The entire sequential circuit can be viewed as a state
machine. The current state is stored in flip-flops,
while combinational logic calculates the next state
from the present state and inputs. On each clock
cycle, the next state becomes the current state,
allowing the circuit to perform step-by-step
operations and remember past information.


FIBONACCI SERIES:
<img width="1520" height="720" alt="WhatsApp Image 2026-06-03 at 11 29 45 AM (1)" src="https://github.com/user-attachments/assets/3f905bcd-26e7-4f00-88fa-587e350b4fdf" />

A simple example of sequential logic is generating
the Fibonacci sequence. In this circuit, the next
number is calculated by adding the previous two
numbers. The values are stored in flip-flops and
updated on every clock cycle. As the clock continues,
the circuit produces the sequence 1, 1, 2, 3, 5, 8, 13,
and so on.

FIBONACCI SERIES - RESET:
<img width="1520" height="720" alt="WhatsApp Image 2026-06-03 at 11 29 45 AM" src="https://github.com/user-attachments/assets/b8e4957a-7cba-4e72-b33d-50efbcb8bd54" />

A reset signal is added to initialize the Fibonacci
circuit. When the reset is active, the output is forced
to a known value, usually 1. After the reset is
released, the circuit resumes normal operation and
continues generating Fibonacci numbers by adding
the two previously stored values. This ensures that
the sequence always starts correctly and operates
reliably.