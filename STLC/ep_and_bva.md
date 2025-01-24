1. Identify and Define Equivalence Classes for the Input Domain

Valid Equivalence Classes (Input Domain):

Scores between 0-49 → Classification: "Fail"
Scores between 50-69 → Classification: "Pass"
Scores between 70-89 → Classification: "Merit"
Scores between 90-100 → Classification: "Distinction"
Invalid Equivalence Classes (Input Domain):

Scores less than 0 → Classification: "Invalid Input"
Scores greater than 100 → Classification: "Invalid Input"

2. Identify and Define Boundary Values for the Input Domain

Boundary Values for Valid Inputs:

Boundary between "Fail" and "Pass": 49, 50
Boundary between "Pass" and "Merit": 69, 70
Boundary between "Merit" and "Distinction": 89, 90
Lower boundary of valid input: 0
Upper boundary of valid input: 100
Boundary Values for Invalid Inputs:

Just below the lower valid boundary: -1
Just above the upper valid boundary: 101
# Test Cases Based on Equivalence Partitioning and Boundary Value Analysis

| Test Case ID | Description                              | Input Score | Expected Output  |
|--------------|------------------------------------------|-------------|------------------|
| TC1          | Lower boundary of "Fail" classification | 0           | "Fail"           |
| TC2          | Upper boundary of "Fail" classification | 49          | "Fail"           |
| TC3          | Lower boundary of "Pass" classification | 50          | "Pass"           |
| TC4          | Upper boundary of "Pass" classification | 69          | "Pass"           |
| TC5          | Lower boundary of "Merit" classification | 70          | "Merit"          |
| TC6          | Upper boundary of "Merit" classification | 89          | "Merit"          |
| TC7          | Lower boundary of "Distinction" classification | 90    | "Distinction"    |
| TC8          | Upper boundary of "Distinction" classification | 100   | "Distinction"    |
| TC9          | Just below the valid lower boundary      | -1          | "Invalid Input"  |
| TC10         | Just above the valid upper boundary      | 101         | "Invalid Input"  |
| TC11         | Midpoint of "Fail" classification        | 25          | "Fail"           |
| TC12         | Midpoint of "Pass" classification        | 60          | "Pass"           |
| TC13         | Midpoint of "Merit" classification       | 80          | "Merit"          |
| TC14         | Midpoint of "Distinction" classification | 95          | "Distinction"    |
