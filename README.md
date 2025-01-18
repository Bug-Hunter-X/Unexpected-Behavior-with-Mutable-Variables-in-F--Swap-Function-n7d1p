# F# Mutable Variable Swap Bug

This example demonstrates a common misconception when working with mutable variables in F#.  In F#, mutable variables are passed by reference, not by value.  This means that changes made to the variables within a function directly affect the original variables.

The `swap` function attempts to swap the values of `x` and `y`, but due to pass-by-reference, this doesn't work as intended. The bug.fs file contains the problematic code, and the bugSolution.fs file offers a corrected version.

## Bug

The code in `bug.fs` attempts to swap two mutable variables, but unexpectedly modifies both original variables.