# PRODIGY_ST_01

Test cases for a simple calculator application, Prodigy InfoTech Software Testing Internship

## Prodigy InfoTech – Software Testing Task 01
### Calculator Application Testing

This repository contains the manual functional testing work completed as part of the Software Testing Internship at Prodigy InfoTech.

**Tester:** Priyanshu Sahoo

---

## Objective

The objective of this task is to create and execute test cases for a calculator web application and verify its functionality under normal, invalid, and edge-case conditions.

## Application Under Test

- **Application:** sCalc Calculator
- **Website:** https://dunizb.github.io/sCalc/

## Testing Type

- Manual Functional Testing
- Positive Testing
- Negative Testing
- Boundary and Edge Case Testing

## Testing Scope

The calculator was tested for:

- Addition
- Subtraction
- Multiplication
- Division
- Decimal calculations
- Negative results
- Order of operations (BODMAS)
- Percentage
- Clear Entry (CE)
- Backspace
- Division by zero
- Multiple decimal points
- Consecutive operators
- Repeated equals
- Large number calculations
- Non-numeric (alphabetic) character input
- Input and stability testing

## Test Environment

| Item | Details |
|---|---|
| Browser | Google Chrome |
| Operating System | Windows |
| Testing Type | Manual Functional Testing |
| Application | sCalc Calculator |
| Testing Date | 07 October 2026 |

## Test Cases

The detailed test cases and execution results are available in:

**``**

The Excel file contains:

- Test scenarios
- Preconditions
- Test steps
- Test data
- Expected results
- Actual results
- Test status
- Test Summary (separate sheet)
- Defect Log (separate sheet)
- Test date (separate sheet)

Any failed test cases identified during execution are documented based on the actual behavior of the application. Defects are reported based on actual testing evidence.

## Test Summary

| Total | Passed | Failed | Blocked | Not Executed |
|       |        |        |         |              |
|   36  |   30   |    6   |    0    |       0      |

## Defects Found

| Bug ID | Test Case(s) | Summary | Severity |
|---|---|---|---|
| BUG_01 | TC-015, TC-016, TC-018 | Calculator ignores BODMAS and evaluates left to right (e.g., `2 + 3 × 4` gives 20 instead of 14) | Medium |
| BUG_02 | TC-019 | Division by zero shows raw `Infinity` instead of a user-friendly error message | Low |
| BUG_03 | TC-022 | `NaN` shown when an expression starts with an operator | Low |
| BUG_04 | TC-030 | `200 × 10 %` returns `0` instead of the expected percentage result | Low |

Full steps to reproduce, expected results, and actual results are in the **Defect Log** sheet of the Excel file.

## Key Observations

- Basic arithmetic and decimal operations work correctly.
- The calculator evaluates expressions strictly left to right and does not follow BODMAS.
- Invalid input (extra operators, repeated decimal points, keyboard letters) is handled without crashing.
- Division by zero and a leading operator show raw values (`Infinity`, `NaN`) instead of clear messages.
- Very large results are shown in scientific notation (`9.99999998E+17`), so precision is lost.
- `CE` clears the whole expression, not only the current entry.

## What I Learned

- How to write structured test cases with clear preconditions, steps, and expected results
- The difference between positive (valid input) and negative (invalid input) testing
- How to test boundary and edge cases such as zero, large numbers, and repeated decimal points
- How to report a defect with reproducible steps, severity, and status
- Why expected results should be specific, so each test is clearly a Pass or a Fail

## Conclusion

The sCalc calculator application was tested using manual functional testing techniques. The test cases cover normal operations, invalid inputs, edge cases, calculator controls, and operator behavior.

The results documented in the Excel file represent the actual observed behavior of the application during testing.
