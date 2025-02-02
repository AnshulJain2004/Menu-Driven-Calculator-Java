# Menu Driven Calculator in Java

A simple Java application showcasing:
1. **A menu-driven calculator** (with basic operations like addition, subtraction, multiplication, division, square root, power, mean, and variance).
2. **Various input handling methods** in Java (using `Scanner`, `BufferedReader`, `DataInputStream`, `Console`, and command-line arguments).

This project is organized into four main Java files:
- **Calculator.java**  
- **InputProcessor.java**  
- **InputDemoMain.java**  
- **MainClass.java**

## Features

1. **Calculator Class**  
   - Implements basic arithmetic operations: add, subtract, multiply, divide.  
   - Supports additional operations: square root, power, mean, and variance.
   - Simple, reusable methods that throw an `IllegalArgumentException` when necessary (e.g., division by zero).

2. **InputDemoMain Class**  
   - Demonstrates different ways to capture user input in Java.  
   - Accepts a command-line argument for calculating a factorial.  
   - Provides a menu for choosing the input method at runtime:
     - `Scanner`
     - `BufferedReader`
     - `DataInputStream`
     - `Console`
   - Showcases how to switch between different input methods gracefully.

3. **InputProcessor Class**  
   - Provides static methods for reading user input via different Java I/O classes.  
   - Contains a `factorial` method to demonstrate a recursive solution.

4. **MainClass**  
   - Presents a text-based menu to perform calculator operations:
     1. Add  
     2. Subtract  
     3. Multiply  
     4. Divide  
     5. Square Root  
     6. Power  
     7. Mean  
     8. Variance  
     9. Exit  
   - Demonstrates how to process and display results.
   - Uses `Scanner` to collect numbers from the user.  
   - Implements a helper method (`readNumbers`) to read multiple numbers until the user types `end`.

---

## How to Run

You can run the program(s) in two primary ways:

### 1. Running the Calculator (MainClass)

1. **Compile** all the `.java` files:
   ```bash
   javac Calculator.java InputProcessor.java InputDemoMain.java MainClass.java
   ```
2. **Run** the `MainClass`:
   ```bash
   java MainClass
   ```
3. **Follow the on-screen menu** to perform different calculator operations.

### 2. Demonstrating Different Input Methods (InputDemoMain)

1. **Compile** all the `.java` files:
   ```bash
   javac Calculator.java InputProcessor.java InputDemoMain.java MainClass.java
   ```
2. **Option A**: **Run** and provide a command-line argument for factorial:
   ```bash
   java InputDemoMain 5
   ```
   - This calculates the factorial of `5` and displays the result immediately.
   
3. **Option B**: **Run** without arguments to see the menu for choosing the input method:
   ```bash
   java InputDemoMain
   ```
   - You will see a prompt to select an input method:
     1. Scanner
     2. BufferedReader
     3. DataInputStream
     4. Console

   - After choosing an input method, you’ll be prompted to enter a number. The program will then calculate its factorial.

---

## Code Organization

- **Calculator.java**  
  Houses all arithmetic operations.

- **InputDemoMain.java**  
  - Entry point for demonstrating multiple input methods and factorial calculation.
  - If a command-line argument is present, it directly calculates the factorial.
  - Otherwise, presents an input method selection menu.

- **InputProcessor.java**  
  - Contains the static methods for reading user input (`Scanner`, `BufferedReader`, `DataInputStream`, `Console`).
  - Contains the `factorial` method for demonstration.

- **MainClass.java**  
  - Entry point for the main Calculator application.
  - Provides a loop-based menu for different math operations.
  - Uses `Calculator` class methods to perform calculations.
  - Reads multiple inputs until `end` is typed for mean and variance calculations.

---

## Usage Examples

### Calculator Example (MainClass)
```
Calculator Menu:
1. Add
2. Subtract
3. Multiply
4. Divide
5. Square Root
6. Power
7. Mean
8. Variance
9. Exit
Enter your choice: 1
Enter two numbers: 10 5
Result: 15.0
```

### Input Methods Example (InputDemoMain)

1. **Command-Line Argument**  
   ```bash
   java InputDemoMain 5
   ```
   **Output**:  
   ```
   Factorial of 5 (via Command Line): 120
   ```

2. **Interactive Menu** (no command-line arguments):
   ```
   Select input method:
   1. Scanner
   2. BufferedReader
   3. DataInputStream
   4. Console
   Your choice: 1
   Enter a number (Scanner): 5
   Factorial of 5: 120
   ```

---

## Contributing

- Fork this repository.
- Create a new branch for your feature or bug fix.
- Make your changes and submit a pull request.

---

## License

This project is licensed under the [MIT License](LICENSE).  
You are free to use, modify, and distribute this software according to the terms of the MIT License.

---
