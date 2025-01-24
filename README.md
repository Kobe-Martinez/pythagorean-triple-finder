# Pythagorean Triple Finder

This project implements a C program to determine the missing value in a Pythagorean triple given two integers. The program reads input from a file, computes the missing value (if a valid triple exists), and outputs the result. The repository includes test cases, an autograder, and a Makefile for compilation.


## Table of Contents

- [Features](#features)
- [Usage](#usage)
- [Code Structure](#code-structure)
- [Requirements](#requirements)
- [File Output](#file-output)
- [License](#license)
- [Important Note](#important-note)


## Features

- **Pythagorean Triple Verification**: 

  - Given two integers, the program determines if they can form a valid Pythagorean triple
  
  - Outputs the third integer if valid or `-1` if not
    
- **Test Cases**: 

  - Includes sample input files in the `tests/` directory with expected outputs in the `answers/` directory

- **Autograder**: 

  - Automates testing of the program against predefined and random test cases
    
- **Makefile**: 

  - Simplifies compilation with necessary compiler flags for error checking and debugging
        

## Usage

1. **Setup**:
   
   - Rename the provided file:
   
   ```bash
   mv pythagorean_provided.c pythagorean.c

2. **Compile the program**:
      
   - Using GCC:
     
   ```bash
   gcc -Wall -Werror -fsanitize=address -std=c99 -o pythagorean pythagorean.c -lm
       
   - Or with the Makefile:
      
   ```bash
   make
   
3. **Run the Program**:
   
   - Provide an input file
     
    ```bash
   ./pythagorean tests/test0.txt
     

## Code Structure

- **pythagorean.c**:
  
  - The primary source code for determining Pythagorean triples
    
- **Makefile**:
  
   - Automates compilation with proper flags
     
- **tests/**:
  
   - Contains input files for testing
     
- **answers/**:
  
   - Contains expected output files


## Requirements

- Linux environment
  

- **Tools**: 

  - GCC (C Compiler)
      

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

This project emphasizes learning the Linux command line, compiling C programs, and understanding Pythagorean triples
