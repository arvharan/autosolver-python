🧮 Polynomial Solver & Creator
This project provides a robust, high-precision tool for handling polynomial equations of any degree. It leverages SymPy for algebraic accuracy and IPython for elegant LaTeX rendering.

🚀 Features
Dual Mode Operation: Switch between solving existing equations or creating new ones from known roots.
Natural Math Notation: Supports ^ for exponents and implicit multiplication (e.g., 9x instead of 9*x).
Complex Number Support: Fully handles imaginary roots (using i or j notation).
Factored Output: Automatically detects repeated roots to present equations in their simplest factored form (e.g.,  (𝑥−1)10=0 ).
Beautiful Formatting: High-visibility LaTeX output for clear reading of mathematical steps.
🛠 How to Use
1. Solve Mode (mode = 'solve')
Finds all roots (real and complex) of a given polynomial.

Input: Enter your equation in the question variable.
Example: x^3 - 9x^2 + 25x - 17
2. Create Mode (mode = 'create')
Generates a simplified polynomial equation based on a list of roots.

Input: List your roots in the roots_input string using the format x1=val, x2=val etc.
Example:
x1=4+i
x2=4-i
x3=1
🧪 Technical Details
Engine: Uses sympy.roots for exact algebraic solutions and nroots as a numerical fallback.
Parsing: Uses custom transformations to handle caret notation and implicit multiplication.
Rendering: Uses IPython.display.Math with \Large styling for a professional appearance.
