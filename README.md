# hw3-OS
Multithreaded Sum Calculation Program
Description
This program calculates the sum of numbers from 0 to 9999 using multithreading. It divides the task into 10 threads, where each thread calculates the sum of 1000 numbers. The program is implemented in C using the Pthreads library.

Files Included
OSsum.c: The source code for the program.
README.md: This readme file.
Compilation and Execution Instructions
Prerequisites
Make sure you have gcc installed on your system, along with support for Pthreads (which is usually included by default).

Steps to Compile the Program:
Open the terminal and navigate to the directory where OSsum.c is saved.

Run the following command to compile the program:

bash
Copy code
gcc -pthread OSsum.c -o OSsum
This will compile the C program and create an executable file named OSsum.

Steps to Run the Program:
After compiling, you can run the program with the following command:

bash
Copy code
./OSsum
The program will output the total sum from 0 to 9999, which should be:

css
Copy code
Total sum from 0 to 9999: 49995000
How the Program Works
The range of numbers from 0 to 9999 is split into 10 equal parts.
Each thread is responsible for calculating the sum of 1000 numbers.
After all threads finish their calculations, the results are summed up to produce the final result.
