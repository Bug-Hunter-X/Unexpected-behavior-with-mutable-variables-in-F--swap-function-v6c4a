# F# Mutable Variable Swap Bug

This repository demonstrates a common error involving mutable variables in F#.  The `swap` function attempts to swap the values of two mutable variables, but due to how mutable variables are handled in F#, it doesn't work as expected.

The `bug.fs` file contains the buggy code, while `bugSolution.fs` provides a corrected version.  The issue stems from the fact that mutable variables are passed by reference, leading to unexpected side effects when used within functions.

## How to Reproduce

1. Clone this repository.
2. Open `bug.fs` in an F# environment.
3. Run the code. The output will be unexpected.
4. Open `bugSolution.fs` to see the corrected code. 
5. Run the corrected code. Observe the correct output.