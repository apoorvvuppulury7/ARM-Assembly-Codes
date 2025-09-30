# AIM
Write an ARM Assembly program to implement an 8-bit LFSR (Linear Feedback Shift Register) to generate pseudo-random patterns and display them on Port1 LEDs (P1.0 – P1.7).

Use ARM Code to understand the running on the Keil Uvision 4 softwares.

# Program Details
1) Task
   - Implement an 8-bit LFSR using ARM assembly.
   - Display the generated pseudo-random patterns on LEDs connected to Port1.
   - Verify the random sequence by observing the output patterns in the Watch Window or LEDs.
   - Ensure that the seed value is non-zero to avoid the register getting stuck.
2) Program Details
   - Initialize Port1 pins (P1.0–P1.7) as output.
   - Load an initial non-zero seed value into the LFSR.
   - Update the LFSR on each iteration using XOR feedback taps.
   - Output the new LFSR value to Port1.
   - Continue indefinitely to generate a stream of pseudo-random patterns.
3) Instructions to Use
   - MOV, STR, LDR, LSL, LSR, ORR, EOR, B, BEQ, BNE
4) Hints
   - Use taps at bits 7, 5, 4, and 3 for an 8-bit maximal length LFSR.
   - Ensure seed ≠ 0, otherwise LFSR will lock in zero state.
   - Add a delay loop if using physical LEDs to make patterns visible.
