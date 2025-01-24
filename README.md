# Pythagorean Triple Finder

This C program calculates the missing value in a Pythagorean triple, which consists of three integers that satisfy the equation \(a^2 + b^2 = c^2\). The program takes an input file containing two integers, reads the values, and determines if they can form two sides of a right triangle. If they can, it calculates and outputs the third integer to complete the Pythagorean triple. If the given integers cannot form a valid triple, the program outputs `-1`.

## How It Works

1. **Input**:
   - The program reads two integers from a specified text file

2. **Validation**:
   - It checks if the two integers can form a valid Pythagorean relationship

3. **Calculation**:
   - If valid, the program calculates the missing side (either the hypotenuse or one of the legs)
   - If not, it outputs `-1`

4. **Output**:
   - The program outputs the calculated value or `-1` if no valid Pythagorean triple exists

This implementation includes robust handling of edge cases and is designed for use with predefined test cases and randomized inputs for validation

---

## Table of Contents

- [Features](#features)
- [Usage](#usage)
- [Code Structure](#code-structure)
- [Requirements](#requirements)
- [File Output](#file-output)
- [License](#license)
- [Important Note](#important-note)

---

## Features

- **Pythagorean Triple Verification**: 
  - Given two integers, the program determines if they can form a valid Pythagorean triple
  - Outputs the third integer if valid or `-1` if not
    
- **Test Cases**: 
  - Includes sample input files in the `tests/` directory with expected outputs in the `answers/` directory
    
- **Makefile**: 
  - Simplifies compilation with necessary compiler flags for error checking and debugging

---

## Usage

1. **Setup**:
   - Rename the provided file:
     ```bash
     mv pythagorean_provided.c pythagorean.c
     ```

2. **Compile the program**:
   - Using GCC:
     ```bash
     gcc -Wall -Werror -fsanitize=address -std=c99 -o pythagorean pythagorean.c -lm
     ```
   - Or with the Makefile:
     ```bash
     make
     ```

3. **Run the Program**:
   - Provide an input file:
     ```bash
     ./pythagorean tests/test0.txt
     ```

---

## Code Structure

- **pythagorean.c**:
  - The primary source code for determining Pythagorean triples
    
- **Makefile**:
  - Automates compilation with proper flags
     
- **tests/**:
  - Contains input files for testing
     
- **answers/**:
  - Contains expected output files

---

## Requirements

- Linux environment
  
- **Tools**: 
  - GCC (C Compiler)

---

## File Output

- Outputs the missing value of a Pythagorean triple or `-1` if no triple exists

- **Example Output**:
  ```bash
  Input: 
  5
  3
  
  Output: 
  4


 
## License

This project is licensed under the MIT License. See the LICENSE file for details.


## Important Note

This project emphasizes learning the Linux command line, compiling C programs, and understanding Pythagorean triples.
