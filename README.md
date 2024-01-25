# Process Scheduler and Memory Manager

## Overview

This project involves the implementation of a process scheduler and memory manager. The system will handle multiple programs with variable assignments, arithmetic operations, file I/O, and print commands. Two scheduling algorithms, Round Robin and Shortest Job First, will be implemented to manage process execution efficiently.

## Input

The project takes three text files as input, each containing programs with specific syntax and format. These programs will be processed and executed by the system. The assumed scenario is that all programs arrive at time zero.

## Components to Implement

1. **Queue: Ready Queue**
   - Create a data structure for the ready queue.

2. **Memory Management**
   - Implement memory allocation to store variables and program data.

3. **PCB (Process Control Block)**
   - Define the PCB structure with Process ID, Program Counter, and Memory Boundaries.

4. **Scheduling Algorithms**
   - Implement Round Robin and Shortest Job First algorithms.

5. **Functions/Operations**
   - Variable Assignment: Implement 'assign' operation, handling direct value assignment and user input.
   - Arithmetic Operations: Implement add, subtract, multiply, and divide operations.
   - File I/O: Implement writeFile and readFile operations for handling data storage and retrieval from files (create a new file if it doesn't exist).
   - Print Commands: Implement commands for displaying output.

6. **Execution Monitoring**
   - Iterate through parsed instructions and execute them based on scheduling algorithms.
   - Print the current process executing at each cycle.
   - Track and print when each process finishes execution.

## Implementation Steps

1. **Initialize Queues and Memory**
   - Create a data structure for the Ready queue.
   - Implement memory allocation to store variables and program data.

2. **Parsing Programs**
   - Read each input text file containing programs.
   - Parse instructions from each file and organize them for execution.
   - Identify and categorize instructions.

3. **Implement Operations**
   - Variable Assignment: Implement 'assign' operation.
   - Arithmetic Operations: Implement add, subtract, multiply, divide operations.
   - File I/O: Implement writeFile and readFile operations.

4. **Scheduling Algorithms**
   - Implement Round Robin (quantum=2) and Shortest Job First algorithms.
   - Define time-slice for Round Robin and criteria for Shortest Job First.

5. **Execution Control**
   - Iterate through parsed instructions and execute them based on scheduling algorithms.
   - Print the current process executing at each cycle.
   - Track and print when each process finishes execution.

6. **Testing and Debugging**
   - Test implementation with various input programs to ensure correct execution.
   - Debug any issues encountered during testing.

## Expected Outputs at Each Clock Cycle

1. **Ready Queues**
   - Display the contents of the Ready queue.

2. **Processor Status**
   - Indicate which process is currently on the processor (CPU).

3. **Memory State**
   - Showcase the state of memory after each operation:
     - Variables and their assigned values.
     - Any changes in memory due to file I/O or program execution.

4. **Gantt Chart**
   - Display the Gantt chart for each scheduling algorithm.

## Evaluation Criteria

1. **Correctness**
   - Verify accurate functioning of implemented operations.
   - Validate correct variable values after assignments and arithmetic operations.
   - Ensure accuracy of file I/O operations.

2. **Scheduling Algorithms**
   - Evaluate Round Robin and Shortest Job First algorithms.
   - Confirm correct rotation of processes based on time slices (Round Robin).
   - Validate prioritization of shortest tasks (Shortest Job First).

3. **Execution Monitoring**
   - Validate accurate display of the current executing process.
   - Ensure precise process completion tracking for each clock cycle.

4. **Memory Management**
   - Verify efficiency of memory allocation and deallocation.
   - Check for memory leaks or inefficient memory utilization.

5. **Error Handling and Robustness**
   - Test with various input scenarios, including edge cases, to check error handling.
   - Confirm graceful handling of unexpected inputs without crashing or hanging.

6. **Performance**
   - Assess execution time for different programs.
   - Measure efficiency of scheduling algorithms in managing processes.

7. **Debugging**
   - Identify and resolve any encountered issues or bugs during testing.
   - Ensure the program is free from logical errors and runs smoothly under different scenarios.
