# Threaded Calculator Application

A multi-threaded Java application that demonstrates concurrent execution by performing arithmetic operations in a separate thread while maintaining a responsive user interface.


## Features
-  Basic arithmetic operations (addition, subtraction, multiplication, division)
-  Each operation executes in a separate thread
-  Division by zero handling
-  Simple console-based menu interface
-  Synchronous operation flow with thread joining
-  Basic thread interruption handling

## Prerequisites
- Java Development Kit (JDK) 17 or later
- Basic understanding of Java threading concepts

## Installation
1. Clone the repository or download the source files:
   ```bash
   git clone https://github.com/your-repo/threaded-calculator.git
   cd threaded-calculator

## Main Components:
OperationTask Class

Implements Runnable interface

Contains operation logic in run() method

Handles all arithmetic operations in a thread-safe manner

Main Class

Manages application lifecycle

Creates and starts operation threads

Implements thread joining for synchronous flow

Threading Model
Thread Creation: New thread spawned for each operation

Thread Joining: Main thread waits for operation completion

Error Handling: Basic interruption handling

Resource Management: No shared resources (thread-safe by design)

## Sample Output
=== Calculator Menu ===
1. Addition
2. Subtraction
3. Multiplication
4. Division
5. Exit
Enter your choice (1-5): 3
Enter first number: 5
Enter second number: 4
Operation Thread: Product = 20.0

=== Calculator Menu ===
1. Addition
2. Subtraction
3. Multiplication
4. Division
5. Exit
Enter your choice (1-5): 5
Thank you for using the calculator. Goodbye!
