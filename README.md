# Lua Recursive Function Iteration Bug

This repository demonstrates a potential issue with Lua's `pairs` iterator when used in recursive functions that modify the table being iterated over.  The bug manifests as unpredictable behavior due to the change in table structure during iteration.

The `bug.lua` file contains a function that recursively iterates over a table.  The order of iteration is not guaranteed, leading to potential errors if the table is modified during the iteration.

The `bugSolution.lua` file provides a corrected version which avoids modifying the table during iteration, ensuring predictable results.