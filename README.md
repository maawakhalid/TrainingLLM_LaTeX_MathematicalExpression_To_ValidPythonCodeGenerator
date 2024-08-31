# TrainingLLMs: LaTeX MathematicalExpression To Valid PythonCode
Given a LaTeX expression, train an LLM to generate valid python code.

# Description
This project focuses on developing a model to convert LaTeX mathematical expressions into executable Python code. The project was part of a competition where participants trained language models to accurately translate LaTeX expressions into valid Python code that maintains the intended functionality.

# Problem Statement
The primary challenge is to generate functionally correct Python code from LaTeX expressions. Participants were provided with a dataset containing LaTeX-Python code pairs, which served as the training data for their models. The goal is to ensure the generated Python code correctly implements the operations described by the LaTeX input.

# Objectives
Participants in the competition were tasked to:

- Train language models using the provided LaTeX-Python pairs.
- Generate Python code for a set of test LaTeX inputs.
- Execute the generated Python code on specific test inputs and save the results along with task IDs in a CSV file.
- Submit the CSV file for evaluation.

# Types of Equations
The dataset includes a wide variety of equations across 14 types:

1. Algebraic
2. Multivariable Algebraic
3. Trigonometric
4. Logarithmic
5. Exponential
6. Exponential Decay
7. Geometric
8. Diophantine
9. Summation
10. Rational
11. Fractional
12. Derivative
13. Integration
14. Differential Equations

## Example Conversion
**Equation type:** Logarithmic

**Mathematical Expression**
```scss
3log(10x) + 10
```

**LaTeX Expression:**

```latex
3 \log{\left(10 x \right)} + 10
```

**Solution (Python Code):**

String: "from sympy import log\n\ndef logrithmic_function(x):\n return 3log(10x) + 10\n"

```python
from sympy import log

def logrithmic_function(x):
    return 3*log(10*x) + 10
```
