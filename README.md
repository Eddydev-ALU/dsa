# DSA HW01 - Sparse Matrix

This project implements sparse matrix operations in Python. It efficiently handles large matrices where most values are zero by storing only the non-zero elements.

## Features
- Read sparse matrices from text files
- Perform addition, subtraction, and multiplication
- Validate input file format and handle errors
- Simple command-line interface
- No external libraries required

## Folder Structure

```
DSA/
├── README.md
├── sparse_matrix/
│   ├── code/
│   │   └── src/
│   │       ├── sparse_matrix.py
│   │       └── results/
│   │           ├── addition_result.txt
│   │           ├── subtraction_result.txt
│   │           └── multiplication_result.txt
│   └── sample_inputs/
│       └── easy_sample_03_1.txt
```

## File Format
Each input file should look like this:
```
rows=3
cols=3
(0, 0, 5)
(1, 2, -3)
(2, 1, 7)
```
- First two lines specify dimensions
- Each remaining line is a non-zero value in (row, col, value) format

## How to Run
1. Navigate to the code directory:
    ```bash
    cd sparse_matrix/code/src/
    ```
2. Run the program:
    ```bash
    python sparse_matrix.py
    ```
3. Enter the paths to two input files and select the operation:
    - 1 = Add
    - 2 = Subtract
    - 3 = Multiply
4. Follow the on screen instruction

## Output
The result is saved in a file (e.g. `addition_result.txt`) in the same format as the inputs.

## Error Handling
- Raises errors for invalid formats or incompatible matrix sizes
- Ignores extra spaces
- Skips out-of-bounds entries
- I deleted multiplication result because it is too big to be pushed on github.