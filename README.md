
# Fibonacci Sequence Calculator in Assembly

This simple assembly program calculates and prints the Fibonacci sequence up to a user-defined maximum value.

## Usage

1. **Input:**
   - Run the program, and it will prompt you to input the maximum value (Fn) for the Fibonacci sequence.

2. **Output:**
   - The program will then display the Fibonacci sequence up to the specified maximum value.

## How to Run

1. **Requirements:**
   - Ensure you have an environment that supports x86_64 assembly.

2. **Compile:**
   - Use an assembler (e.g., NASM) to assemble the code.
     ```bash
     nasm -f elf64 fib.s -o fib.o
     ```

3. **Link:**
   - Link the object file to create the executable.
     ```bash
     ld fib.o -o fib -lc --dynamic-linker /lib64/ld-linux-x86-64.so.2
     ```

4. **Run:**
   - Execute the program.
     ```bash
     ./fib
     ```

## Assembly Code Explanation

The assembly code performs the following steps:

1. **Print Intro Message:**
   - Displays a message asking the user to input the maximum value.

2. **Get User Input:**
   - Receives user input for the maximum value of the Fibonacci sequence.

3. **Initialize Fibonacci Sequence:**
   - Sets up initial values for the Fibonacci sequence.

4. **Print Fibonacci Sequence:**
   - Prints the current Fibonacci number.

5. **Loop to Calculate Fibonacci Sequence:**
   - Continues to calculate and print Fibonacci numbers until the specified maximum value is reached.

6. **Exit:**
   - Exits the program.

## Note
- This program uses x86_64 assembly and assumes that `printf` and `scanf` functions are available externally.

Feel free to explore and modify the code for educational purposes or further enhancements.
