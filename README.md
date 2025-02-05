# Lua Nested Table Iteration Bug

This repository demonstrates a subtle bug related to iteration order in nested Lua tables using the `pairs` iterator.  Lua's `pairs` iterator doesn't guarantee any specific order, which can lead to unexpected results when processing nested data structures where the iteration order matters.

## Bug Description
The `bug.lua` file contains a function `foo` that recursively iterates through a nested table.  The correct behavior depends on consistent iteration order; however, Lua doesn't provide this guarantee.

## Solution
The `bugSolution.lua` file provides a solution demonstrating how to maintain consistent iteration order if it's necessary.