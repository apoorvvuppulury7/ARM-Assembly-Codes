# AIM
Write an ARM Assembly program to toggle LEDs connected to Port 1.16–P1.23 using specific patterns.

Use Toggle Code to understand the running on the Keil Uvision 4 softwares.

# Program Details
TASK :- 
1) Prime Number Generation
   - Configure GPIO pins P1.16–P1.23 as output.
   - Continuously write two patterns (0x55 and 0xAA) to the port to toggle the LEDs.
   - Verify the LED toggle effect on the hardware or simulator.
2) Program Details
   - Use IO1DIR register to set direction of Port 1 pins as output.
   - Use IO1PIN register to write patterns to LEDs.
   - Alternate between 0x55 and 0xAA shifted into P1.16–P1.23.
   - Use an infinite loop to repeat toggling.
3) Instructions to Use
   - LDR, STR, B
4) Hints
   - Use IO1DIR to configure pins P1.16–P1.23 as outputs (mask = 0x00FF0000).
   - Write 0x00550000 and 0x00AA0000 alternately to IO1PIN to toggle LEDs.
   - Use an infinite loop to continuously change LED states.
