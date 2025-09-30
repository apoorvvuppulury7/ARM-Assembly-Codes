# AIM
Write an ARM Assembly program to generate the first N prime numbers.

Use ARM Code to understand the running on the Keil Uvision 4 softwares.

# Program Details
TASK :- 
1) Prime Number Generation
   - Write an ARM assembly program that generates the first 20 prime numbers.
   - Store each prime number in a predefined memory location starting at 0x40000000.
   - Verify the prime numbers by inspecting the memory in the debugger.
2) Program Details
   - Initialize the candidate number with 2 (first prime number).
   - Use a loop to check if the candidate number is divisible by any number from 2 up to the square root of the candidate.
   - If the candidate is not divisible by any number in that range, it is prime and should be stored in memory.
   - Increment the candidate number and repeat until the desired number of primes are found.
3) Instructions to Use
   - MOV, ADD, SUBS, STR, LDR
4) Hints
   - Start candidate number with 2.
   - Use a loop to test divisibility.
   - If candidate number is prime, store it using STR and increment the memory pointer.
   - Continue until the required number of primes are stored.
